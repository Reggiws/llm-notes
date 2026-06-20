# Adam 与 AdamW

## 指数加权平均与修正
![[Pasted image 20260601143706.png]]
## SGD
![[Pasted image 20260601143852.png]]
## Momentum
![[Pasted image 20260601143918.png]]
## RMSProp
![[Pasted image 20260601144023.png]]
## Adam:RMS Prop+Momentum
![[Pasted image 20260601145344.png]]
## AdamW
![[Pasted image 20260601145447.png]]
每个参数都要额外保存两个值。
每个值都需要用float32位来存储。
如果参数用float16存储，这两个值占用大小将是参数大小的4倍。[[显存计算]]