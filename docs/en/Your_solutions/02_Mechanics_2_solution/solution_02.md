To format these physics problems for a GitHub README or a markdown file, you can use the code block below. This uses standard Markdown syntax with LaTeX for clean math rendering.

```markdown
# Physics Problems: Oscillations and Gravitation

## 1. Gravitational Dependence
**Problem:** A simple pendulum has a period of 4 seconds on Earth. What would its period be on the Moon, where the gravitational acceleration is about 1/6th of Earth's? What is the required length of a simple pendulum to have a period of exactly 1 second on Earth?

### Solution
The period of a simple pendulum is defined by:
$$T = 2\pi \sqrt{\frac{L}{g}}$$

#### Part A: Period on the Moon
Given $T_{Earth} = 4\text{s}$ and $g_{Moon} = \frac{1}{6}g_{Earth}$:
* Since $T \propto \frac{1}{\sqrt{g}}$, the new period is $T_{Moon} = T_{Earth} \times \sqrt{6}$.
* $T_{Moon} = 4 \times \sqrt{6} \approx \mathbf{9.80\text{s}}$

#### Part B: Required Length on Earth
To find $L$ for $T = 1\text{s}$ on Earth ($g \approx 9.81\text{m/s}^2$):
* Rearranging for $L$: $L = \frac{T^2 g}{4\pi^2}$
* $L = \frac{1^2 \times 9.81}{4\pi^2} \approx \mathbf{0.248\text{m}}$ (or $24.8\text{cm}$)

---

## 2. Harmonic Motion
**Problem:** A 10 kg mass is attached to a spring and oscillates according to the equation $x(t) = 0.2\cos(10\pi t)$ (in meters). What is the spring constant $k$? What is the total mechanical energy of the system?

### Solution
From the equation $x(t) = A\cos(\omega t)$, we identify:
* **Amplitude ($A$):** $0.2\text{ m}$
* **Angular Frequency ($\omega$):** $10\pi\text{ rad/s}$
* **Mass ($m$):** $10\text{ kg}$

#### Part A: Spring Constant ($k$)
Using the relation $\omega^2 = \frac{k}{m}$:
* $k = m\omega^2$
* $k = 10 \times (10\pi)^2 = 1000\pi^2$
* $k \approx \mathbf{9869.60\text{ N/m}}$

#### Part B: Total Mechanical Energy ($E$)
Using the energy formula $E = \frac{1}{2}kA^2$:
* $E = \frac{1}{2}(1000\pi^2)(0.2)^2$
* $E = 20\pi^2$
* $E \approx \mathbf{197.39\text{ J}}$
```
