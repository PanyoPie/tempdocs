---
sidebar_position: 3
---

# Xác suất có điều kiện và Quy tắc nhân tổng quát

## Xác suất có điều kiện

### Định nghĩa
Giả sử $A$ là một biến cố, $B$ là một biến cố khác. Xác suất của $B$ được tính trong điều kiện biết rằng $A$ đã xảy ra được gọi là *"xác suất của $B$ với điều kiện $A$"* và được ký hiệu $P(B | A)$.

### Công thức
Cho $A$ và $B$ là hai biến cố bất kỳ, trong đó $P(A) \ne 0$. Khi đó xác suất có điều kiện $P(B | A)$ được tính theo công thức sau:
$$
P(B | A) = \frac{P(AB)}{P(A)}
$$

### Chú ý
1. Nếu $P(A) = 0$ thì xác suất có điều kiện $P(B | A)$ vẫn tồn tại nhưng ta không áp dụng công thức trên được.
2. Xác suất có điều kiện $P(B | A)$ có thể tính trực tiếp từ bối cảnh bài toán mà không cần thông qua công thức trên.

## Quy tắc nhân tổng quát

### Công thức
Với $A$ và $B$ là hai biến cố bất kỳ, ta có:
$$
P(AB) = P(A) \cdot P(B | A)
$$

### Tổng quát
Một cách tổng quát: Với $n$ biến cố bất kỳ $A_1, A_2, \dots, A_n$ ta có:
$$
P(A_1 A_2 \dots A_n) = P(A_1) \cdot P(A_2 | A_1) \cdot P(A_3 | A_1 A_2) \dots P(A_n | A_1 A_2 \dots A_{n - 1})
$$