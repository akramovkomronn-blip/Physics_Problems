```python?code_reference&code_event_index=2
def v(t):
    return t**2 + 2*t - 5

# Acceleration a(t) = dv/dt = 2t + 2
def a(t):
    return 2*t + 2

# Position x(t) = integral(v(t)) + C
# x(t) = (1/3)t^3 + t^2 - 5t + C
# Given x(0) = 4 -> C = 4
def x(t):
    return (1/3)*t**3 + t**2 - 5*t + 4

t_val = 3
accel_at_3 = a(t_val)
pos_at_3 = x(t_val)

print(f"{accel_at_3=}")
print(f"{pos_at_3=}")

```
```text?code_stdout&code_event_index=2
accel_at_3=8
pos_at_3=7.0

```
To find the position and acceleration, we use the "calculus ladder" of motion. Starting with **velocity**, we move "up" to find acceleration and "down" to find position.

### 1. Finding Acceleration ($a$)
Acceleration is the **derivative** of velocity ($a = \frac{dv}{dt}$):
* **Formula:** $\frac{d}{dt}(t^2 + 2t - 5) = 2t + 2$
* **At $t=3$:** $a(3) = 2(3) + 2 = \mathbf{8 \text{ m/s}^2}$



---

### 2. Finding Position ($x$)
Position is the **integral** of velocity ($x = \int v(t) \, dt$).
* **The Integral:** $x(t) = \int (t^2 + 2t - 5) \, dt = \frac{1}{3}t^3 + t^2 - 5t + C$
* **Find $C$ (Initial Condition):** We know at $t=0, x=4$.
    $$4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C \implies C = 4$$
* **The Full Equation:** $x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$

Now, calculate for **$t=3$**:
* $x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4$
* $x(3) = 9 + 9 - 15 + 4 = \mathbf{7 \text{ m}}$



---

### **Simple Summary for Your Professor**
> "I found the **acceleration** by taking the derivative of the velocity function, which gave me $2t + 2$. At $3$ seconds, that equals $8 \text{ m/s}^2$. To find the **position**, I integrated the velocity function and added the constant of $4$ from our initial condition. Plugging in $3$ seconds into that position formula, the object's location is at **$7$ meters**."

| Property | Value at $t=3$ |
| :--- | :--- |
| **Acceleration** | $8 \text{ m/s}^2$ |
| **Position** | $7 \text{ m}$ |
