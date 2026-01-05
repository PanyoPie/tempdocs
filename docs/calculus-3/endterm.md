---
sidebar_position: 2
---

# Một số thứ liên quan đến bài thi cuối kỳ

## Câu 1. Phát biểu nội dung định lý Fubini
Giả sử $A \subset \mathbb{R}^n$ và $B \subset \mathbb{R}^m$ là các hình hộp đóng và $f: A \times B \to \mathbb{R}$ là hàm khả tích. Hơn nữa giả sử rằng hàm $g_x : B \to \mathbb{R}$ xác định đối với mỗi $x \in A$ bởi đẳng thức:
$$
g_x(y) = f(x, y)
$$

$$
I_*(x) = \int_{*B} g_x \, \text{d}y =  \int_{*B} f(x, y) \, \text{d}y
$$

$$
I^*(x) = \int^*_B g_x \, \text{d}y =  \int^*_B f(x, y) \, \text{d}y
$$

Khi đó: $I_*$ và $I^*$ khả tích trên $A$ và:
$$
\int_{A \times B} f \, \text{d}V = \int_A I_* \, \text{d}x = \int_A \left( \int_{*B} f(x, y) \, \text{d}y \right) \text{d}x
$$

$$
\int_{A \times B} f \, \text{d}V = \int_A I^* \, \text{d}x = \int_A \left( \int^*_B f(x, y) \, \text{d}y \right) \text{d}x
$$

## Câu 2. Phát biểu nội dung định lý Green
Giả sử D là miền bị chặn, đơn liên trong mặt phẳng $Oxy$ được giới hạn bởi chu tuyến $C$ đóng, trơn từng khúc, không bị cắt. Chu tuyến $C$ được định hướng dương theo ngược hướng chiều kim đồng hồ. Như vậy khi đi theo hướng đó thì miền $D$ luôn luôn ở về phía bên trái.

Giả sử $P(x, y)$ và $Q(x, y)$ là các hàm xác định và liên tục cùng với các đạo hàm riêng $\displaystyle \frac{\partial Q}{\partial x}(x, y)$, $\displaystyle \frac{\partial P}{\partial y}(x, y)$ liên tục trong miền đóng $\overline{D} = D \cup C$.

Khi đó ta có công thức Green:
$$
\oint_{C^+} P(x, y) \, \text{d}x + Q(x, y) \, \text{d}y = \iint_D \left[ \frac{\partial Q}{\partial x}(x, y) - \frac{\partial P}{\partial y}(x, y) \right] \, \text{d}x \, \text{d}y
$$

## Câu 3. Phát biểu nội dung định lý (Gauss-)Ostrogradsky
:::success[Định lý này cũng được biết đến với các tên]
1. Định lý Gauss
2. Định lý Ostrogradsky
3. Định lý phân kỳ
4. Định lý Gauss-Ostrogradsky
5. Định lý Ostrogradsky-Gauss
:::

Giả sử $\Omega$ là miền bị chặn trong không gian $\mathbb{R}^3$ với biên $S$ trơn hoặc trơn từng mảnh.

$P(x, y, z)$, $Q(x, y, z)$ và $R(x, y, z)$ là các hàm khả vi liên tục trong $\overline{\Omega} = \Omega \cup S$.

Khi đó ta có công thức Gauss-Ostrogradsky:
$$
\iint_{S^+} P(x, y, z) \, \text{d}y \, \text{d}z + Q(x, y, z) \, \text{d}z \, \text{d}x + R(x, y, z) \, \text{d}x \, \text{d}y = \iiint_{\Omega} \left[ \frac{\partial P}{\partial x}(x, y, z) + \frac{\partial Q}{\partial y}(x, y, z) + \frac{\partial R}{\partial z}(x, y, z) \right] \, \text{d}x \, \text{d}y \, \text{d}z
$$

với $S^+$ là biên của $\Omega$ được định hướng dương theo pháp tuyến ngoài.