We’ll use the electric field of point charges from Coulomb's law:

$[
\vec E = k , q , \frac{\vec r}{r^3}, \quad k=\frac{1}{4\pi\varepsilon_0}
]$

Two charges:

* $(+q) at ((-a,0))$
* $(+2q) at ((a,0))4

---

# 1. General field ( \vec E(x,y) )

Position vectors from charges to point ((x,y)):

$[
\vec r_1 = (x+a,, y), \quad r_1 = \sqrt{(x+a)^2 + y^2}
]$
$[
\vec r_2 = (x-a,, y), \quad r_2 = \sqrt{(x-a)^2 + y^2}
]$

Total field:

$[
\vec E(x,y) =
k q \frac{(x+a,,y)}{r_1^3}

* k (2q) \frac{(x-a,,y)}{r_2^3}
  ]$

So components:

$[
E_x = kq\left(\frac{x+a}{r_1^3} + 2\frac{x-a}{r_2^3}\right)
]$
$[
E_y = kq\left(\frac{y}{r_1^3} + 2\frac{y}{r_2^3}\right)
]$

---

# 2. Field on the **y-axis**: $( (0,y) )$

Here:
$[
r_1 = r_2 = \sqrt{a^2 + y^2}
]$

$[
E_x = kq\left(\frac{a}{r^3} - 2\frac{a}{r^3}\right)
= -\frac{kqa}{(a^2+y^2)^{3/2}}
]$

$[
E_y = kq\left(\frac{y}{r^3} + 2\frac{y}{r^3}\right)
= \frac{3kqy}{(a^2+y^2)^{3/2}}
]$

$[
\boxed{
\vec E(0,y) =
\left(-\frac{kqa}{(a^2+y^2)^{3/2}},;
\frac{3kqy}{(a^2+y^2)^{3/2}}\right)
}
]$

---

# 3. Field on the **x-axis**: $( (x,0) )$

$[
E_y = 0
]$

$[
E_x = kq\left(\frac{x+a}{|x+a|^3} + 2\frac{x-a}{|x-a|^3}\right)
]$

(Sign depends on position relative to charges.)

---

# 4. Conditions for zero components

### (i) $(E_y = 0)$

From:
$[
E_y = kq,y\left(\frac{1}{r_1^3} + \frac{2}{r_2^3}\right)
]$

So:
$[
\boxed{y = 0}
]$

---

### (ii) $(E_x = 0) (on x-axis)$

Solve:
$[
\frac{x+a}{|x+a|^3} + 2\frac{x-a}{|x-a|^3} = 0
]$

This gives a point **between the charges**, closer to the smaller charge (q).

---

### (iii) Total field $( \vec E = 0 )$

Requires both components zero → only possible on **x-axis**, at the solution of (E_x=0).

---

# 5. Numerical calculation at $( (0,y) )$

Given:

* $(a = 0.2 , \text{m})$
* $(y = 0.3 , \text{m})$
* $(q = 2 ,\mu\text{C} = 2\times10^{-6} , \text{C})$
* $(k = 9\times10^9)$

Compute:

$[
r = \sqrt{0.2^2 + 0.3^2} = \sqrt{0.13} \approx 0.361
]$
$[
r^3 \approx 0.047
]$

### (E_x):

$[
E_x = -\frac{(9\times10^9)(2\times10^{-6})(0.2)}{0.047}
\approx -7.7 \times 10^4 , \text{N/C}
]$

### (E_y):

$[
E_y = \frac{3(9\times10^9)(2\times10^{-6})(0.3)}{0.047}
\approx 3.45 \times 10^5 , \text{N/C}
]$

---

### ✅ Final numerical result:

$[
\boxed{
\vec E(0,0.3) \approx (-7.7\times10^4,; 3.45\times10^5)\ \text{N/C}
}
]$

---

# 6. Limit ( y \gg a )

Then:
$[
r_1 \approx r_2 \approx y
]$

$[
E_x \approx -\frac{kqa}{y^3} \to 0
]$

$[
E_y \approx \frac{3kqy}{y^3} = \frac{3kq}{y^2}
]$

---

### Interpretation

At large distances, the system behaves like a **single charge (3q)** located near the origin:

$[
\boxed{
\vec E \approx \frac{3kq}{y^2} ,\hat{y}
}
]$


