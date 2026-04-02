

### 1. Equation of Motion
Using Newton's Second Law ($F = ma$), and knowing that acceleration $a$ is the second derivative of position ($d^2x/dt^2$):
$$-kx = m\frac{d^2x}{dt^2}$$
This is the equation for **Simple Harmonic Motion**. The solution is a wave:
$$x(t) = A \cos(\omega t + \phi)$$
where $\omega = \sqrt{k/m}$ is the angular frequency.

### 2. Work Done
Work is the integral of force over distance. Since the force changes as $x$ changes, we integrate:
$$W = \int_{0}^{x_0} F(x) \, dx = \int_{0}^{x_0} -kx \, dx$$
$$W = \left[ -\frac{1}{2}kx^2 \right]_{0}^{x_0} = -\frac{1}{2}kx_0^2$$

### 3. Potential Energy ($U$)
Potential energy is defined as the negative of the work done by a conservative force. Therefore:
$$U(x) = -W = \frac{1}{2}kx^2$$
This result tells us that the energy stored in a spring increases with the square of the displacement.

### 4. Verify $F = -dU/dx$
If we take the derivative of our potential energy equation:
$$\frac{dU}{dx} = \frac{d}{dx}\left(\frac{1}{2}kx^2\right) = kx$$
Applying the negative sign:
$$- \frac{dU}{dx} = -kx$$
This matches our original force $F(x)$, verifying the relationship.

---

### 5. Graphs
* **$F(x) = -kx$**: This is a **straight line** passing through the origin with a negative slope. It shows that as you pull further ($+x$), the force pulls back harder in the opposite direction ($-F$).
* **$U(x) = \frac{1}{2}kx^2$**: This is a **parabola** opening upwards. It shows that energy is always positive, whether you compress or stretch the spring.
