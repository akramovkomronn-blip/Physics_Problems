To derive the differential equation for a series RLC circuit, we apply **Kirchhoff’s Voltage Law (KVL)**, which states that the sum of the voltages around a closed loop must equal zero.

### **1. The RLC Circuit Differential Equation**

In a series circuit containing an inductor ($L$), a resistor ($R$), a capacitor ($C$), and a voltage source ($V$), the sum of the potential drops is:


$$V(t) = V_L + V_R + V_C$$

Using the fundamental relationships for each component ($V_L = L \frac{dI}{dt}$, $V_R = IR$, and $I = C \frac{dV_C}{dt}$), we can express the equation in terms of the capacitor voltage $V_C(t)$:

$$LC \frac{d^2V_C(t)}{dt^2} + RC \frac{dV_C(t)}{dt} + V_C(t) = V(t)$$

Dividing by $LC$ to put it in standard form:


$$\frac{d^2V_C}{dt^2} + \frac{R}{L} \frac{dV_C}{dt} + \frac{1}{LC} V_C = \frac{V(t)}{LC}$$

---

### **2. Comparison to the Damped Harmonic Oscillator**

The behavior of an RLC circuit is mathematically identical to a mechanical damped harmonic oscillator (such as a mass on a spring with friction). The mechanical equation is:


$$m \frac{d^2x}{dt^2} + b \frac{dx}{dt} + kx = F_{ext}(t)$$

Where:

* **$m$** is the mass.
* **$b$** is the damping coefficient (friction).
* **$k$** is the spring constant.
* **$x$** is the displacement.
* **$F_{ext}$** is the external driving force.

---

### **3. Analogies Between Terms**

The following table highlights the direct physical analogies between the electrical and mechanical systems:

| Electrical Term (RLC) | Mechanical Term (Oscillator) | Physical Role |
| --- | --- | --- |
| **Inductance ($L$)** | **Mass ($m$)** | Inertia (resistance to change in motion/current). |
| **Resistance ($R$)** | **Damping ($b$)** | Energy dissipation (friction/heat). |
| **Reciprocal Capacitance ($1/C$)** | **Spring Constant ($k$)** | Restoring force (stiffness). |
| **Charge ($q$) or Voltage ($V_C$)** | **Displacement ($x$)** | The state variable being tracked. |
| **Current ($I$)** | **Velocity ($v$)** | The rate of change of the state variable. |
| **Source Voltage ($V$)** | **External Force ($F$)** | The "driver" of the system. |

This mathematical symmetry is why electrical circuits are often used to model complex mechanical systems in engineering.
