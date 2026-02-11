---
sidebar_position: 2
---

# Phép thử lặp (Phép thử Bernoulli) và Công thức Bernoulli

## Phép thử lặp
Xét một phép thử $\mathcal{C}$ và một biến cố $A$ liên quan tới phép thử đó. Xác suất xuất hiện $A$ là $p$. Ta thực hiện phép thử $\mathcal{C}$ $n$ lần một cách độc lập. Bài toán đặt ra là hãy tính xác suất để trong $n$ phép thử lặp này biến cố $A$ xuất hiện đúng $k$ lần, ở đó $k$ là một số tự nhiên cho trước, $0 \le k \le n$.

Ký hiệu $H_k$ là biến cố: *"$A$ xảy ra đúng $k$ lần trong $n$ phép thử $\mathcal{C}$"*. <br />
Ta hãy xét một số trường hợp đặc biệt.

1. Với $k = n$: $H_n = \underbrace{A \; A \; \dots \; A}_{n \text{ lần}}$
    - Do đó: $P(H_n) = P(A \; A \; \dots \; A) = \left[ P(A) \right]^n = p^n$.

2. Với $k = 0$: $H_0 = \underbrace{\overline{A} \; \overline{A} \; \dots \; \overline{A}}_{n \text{ lần}}$
    - Do đó: $P(H_0) = P(\overline{A} \; \overline{A} \; \dots \; \overline{A}) = \left[ P(\overline{A}) \right]^n = (1 - p)^n$.

3. Với $k = 1$: $H_1 = \underbrace{\underbrace{A \; \overline{A} \; \dots \; \overline{A}}_{n \text{ biến cố}} \cup \underbrace{\overline{A} \; A \; \dots \; \overline{A}}_{n \text{ biến cố}} \cup \dots \cup \underbrace{\overline{A} \; \overline{A} \; \dots \; A}_{n \text{ biến cố}}}_{n \text{ lần}}$
    - Do đó: $P(H_1) = \underbrace{P(A) \cdot \left[ P(\overline{A}) \right]^{n - 1} + \dots + \left[ P(\overline{A}) \right]^{n - 1} \cdot P(A)}_{n \text{ lần}} = \underbrace{p(1 - p)^{n - 1} + \dots + (1 - p)^{n - 1}p}_{n \text{ lần}}$.
    - Kết luận: $P(H_1) = np(1 - p)^{n - 1}$.

Một cách tổng quát biến cố $H_k$ là hợp của các biến cố có dạng $A \; A \; \overline{A} \; \overline{A} \dots A$ $(*)$ trong đó chữ cái $A$ xuất hiện $k$ lần, còn chữ cái $\overline{A}$ xuất hiện $n - k$ lần. Do tính độc lập của các phép thử lặp, mỗi biến cố dạng như vậy có xác suất là:
$$
P(A) \cdot P(A) \cdot P(\overline{A}) \dots P(\overline{A}) \dots P(A) = p^k(1 - p)^{n - k}
$$

Dễ thấy $H_k$ là hợp của $C^k_n$ biến cố dạng $(*)$. Thành thử:
$$
P(H_k) = C^k_n p^k (1 - p)^{n - k}
$$

Vậy ta có công thức Bernoulli.

## Công thức Bernoulli

### Định lý (Công thức Bernoulli)
Ký hiệu: $P_k(n; p)$ là xác suất để trong một dãy $n$ phép thử độc lập biến cố $A$ xuất hiện đúng $k$ lần:
$$
P_k(n; p) = C^k_n p^k q^{n - k}
$$
ở đó $p = P(A)$, $q = P(\overline{A}) = 1 - p$.