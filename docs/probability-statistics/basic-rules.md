---
sidebar_position: 1
---

# Các quy tắc tính xác suất

## Quy tắc cộng xác suất
Nếu $A$ và $B$ là hai biến cố xung khắc thì:
$$
P(A \cup B) = P(A) + P(B)
$$

Một cách tổng quát, cho các biến cố $A_1, A_2, \dots, A_n$ sao cho hai biến cố bất kỳ là xung khắc (nghĩa là chúng xung khắc từng đôi). Khi đó:
$$
P(A_1 \cup A_2 \cup \dots \cup A_n) = P(A_1) + P(A_2) + \dots + P(A_n)
$$

hay

$$
P \left( \bigcup_{i = 1}^n A_i \right) = \sum_{i = 1}^n P(A_i)
$$

## Quy tắc cộng xác suất tổng quát
Nếu $A$ và $B$ là hai biến cố bất kỳ (không nhất thiết xung khắc) thì:
$$
P(A \cup B) = P(A) + P(B) - P(AB)
$$

Ta có thể mở rộng công thức này cho hợp của ba biến cố:
$$
P(A \cup B \cup C) = P(A) + P(B) + P(C) - P(AB) - P(BC) - P(CA) + P(ABC)
$$

## Quy tắc chuyển sang biến cố đối
Trong nhiều bài toán việc tính xác suất của biến cố $A$ khó hơn nhiều so với việc tính xác suất của biến cố đối $\overline{A}$. Khi đó ta sẽ tính $P(\overline{A})$ rồi từ đó tìm $P(A)$ nhờ quan hệ sau:
$$
P(A) = 1 - P(\overline{A})
$$

## Quy tắc nhân

### Biến cố độc lập
- Hai biến cố $A$ và $B$ được gọi là dộc lập với nhau nếu việc xảy ra hay không xảy ra biến cố này không làm ảnh hưởng tới việc xảy ra hay không xảy ra của biến cố kia.
- Tổng quát các biến cố $A_1, A_2, \dots, A_n$ được gọi là độc lập nếu việc xảy ra hay không xảy ra của một nhóm bất kỳ $k$ biến cố trong đó $(1 \le k \le n)$ không làm ảnh hưởng tới việc xảy ra hay không xảy ra của các biến cố còn lại.

### Quy tắc
Nếu hai biến cố $A$ và $B$ độc lập thì:
$$
P(AB) = P(A) \cdot P(B)
$$

Nếu $A_1, A_2, \dots, A_n$ là độc lập thì:
$$
P(A_1 A_2 \dots A_n) = P(A_1) \cdot P(A_2) \dots P(A_n)
$$