To solve for the currents $I_1$, $I_2$, and $I_3$ in this two-loop circuit, we will apply **Kirchhoff’s Current Law (KCL)** and **Kirchhoff’s Voltage Law (KVL)**.

### **1. Define the Current Directions**

First, we assign directions to the currents at the top junction (node):

* **$I_1$**: Current flowing through the left loop (through $R_1$, the ammeter, and $E_1$).
* **$I_2$**: Current flowing down through the shared center branch ($R_2$).
* **$I_3$**: Current flowing through the right branch (through $E_2$ and $r_w$).

**Applying KCL at the top junction:**
The sum of currents entering a junction equals the sum of currents leaving it. Assuming $I_1$ and $I_3$ enter the junction and $I_2$ leaves it:


$$I_1 + I_3 = I_2 \implies I_3 = I_2 - I_1 \quad \text{(Equation 1)}$$

---

### **2. Apply Kirchhoff’s Voltage Law (KVL)**

We will sum the potential differences around each loop. By convention, we subtract $I \cdot R$ when moving in the direction of current and add voltage when moving from the negative to the positive terminal of a battery.

#### **Loop 1: Left Loop (Clockwise)**

Starting from the bottom-left corner and moving clockwise:


$$-I_1(R_1) - I_2(R_2) - I_1(r_w) + E_1 = 0$$

$$-20I_1 - 10I_2 - 1I_1 + 4.5 = 0$$

$$-21I_1 - 10I_2 = -4.5 \implies 21I_1 + 10I_2 = 4.5 \quad \text{(Equation 2)}$$

#### **Loop 2: Right Loop (Counter-Clockwise)**

Starting from the bottom-right corner and moving counter-clockwise:


$$-I_3(r_w) + E_2 - I_2(R_2) = 0$$

$$-1I_3 + 9 - 10I_2 = 0 \quad \text{(Equation 3)}$$

---

### **3. Solve the System of Equations**

Substitute **Equation 1** ($I_3 = I_2 - I_1$) into **Equation 3**:


$$-(I_2 - I_1) + 9 - 10I_2 = 0$$

$$-I_2 + I_1 + 9 - 10I_2 = 0$$

$$I_1 - 11I_2 = -9 \implies I_1 = 11I_2 - 9 \quad \text{(Equation 4)}$$

Now, substitute **Equation 4** into **Equation 2**:


$$21(11I_2 - 9) + 10I_2 = 4.5$$

$$231I_2 - 189 + 10I_2 = 4.5$$

$$241I_2 = 193.5$$

$$I_2 = \frac{193.5}{241} \approx \mathbf{0.803\,\text{A}}$$

Using $I_2$ to find $I_1$:


$$I_1 = 11(0.803) - 9 \approx \mathbf{-0.167\,\text{A}}$$


*(The negative sign means the actual current $I_1$ flows in the opposite direction of our initial clockwise assumption.)*

Finally, find $I_3$:


$$I_3 = I_2 - I_1 = 0.803 - (-0.167) = \mathbf{0.970\,\text{A}}$$

---

### **Final Results**

* **$I_1$ (Left Branch):** $-0.167\,\text{A}$
* **$I_2$ (Center Branch):** $0.803\,\text{A}$
* **$I_3$ (Right Branch):** $0.970\,\text{A}$
