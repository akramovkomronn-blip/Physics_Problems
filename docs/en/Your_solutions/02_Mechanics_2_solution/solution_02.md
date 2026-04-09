```python?code_reference&code_event_index=2
import math

m = 10
A = 0.2
omega = 10 * math.pi

# Spring constant k
k = m * (omega**2)

# Total Mechanical Energy E
E = 0.5 * k * (A**2)

print(f"{k=}")
print(f"{E=}")


```
```text?code_stdout&code_event_index=2
k=9869.604401089358
E=197.3920880217872

```
To find the spring constant and total mechanical energy, we analyze the given displacement equation for simple harmonic motion (SHM).

The general form of the equation is:
$$x(t) = A \cos(\omega t + \phi)$$

Comparing this to your equation, $x(t) = 0.2 \cos(10\pi t)$, we can identify:
* **Amplitude ($A$):** $0.2 \text{ m}$
* **Angular frequency ($\omega$):** $10\pi \text{ rad/s}$
* **Mass ($m$):** $10 \text{ kg}$



### 1. Finding the Spring Constant ($k$)
The relationship between angular frequency, mass, and the spring constant is given by the formula:
$$\omega = \sqrt{\frac{k}{m}}$$

Squaring both sides and solving for $k$:
$$k = m \omega^2$$

Substituting the known values:
$$k = 10 \cdot (10\pi)^2$$
$$k = 10 \cdot 100\pi^2$$
$$k = 1000\pi^2 \text{ N/m}$$

Using the numerical value of $\pi \approx 3.14159$:
$$k \approx 1000 \cdot 9.8696$$
**$k \approx 9869.60 \text{ N/m}$**

---

### 2. Finding the Total Mechanical Energy ($E$)
The total mechanical energy in a mass-spring system is constant and can be calculated using the maximum potential energy (at the amplitude):
$$E = \frac{1}{2} k A^2$$



Substituting the values for $k$ and $A$:
$$E = \frac{1}{2} (1000\pi^2) \cdot (0.2)^2$$
$$E = 500\pi^2 \cdot 0.04$$
$$E = 20\pi^2 \text{ J}$$

Using the numerical value:
$$E \approx 20 \cdot 9.8696$$
**$E \approx 197.39 \text{ J}$**

**Summary:**
* **Spring Constant ($k$):** $\approx 9869.60 \text{ N/m}$
* **Total Mechanical Energy ($E$):** $\approx 197.39 \text{ J}$
