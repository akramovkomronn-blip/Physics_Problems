```python?code_reference&code_event_index=2
import numpy as np

m = 10
A = 0.2
omega = 10 * np.pi

k = m * (omega**2)
E = 0.5 * k * (A**2)

print(f"{k=}")
print(f"{E=}")


```
```text?code_stdout&code_event_index=2
k=9869.604401089358
E=197.3920880217872

```
To find the spring constant and the total mechanical energy, we start by analyzing the given displacement equation for simple harmonic motion:

$$x(t) = 0.2 \cos(10\pi t)$$

The standard form for the displacement of an oscillating mass is:
$$x(t) = A \cos(\omega t + \phi)$$

From the equation, we can identify:
* **Amplitude ($A$):** $0.2 \text{ m}$
* **Angular frequency ($\omega$):** $10\pi \text{ rad/s}$
* **Mass ($m$):** $10 \text{ kg}$

---

### 1. Spring Constant ($k$)
The angular frequency $\omega$ of a mass-spring system is related to the mass and spring constant by the formula:
$$\omega = \sqrt{\frac{k}{m}}$$

Squaring both sides and solving for $k$:
$$k = m \omega^2$$

Substituting the known values:
$$k = 10 \cdot (10\pi)^2$$
$$k = 10 \cdot 100\pi^2$$
$$k = 1000\pi^2 \text{ N/m}$$

Using $\pi^2 \approx 9.87$:
$$k \approx 9869.6 \text{ N/m}$$

---

### 2. Total Mechanical Energy ($E$)
The total mechanical energy in a simple harmonic oscillator is given by the sum of kinetic and potential energy, which remains constant and is equal to the maximum potential energy at the amplitude:
$$E = \frac{1}{2} k A^2$$

Substituting the values for $k$ and $A$:
$$E = \frac{1}{2} (1000\pi^2) (0.2)^2$$
$$E = 500\pi^2 \cdot 0.04$$
$$E = 20\pi^2 \text{ J}$$

Using $\pi^2 \approx 9.87$:
$$E \approx 197.39 \text{ J}$$

---

### **Summary of Results**
* **Spring Constant ($k$):** $1000\pi^2 \text{ N/m} \approx 9869.6 \text{ N/m}$
* **Total Mechanical Energy ($E$):** $20\pi^2 \text{ J} \approx 197.4 \text{ J}$
