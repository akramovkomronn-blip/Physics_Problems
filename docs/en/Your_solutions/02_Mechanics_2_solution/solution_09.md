This problem explores how air resistance (drag) changes the classic "projectile motion" we see in textbooks. 

### 1. Analytical Solution
The equation of motion is $m\frac{dv}{dt} = -mg - kv$. We can rewrite this to separate the variables ($v$ and $t$):

$$\frac{dv}{g + \frac{k}{m}v} = -dt$$

Integrating both sides and applying the initial condition $v(0) = v_0$, we get the velocity as a function of time:
$$v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}$$

To find the position $x(t)$, we integrate the velocity and apply $x(0) = 10$:
$$x(t) = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)(1 - e^{-\frac{k}{m}t}) - \frac{mg}{k}t$$



---

### 2. Maximum Height
The object reaches its maximum height when its velocity is zero ($v(t) = 0$). 
1.  **Find time to peak ($t_p$):** Set the velocity equation to zero and solve for $t$:
    $$t_p = \frac{m}{k} \ln\left(1 + \frac{kv_0}{mg}\right)$$
2.  **Find $x_{max}$:** Plug $t_p$ back into the $x(t)$ equation. This results in a height that is **lower** than the vacuum case because drag is constantly removing energy.

---

### 3. Comparison with No Drag
| Feature | No Drag ($k=0$) | With Drag ($k>0$) |
| :--- | :--- | :--- |
| **Velocity** | Linear decrease: $v = v_0 - gt$ | Exponential decay toward terminal velocity |
| **Max Height** | Higher: $H = \frac{v_0^2}{2g}$ | Lower: Energy is lost to heat/friction |
| **Symmetry** | Time up = Time down | Time to fall is longer than time to rise |

[Image comparing trajectories of projectile motion with and without air resistance]

---

### 4. Numerical Simulation (Python)
Numerical methods (like Euler's method) are great for when math gets messy. Here is a simple script to compare the two:

```python
import numpy as np

# Constants
m, g, k = 0.5, 9.8, 0.1
v, x = 20.0, 10.0  # Initial conditions
dt = 0.01

# Simulation Loop
while v > 0: # Only simulating the upward trip
    f_drag = -k * v
    f_grav = -m * g
    a = (f_grav + f_drag) / m
    
    v += a * dt
    x += v * dt

print(f"Max Height with Drag: {x:.2f} m")
```

This code calculates the forces at every tiny step ($0.01\text{s}$) to find the peak height. Because the drag force changes as the velocity changes, these tiny steps accurately "track" the curve that simple algebra can't easily solve.
