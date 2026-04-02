To find the velocity and position, we move "up" the ladder of motion. Instead of taking derivatives (like we did in your previous problem), we use **integration** to work backward from Force to Position.

### 1. Acceleration ($\vec{a}$)
First, we find acceleration using $a = \frac{F}{m}$. Since the mass $m = 3 \text{ kg}$, we divide every part of the force by 3:
* $a_x = \frac{15t}{3} = 5t$
* $a_y = \frac{3t - 12}{3} = t - 4$
* $a_z = \frac{-6t^2}{3} = -2t^2$

**$\vec{a}(t) = (5t, t - 4, -2t^2)$**

---

### 2. Velocity ($\vec{v}$)
Velocity is the integral of acceleration plus the initial velocity ($\vec{v}_0$).
* $v_x = \int 5t \, dt = 2.5t^2 + v_{0x} = \mathbf{2.5t^2 + 2}$
* $v_y = \int (t - 4) \, dt = 0.5t^2 - 4t + v_{0y} = \mathbf{0.5t^2 - 4t + 0}$
* $v_z = \int -2t^2 \, dt = -\frac{2}{3}t^3 + v_{0z} = \mathbf{-\frac{2}{3}t^3 + 1}$



---

### 3. Position ($\vec{r}$)
Position is the integral of velocity plus the initial position ($\vec{r}_0$).
* $x = \int (2.5t^2 + 2) \, dt = \frac{2.5}{3}t^3 + 2t + x_0 = \mathbf{\frac{5}{6}t^3 + 2t + 5}$
* $y = \int (0.5t^2 - 4t) \, dt = \frac{0.5}{3}t^3 - 2t^2 + y_0 = \mathbf{\frac{1}{6}t^3 - 2t^2 + 2}$
* $z = \int (-\frac{2}{3}t^3 + 1) \, dt = -\frac{2}{12}t^4 + t + z_0 = \mathbf{-\frac{1}{6}t^4 + t - 3}$

---

### Summary of Results
| Quantity | Time-Dependent Equation |
| :--- | :--- |
| **Velocity** $\vec{v}(t)$ | $(2.5t^2 + 2, \,\, 0.5t^2 - 4t, \,\, -\frac{2}{3}t^3 + 1)$ |
| **Position** $\vec{r}(t)$ | $(\frac{5}{6}t^3 + 2t + 5, \,\, \frac{1}{6}t^3 - 2t^2 + 2, \,\, -\frac{1}{6}t^4 + t - 3)$ |

**Note:** The constants at the end of each equation (like $+5, +2, -3$) are the starting coordinates you provided. If you plug in $t=0$, you get your exact initial conditions back!
