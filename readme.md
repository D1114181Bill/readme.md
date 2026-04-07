### **LMS 演算法步驟**

**Initialisation:**
$$\mathbf{\hat{h}}(0) = \text{zeros}(p)$$

**Computation:** 針對 $n = 0, 1, 2, \dots$ 

1.  **輸入向量 (Input Vector):**
    $$\mathbf{x}(n) = [x(n), x(n-1), \dots, x(n-p+1)]^T$$

2.  **誤差訊號 (Error Signal):**
    $$e(n) = d(n) - \mathbf{\hat{h}}^H(n)\mathbf{x}(n)$$

3.  **權重更新 (Tap-Weight Adaptation):**
    $$\mathbf{\hat{h}}(n+1) = \mathbf{\hat{h}}(n) + \mu e^*(n)\mathbf{x}(n)$$

---
