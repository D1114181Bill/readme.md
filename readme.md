### **LMS 演算法步驟**

**Initialisation:**
$$\mathbf{\hat{h}}(0) = \text{zeros}(p)$$

**Computation:**  $n = 0, 1, 2, \dots$ 

    $$\mathbf{x}(n) = [x(n), x(n-1), \dots, x(n-p+1)]^T$$

    $$e(n) = d(n) - \mathbf{\hat{h}}^H(n)\mathbf{x}(n)$$

    $$\mathbf{\hat{h}}(n+1) = \mathbf{\hat{h}}(n) + \mu e^*(n)\mathbf{x}(n)$$

---
