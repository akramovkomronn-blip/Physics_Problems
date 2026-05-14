When you have three identical $1\,\Omega$ resistors, you can arrange them in four distinct configurations. Each setup provides a unique equivalent resistance ($R_{eq}$) based on how the current is divided or channeled.

### **1. All Three in Series**

In this configuration, the resistors are connected end-to-end. The total resistance is the sum of the individual parts.

* **Formula:** $R_{eq} = R_1 + R_2 + R_3$
* **Calculation:** $1 + 1 + 1 = \mathbf{3\,\Omega}$

### **2. All Three in Parallel**

Here, the resistors are connected across the same two nodes, creating three separate paths for the current.

* **Formula:** $\frac{1}{R_{eq}} = \frac{1}{R_1} + \frac{1}{R_2} + \frac{1}{R_3}$
* **Calculation:** $\frac{1}{R_{eq}} = 1 + 1 + 1 = 3 \implies R_{eq} = \mathbf{0.33\,\Omega}$ (or $1/3\,\Omega$)

### **3. Two in Parallel, One in Series**

Two resistors are branched together, and that entire unit is connected in series with the third resistor.

* **Step 1 (Parallel branch):** $R_p = \frac{1 \times 1}{1 + 1} = 0.5\,\Omega$
* **Step 2 (Total):** $R_{eq} = 0.5 + 1 = \mathbf{1.5\,\Omega}$ (or $3/2\,\Omega$)

### **4. Two in Series, One in Parallel**

Two resistors are connected end-to-end to form a $2\,\Omega$ branch, which is then placed in parallel with the single $1\,\Omega$ resistor.

* **Step 1 (Series branch):** $R_s = 1 + 1 = 2\,\Omega$
* **Step 2 (Total):** $R_{eq} = \frac{2 \times 1}{2 + 1} = \mathbf{0.67\,\Omega}$ (or $2/3\,\Omega$)

---

### **Summary of Unique Values**

There are **four** unique equivalent resistances possible:

1. **$0.33\,\Omega$** (All parallel)
2. **$0.67\,\Omega$** (Parallel pair of [series pair + single])
3. **$1.5\,\Omega$** (Series pair of [parallel pair + single])
4. **$3\,\Omega$** (All series)
