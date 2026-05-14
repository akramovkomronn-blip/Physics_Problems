To find the total equivalent resistance ($R_{eq}$) for this circuit, we decompose the network into smaller blocks of series and parallel components. Since each individual resistor is $10\,\Omega$, we can calculate the values step-by-step.

---

## **Step 1: The Top Branch**

The top branch consists of two resistors connected in **series**.

* **Calculation:** $10\,\Omega + 10\,\Omega = \mathbf{20\,\Omega}$

## **Step 2: The Bottom Branch (Inner Parallel)**

First, look at the small parallel cluster on the right side of the bottom branch.

* **Formula:** $\frac{1}{R_p} = \frac{1}{10} + \frac{1}{10} = \frac{2}{10} \implies R_p = \mathbf{5\,\Omega}$
* This $5\,\Omega$ combination is in **series** with the single $10\,\Omega$ resistor to its left.
* **Bottom Branch Total:** $10\,\Omega + 5\,\Omega = \mathbf{15\,\Omega}$

## **Step 3: Combining the Main Branches**

Now we combine the top branch ($20\,\Omega$) and the bottom branch ($15\,\Omega$), which are in **parallel** with each other.

* **Calculation:** $R_{branches} = \frac{20 \times 15}{20 + 15} = \frac{300}{35}$
* **Result:** $\approx \mathbf{8.57\,\Omega}$

## **Step 4: The Final Series Resistor**

The entire network calculated above is in **series** with the final resistor on the far right.

* **Total $R_{eq}$:** $8.57\,\Omega + 10\,\Omega = \mathbf{18.57\,\Omega}$

---

### **Final Equivalent Resistance**

The total equivalent resistance for the circuit is approximately **$18.57\,\Omega$**.
