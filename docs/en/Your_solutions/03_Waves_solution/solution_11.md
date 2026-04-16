This HTML5 simulation uses the **Canvas API** to visualize Young's double-slit interference. It calculates the displacement at every pixel based on the superposition of two spherical waves originating from $r_1$ and $r_2$.

To maintain performance while calculating thousands of sine functions per frame, the simulation uses a slightly optimized version of your displacement formula.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Young's Double Slit Interference</title>
    <style>
        body { margin: 0; background: #111; color: white; font-family: sans-serif; overflow: hidden; display: flex; flex-direction: column; align-items: center; }
        canvas { background: #000; cursor: crosshair; box-shadow: 0 0 20px rgba(0,255,255,0.2); }
        .controls { background: rgba(30, 30, 30, 0.9); padding: 15px; border-radius: 0 0 10px 10px; display: flex; gap: 20px; z-index: 10; }
        .control-group { display: flex; flex-direction: column; align-items: center; }
        label { font-size: 12px; margin-bottom: 5px; color: #0cf; }
        input { cursor: pointer; }
    </style>
</head>
<body>

    <canvas id="canvas"></canvas>

    <div class="controls">
        <div class="control-group">
            <label>Slit Distance (d)</label>
            <input type="range" id="slitDist" min="10" max="150" value="50">
        </div>
        <div class="control-group">
            <label>Wavelength (λ)</label>
            <input type="range" id="waveLength" min="10" max="100" value="30">
        </div>
        <div class="control-group">
            <label>Wave Speed (ω)</label>
            <input type="range" id="speed" min="1" max="10" value="5">
        </div>
    </div>

<script>
    const canvas = document.getElementById('canvas');
    const ctx = canvas.getContext('2d');
    const slitInput = document.getElementById('slitDist');
    const waveInput = document.getElementById('waveLength');
    const speedInput = document.getElementById('speed');

    let width, height;
    let time = 0;

    function resize() {
        width = canvas.width = window.innerWidth;
        height = canvas.height = window.innerHeight - 80;
    }

    window.addEventListener('resize', resize);
    resize();

    function draw() {
        const d = parseInt(slitInput.value);
        const lambda = parseInt(waveInput.value);
        const omega = parseInt(speedInput.value) / 10;
        const k = (2 * Math.PI) / lambda;
        
        const imageData = ctx.createImageData(width, height);
        const data = imageData.data;

        // Slit Positions (Centered horizontally, slightly off the left edge)
        const x1 = 50, y1 = height / 2 - d / 2;
        const x2 = 50, y2 = height / 2 + d / 2;

        // Sampling step for performance (calculating every pixel is heavy)
        const step = 2; 

        for (let y = 0; y < height; y += step) {
            for (let x = 0; x < width; x += step) {
                // Distance to each slit
                const r1 = Math.sqrt((x - x1)**2 + (y - y1)**2);
                const r2 = Math.sqrt((x - x2)**2 + (y - y2)**2);

                // Formula: u = A/r1 * sin(k*r1 - wt) + A/r2 * sin(k*r2 - wt)
                // Using A=100 for visibility
                const u1 = (100 / (r1 + 1)) * Math.sin(k * r1 - time);
                const u2 = (100 / (r2 + 1)) * Math.sin(k * r2 - time);
                
                const resultant = u1 + u2;
                
                // Map resultant to color (Cyan for peaks, Red for troughs)
                const intensity = Math.min(255, Math.abs(resultant) * 40);
                const colorOffset = (y * width + x) * 4;

                // Fill block for step size
                for (let sy = 0; sy < step; sy++) {
                    for (let sx = 0; sx < step; sx++) {
                        const idx = ((y + sy) * width + (x + sx)) * 4;
                        if (idx < data.length) {
                            data[idx] = resultant > 0 ? intensity : 0;     // Red channel
                            data[idx + 1] = intensity;                    // Green channel
                            data[idx + 2] = resultant < 0 ? intensity : intensity; // Blue channel
                            data[idx + 3] = 255;                          // Alpha
                        }
                    }
                }
            }
        }

        ctx.putImageData(imageData, 0, 0);

        // Draw Slits
        ctx.fillStyle = "white";
        ctx.fillRect(x1 - 5, y1 - 10, 5, 20);
        ctx.fillRect(x2 - 5, y2 - 10, 5, 20);

        time += omega;
        requestAnimationFrame(draw);
    }

    draw();
</script>
</body>
</html>
```

### Key Technical Features:
* **Principle of Superposition:** The code calculates the sum of two waves at every coordinate $(x, y)$.
* **Real-time Interaction:** You can adjust the **Slit Distance ($d$)** and **Wavelength ($\lambda$)** to see the interference fringes change width and frequency instantly.
* **Wave Equation Implementation:** It utilizes the spatial frequency (wave number) $k = \frac{2\pi}{\lambda}$ and angular frequency $\omega$ to animate the phase.
* **Visual Representation:** High intensity (bright fringes) represents constructive interference, while dark areas represent destructive interference where the phase difference is $\pi$.
