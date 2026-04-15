To determine if a function represents a traveling wave, it must satisfy the linear wave equation:



$$\frac{\partial^2 y}{\partial x^2} = \frac{1}{v^2} \frac{\partial^2 y}{\partial t^2}$$



A general solution to this equation is any function of the form $y(x,t) = f(x \pm vt)$. 



---

### Analysis of the Functions



#### a) $y(x,t) = A\cos(kx^2 - \omega t)$


* **Form:** This does not fit the $f(x \pm vt)$ form because $x$ is squared ($x^2$).

* **Test:** If you take the second derivative with respect to $x$, you will get terms involving $x$, whereas the second derivative with respect to $t$ will not. They will not be proportional by a constant $1/v^2$.
*
* * **Verdict:** **No**, it is not a traveling wave.

#### b) $y(x,t) = A(x - vt)^2$


* **Form:** This perfectly fits the form $f(x - vt)$, where $u = (x - vt)$.
  
* **Test:** * $\frac{\partial^2 y}{\partial x^2} = 2A$
  
    * $\frac{\partial^2 y}{\partial t^2} = A(-v)^2(2) = 2Av^2$
      
    * Plugging into the wave equation: $2A = \frac{1}{v^2}(2Av^2) \implies 2A = 2A$.
      
* **Verdict:** **Yes**, it satisfies the wave equation.

#### c) $y(x,t) = A\log(x + vt)$


* **Form:** This fits the form $f(x + vt)$, representing a wave traveling in the negative $x$-direction.
  
* **Test:**
    * $\frac{\partial^2 y}{\partial x^2} = -\frac{A}{(x+vt)^2}$
      
    * $\frac{\partial^2 y}{\partial t^2} = -\frac{Av^2}{(x+vt)^2}$
      
    * Plugging into the wave equation: $-\frac{A}{(x+vt)^2} = \frac{1}{v^2} \left(-\frac{Av^2}{(x+vt)^2}\right)$.
      
* **Verdict:** **Yes**, it satisfies the wave equation (though physically, it is only valid where $x + vt > 0$).
  

---

### Final Summary


The functions that can describe a traveling wave are:

* **b) $y(x,t) = A(x - vt)^2$**
  
* **c) $y(x,t) = A\log(x + vt)$**
  

**Note:** Function **(a)** fails because the spatial part $kx^2$ prevents the wave from maintaining its shape as it translates through time.
