# Attention

$$
 \text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V
$$
## MHA
$$
\text{MultiHead}(Q, K, V) = \text{Concat}(\text{head}_1, \ldots, \text{head}_h) W^O
\text{head}_i = \text{Attention}(Q W_i^Q, K W_i^K, V W_i^V)
$$
参数
hidden_dim, num_heads, max_seq_len, dropout=0.1