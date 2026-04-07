### **LMS 演算法步驟**

**Initialisation:**
$$\mathbf{\hat{h}}(0) = \text{zeros}(p)$$

**Computation:** For $(n) = 0, 1, 2, \dots$ 進行以下疊代：

1.  **輸入向量 (Input Vector):**
    $$\mathbf{x}(n) = [x(n), x(n-1), \dots, x(n-p+1)]^T$$

2.  **誤差訊號 (Error Signal):**
    $$e(n) = d(n) - \mathbf{\hat{h}}^H(n)\mathbf{x}(n)$$

3.  **權重更新 (Tap-Weight Adaptation):**
    $$\mathbf{\hat{h}}(n+1) = \mathbf{\hat{h}}(n) + \mu e^*(n)\mathbf{x}(n)$$

---

**符號說明：**
* $\mathbf{\hat{h}}(n)$：濾波器係數向量（估計值）。
* $\mathbf{x}(n)$：輸入訊號向量。
* $d(n)$：期望響應（Desired response）。
* $e(n)$：估計誤差。
* $\mu$：步長因子（Step-size parameter）。
* $H$：共軛轉置（Hermitian transpose）。
* $*$：共軛複數（Complex conjugate）。
