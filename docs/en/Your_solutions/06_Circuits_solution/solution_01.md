To find the equivalent resistance and the total current for these circuits, we apply the fundamental rules for series and parallel resistor networks.

---

## **Case 1: Series Connection**

In a series circuit, the current has only one path to follow. Therefore, the total resistance is simply the sum of all individual resistances.

### **1. Equivalent Resistance ($R_{eq}$)**

The formula for resistors in series is:


$$R_{eq} = R_1 + R_2 + R_3$$

Substituting the given values:


$$R_{eq} = 15\,\Omega + 30\,\Omega + 50\,\Omega = \mathbf{95\,\Omega}$$

### **2. Total Current ($I$)**

Using Ohm’s Law ($V = I \cdot R$), we can find the current flowing from the battery:


$$I = \frac{V}{R_{eq}}$$

$$I = \frac{12\,\text{V}}{95\,\Omega} \approx \mathbf{0.126\,\text{A (or 126 mA)}}$$

---

## **Case 2: Parallel Connection**

In a parallel circuit, the voltage across each resistor is the same, but the current splits into multiple branches. The total resistance decreases as more paths are added.

### **1. Equivalent Resistance ($R_{eq}$)**

The formula for the reciprocal of the equivalent resistance is:


$$\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$$

Plugging in the values:


$$\frac{1}{R_{eq}} = \frac{1}{15} + \frac{1}{30} + \frac{1}{50}$$

To solve, find a common denominator (150):


$$\frac{1}{R_{eq}} = \frac{10}{150} + \frac{5}{150} + \frac{3}{150} = \frac{18}{150}$$

Now, take the reciprocal to find $R_{eq}$:


$$R_{eq} = \frac{150}{18} \approx \mathbf{8.33\,\Omega}$$

### **2. Total Current ($I$)**

Using Ohm's Law again with the new equivalent resistance:


$$I = \frac{12\,\text{V}}{8.33\,\Omega} \approx \mathbf{1.44\,\text{A}}$$

---
