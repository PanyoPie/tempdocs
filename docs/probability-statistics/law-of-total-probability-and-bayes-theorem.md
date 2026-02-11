---
sidebar_position: 4
---

# Công thức xác suất đầy đủ và Công thức Bayes

## Công thức xác suất đầy đủ

### Hệ đầy đủ các biến cố
Các biến cố $B_1, B_2, \dots, B_n$ được gọi là một *hệ đầy đủ các biến cố* nếu chúng đôi một xung khắc với nhau ($B_i B_j = \varnothing$ nếu $i \ne j$) và hợp của chúng là biến cố chắc chắn:
$$
\Omega = B_1 \cup B_2 \cup \dots \cup B_n
$$

Ta có công thức sau đây, được gọi là *công thức xác suất đầy đủ*. Công thức này có rất nhiều ứng dụng khi giải toán.

### Định lý
**Định lý:** *Nếu $B_1, B_2, \dots, B_n$ là một hệ đầy đủ thì với mỗi biến cố $A$, ta có:*
$$
P(A) = \sum_{i = 1}^n P(B_i) \cdot P(A | B_i)
$$ 

## Công thức Bayes

### Công thức tổng quát
Nếu $B_1, B_2, \dots, B_n$ là một hệ đầy đủ các biến cố và $A$ là một biến cố với $P(A) > 0$ thì với mỗi $k = 1, 2, \dots, n$:
$$
P(B_k | A) = \dfrac{P(B_k) \cdot P(A | B_k)}{\displaystyle \sum_{i = 1}^n P(B_i) \cdot P(A | B_i)}
$$

### Chứng minh
Theo quy tắc nhân:
- $P(A) \cdot P(B_k | A) = P(A B_k)$
- $P(B_k) \cdot P(A | B_k) = P(A B_k)$

Như vậy: $P(A) \cdot P(B_k | A)$ = $P(B_k) \cdot P(A | B_k) \Rightarrow P(B_k | A) = \dfrac{P(B_k) \cdot P(A | B_k)}{P(A)}$.

Mặt khác: $P(A) = \displaystyle \sum_{i = 1}^n P(B_i) \cdot P(A | B_i)$.

Thay vào mẫu số, ta có điều phải chứng minh:
$$
P(B_k | A) = \dfrac{P(B_k) \cdot P(A | B_k)}{\displaystyle \sum_{i = 1}^n P(B_i) \cdot P(A | B_i)}
$$