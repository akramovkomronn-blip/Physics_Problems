To solve for the equivalent resistance between two opposite corners of a cube made of 12 identical resistors ($R$), we can use the principle of **symmetry** and **Kirchhoff’s Laws**.

### **1. Applying Symmetry**

Imagine a current $I$ entering at one corner (let's call it Point A) and leaving at the opposite corner (Point B). Because all 12 resistors are identical, the current will split evenly whenever it encounters a symmetrical path.

* **At the Input (Point A):** The current $I$ meets 3 identical resistors. Due to symmetry, the current splits equally into $I/3$ for each branch.
* **The Middle Section:** After passing through the first set of resistors, each of those 3 currents reaches a new junction. At each of these 3 junctions, the current splits again into 2 paths. This means there are 6 resistors in the middle section, each carrying a current of $I/6$.
* **At the Output (Point B):** Finally, these currents converge back into 3 resistors before reaching Point B. Each of these 3 resistors carries $I/3$, combining to form the total exit current $I$.

---

### **2. Calculating Total Voltage Drop ($V_{total}$)**

To find the equivalent resistance ($R_{eq}$), we calculate the total voltage drop from Point A to Point B along any single path:

1. **First Resistor:** Current is $I/3$. Voltage drop = $\frac{I}{3}R$
2. **Second Resistor:** Current is $I/6$. Voltage drop = $\frac{I}{6}R$
3. **Third Resistor:** Current is $I/3$. Voltage drop = $\frac{I}{3}R$

Summing these individual drops gives the total voltage $V$:


$$V = \frac{I}{3}R + \frac{I}{6}R + \frac{I}{3}R$$

To add these, we use a common denominator of 6:


$$V = \left(\frac{2}{6} + \frac{1}{6} + \frac{2}{6}\right) IR = \frac{5}{6} IR$$

---

### **3. Final Equivalent Resistance**

Using Ohm’s Law ($R_{eq} = V / I$):


$$R_{eq} = \frac{\frac{5}{6} IR}{I}$$

$$R_{eq} = \mathbf{\frac{5}{6} R}$$

### **Summary of Results**

For a cube of 12 identical resistors, the equivalent resistance between the most distant (opposite) corners is **$\frac{5}{6} R$**.

Interestingly, if you were to measure between different points, the values change:

* Between adjacent corners: $\frac{7}{12} R$
* Between face-diagonal corners: $\frac{3}{4} R$
