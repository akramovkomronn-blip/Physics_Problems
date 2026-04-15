### Superposition Principle: Standing Wave Derivation

When two waves with the same amplitude, frequency, and wavelength travel in opposite directions, they interfere to form a **standing wave**.

#### 1. Resulting Wave Equation

Using the principle of superposition, the resultant displacement $y(x,t)$ is the sum of the two waves:

$$y(x,t) = y_1 + y_2 = A\sin(kx - \omega t) + A\sin(kx + \omega t)$$

Applying the trigonometric identity $\sin(\alpha) + \sin(\beta) = 2\sin\left(\frac{\alpha+\beta}{2}\right)\cos\left(\frac{\alpha-\beta}{2}\right)$:

$$y(x,t) = 2A\sin(kx)\cos(\omega t)$$



---

#### 2. Identifying the Nodes

Nodes are positions where the displacement is always zero ($y = 0$). This occurs when the spatial part of the equation, $\sin(kx)$, equals zero.

$$\sin(kx) = 0$$

$$kx = n\pi \quad \text{for } n = 0, 1, 2, \dots$$

Since the wave number $k = \frac{2\pi}{\lambda}$, we substitute to find the positions $x$:

$$\left(\frac{2\pi}{\lambda}\right)x = n\pi$$

$$x = \frac{n\lambda}{2}$$



---

#### Summary
* **Standing Wave Equation:** $y(x,t) = 2A\sin(kx)\cos(\omega t)$
* 
* **Node Positions:** $x = 0, \frac{\lambda}{2}, \lambda, \frac{3\lambda}{2}, \dots$ (multiples of half-wavelengths)
