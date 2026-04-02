To solve this, we use the same "ladder" of integration, but since the force is constant, the math becomes even simpler.

### 1. Acceleration ($\vec{a}$)
Using Newton's Second Law ($\vec{a} = \vec{F}/m$), we divide the force by the mass ($2\text{ kg}$):
* $a_x = 6 / 2 = 3$
* $a_y = 2 / 2 = 1$
**$\vec{a}(t) = (3, 1) \text{ m/s}^2$**

### 2. Velocity ($\vec{v}$)
Velocity is the integral of acceleration plus the initial velocity $\vec{v}(0) = (1, -1)$:
* $v_x = \int 3 \, dt + 1 = 3t + 1$
* $v_y = \int 1 \, dt - 1 = t - 1$
**$\vec{v}(t) = (3t + 1, t - 1) \text{ m/s}$**

### 3. Position ($\vec{r}$)
Position is the integral of velocity plus the initial position $\vec{r}(0) = (0, 0)$:
* $x = \int (3t + 1) \, dt = 1.5t^2 + t$
* $y = \int (t - 1) \, dt = 0.5t^2 - t$
**$\vec{r}(t) = (1.5t^2 + t, 0.5t^2 - t) \text{ m}$**

### 4. Trajectory
The trajectory is a **parabola**. Since both $x$ and $y$ depend on $t^2$, the particle curves through the plane. It starts at the origin, moves slightly down and right (due to the initial $-1$ in $y$), then curves upward as the constant force takes over.



---

### 5. Work Done at $t = 3\text{ s}$
Work is the dot product of Force and Displacement ($\vec{F} \cdot \Delta\vec{r}$).
First, find the position at $t = 3$:
* $x(3) = 1.5(3)^2 + 3 = 13.5 + 3 = 16.5\text{ m}$
* $y(3) = 0.5(3)^2 - 3 = 4.5 - 3 = 1.5\text{ m}$

Now, calculate Work ($W = F_x \cdot x + F_y \cdot y$):
* $W = (6 \times 16.5) + (2 \times 1.5)$
* $W = 99 + 3 = \mathbf{102\text{ J}}$

---

### 6. Work-Energy Theorem Check
The theorem states: $W = \Delta KE = KE_{final} - KE_{initial}$.

**Initial Kinetic Energy ($t=0$):**
* $v^2 = 1^2 + (-1)^2 = 2$
* $KE_i = \frac{1}{2}(2)(2) = 2\text{ J}$

**Final Kinetic Energy ($t=3$):**
* $v_x(3) = 3(3) + 1 = 10$
* $v_y(3) = 3 - 1 = 2$
* $v^2 = 10^2 + 2^2 = 104$
* $KE_f = \frac{1}{2}(2)(104) = 104\text{ J}$

**Change in Energy:**
* $\Delta KE = 104 - 2 = \mathbf{102\text{ J}}$

**Conclusion:** Since both the Work ($102\text{ J}$) and the Change in Kinetic Energy ($102\text{ J}$) match exactly, the theorem is verified!



[Image of work-energy theorem diagram]
