# LoRA

## LoRA 公式

**原始层：**
$$
h = W_0 x
$$

**LoRA 层：**
$$
h = W_0 x + \frac{\alpha}{r} \cdot B A x
$$

- $W_0$：预训练权重，冻结
- $A \in \mathbb{R}^{r \times k}$，$B \in \mathbb{R}^{d \times r}$：低秩矩阵，可训练
- $r \ll \min(d, k)$：秩，远小于原始维度
- $\alpha$：缩放因子
- 初始化：$A$ 随机高斯，$B = 0$，开始时 $\Delta W = 0$

**核心思想：**
$$
\Delta W = B A
$$
用两个小矩阵的乘积代替一个大矩阵的更新。