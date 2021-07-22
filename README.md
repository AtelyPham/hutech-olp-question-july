# Trò chơi của Avenger

Cuộc thi được diễn ra tại [hackkerrank](https://www.hackerrank.com/kythilaptrinhcanhanthang72023).

## Problem Statement

Sau khi chiến thắng Thanos, các Avenger họp mặt với nhau để chúc mừng và tưởng nhớ Tony. Lúc này, một thành viên nghĩ ra một trò chơi.

![image](https://s3.amazonaws.com/hr-assets/0/1626933521-34e9909f4e-susan-holt-simpson-GQ327RPuxhI-unsplash.jpg)

Có $\textit{n}$ người còn lại trong team Avenger, người thứ $i$-th chọn một con số $a_i$. Người chiến thắng là người mà có con số là **duy nhất** (có nghĩa là không có ai chọn con số này ngoài người đó) và đồng thời là **nhỏ nhất** (trong tất cả các con số **duy nhất**, số nhỏ nhất là số chiến thắng).

Nhiệm vụ của bạn là đi tìm $\textit{i}$, **vị trí** của người chiến thắng trong $\textit{n}$ Avengers, hoặc $-1$ nếu không tồn tại người chiến thắng. **Vị trí** được đánh dấu bắt đầu từ $1$, có nghĩa là các Avenger được đánh dấu theo thứ tự $1...n$.

## Input Format

Dòng đầu tiên của input chứa một _số nguyên_ $\textit{t}\ $ ($1 \le t \le 2 \cdot 10^4$) — số lượng bộ test case. Theo sau đó là $\textit{t}\ $ test case.

Dòng đầu tiên của mỗi test case là một _số nguyên_ $\textit{n}\ \ (1 \le n \le 2 \cdot 10^5)$ - số lượng Avenger tham gia chơi. Dòng thứ hai của test case chứa $\textit{n}$ số nguyên $a_1, a_2, \ldots, a_n\ $ ($1 \le a_i \le n$), trong đó $a_i$ là số mà Avenger thứ $\textit{i}$-th chọn.

Đầu vào (input) luôn đảm bảo tổng của $n$ số $a_i$ không vượt quá $2 \cdot 10^5\ $ ($\sum\_{i = 1}^{n} a_i \le 2 \cdot 10^5$).

## Output Format

Đối với mỗi test case, in ra câu trả lời - **vị trí** của người chiến thắng trong trò chơi (hoặc $-1$ nếu không tồn tại người chiến thắng). Người chiến thắng là người có con số là **duy nhất** và **nhỏ nhất** trong tất cả các con số là **duy nhất**.

## Constraints

- $1 \le t \le 2 \cdot 10^4$.
- $1 \le n \le 2 \cdot 10^5$.
- $\sum_{i = 1}^{n} a_i \le 2 \cdot 10^5$.

# Chuỗi nhị phân đẹp

## Problem Statement

Morgan Stark, con gái của Tony Stark, từ nhỏ cô đã thích nghiên cứu về máy tính, và cô đặc biệt thích những chuỗi nhị phân đẹp.

![image](https://s3.amazonaws.com/hr-assets/0/1626933638-ec0a2c82b1-alexander-sinn-KgLtFCgfC28-unsplash.jpg)

Một **chuỗi nhị phân đẹp** là chuỗi nhị phân có độ dài **lớn hơn $1$** và là **chuỗi đối xứng**.

Chuỗi đối xứng là chuỗi mà đọc từ trái sang phải hay ngược lại phải sang trái đều giống nhau. Ví dụ: những chuỗi $1$, $010$, $1001$, $01100110$ là những chuỗi đối xứng, nhứng những chuỗi $10$, $100011$, $0001$ thì không.

Morgan định phát minh ra một sản phẩm dựa trên những chuỗi nhị phân đẹp này, những đang mắc kẹt ở việc do những chuỗi nhị phân trong máy tính quá dài, bạn hãy giúp Morgan đếm xem trong một chuỗi nhị phân dài vô hạn... có bao nhiêu chuỗi nhị phân đẹp nằm trong chuỗi đó nhé!

Bạn được cho một chuỗi $s$ có độ dài $n$, chỉ chứa kí tự $0$ và $1$.

Giúp Morgan tính xem có bao nhiêu chuỗi nhị phân con là chuỗi nhị phân đẹp nhé!

## Input Format

Dòng đầu tiên chứa một số $n$ ($1 \le n \le 3 \cdot 10^5$) - độ dài của chuỗi $s$.

Dòng thứ hai chứa chuỗi $s$, chỉ chứa kí tự $0$ và $1$.

## Output Format

In ra một số nguyên - Số lượng chuỗi con - là chuỗi nhị phân đẹp của $s$.

## Constraints

- $1 \le n \le 3 \cdot 10^5$.
- $s$ chỉ chứa $0$ và $1$.

# Trò chơi hóc búa

## Problem Statement

Natalia Romanoff rất thích Morgan Stark. Biết cô bé là một người thông minh, nên Natalia muốn thử thách cô bé bằng một trò chơi.

![image](https://s3.amazonaws.com/hr-assets/0/1626934437-59593695bc-susan-holt-simpson-H7SCRwU1aiM-unsplash.jpg)

Có $n$ hộp được đánh số từ $1$ đến $n$, Natalia sẽ giấu một con búp bê vào trong một hộp bất kì, sau $m$ lượt thử, nếu Morgan có thể đoán đúng vị trí của con búp bê, Morgan là người chiến thắng, ngược lại nếu Morgan không đoán được, Natalia là người chiến thắng.

Để làm trò chơi khó hơn, Natalia sử dụng thêm một trick, sau mỗi lần Morgan đoán không đúng vị trí, Nataliia có thể di chuyển con búp bê đến hộp bên cạnh hoặc giữ nguyên vị trí. Hộp số $i$ và $i + 1$ là hai hộp bên cạnh nhau trong tất cả $1 \leq i \leq n - 1$. Natalia cũng có thể sử dụng trick một lần này trước khi trò chơi bắt đầu.

Trò chơi diễn ra như sau: Trò chơi bắt đầu, Natalia thực hiện trick, Morgan đoán lần 1, Natalia thực hiện trick, Morgan đoán lần 2, ..., Morgan đoán lần $m$, Natalia thực hiện trick, trò chơi kết thúc.

Morgan đã nghĩ ra một chuỗi $a_1, a_2, \ldots, a_m$. Trong lần đoán thứ i, Morgan sẽ thử đoán hộp $a_i$ có chứa búp bê hay không. Morgan muốn biết số lượng ngữ cảnh ($x,\ y$) (trong tất cả $1 \leq x, y \leq n$), mà Natalia có thể thắng trò chơi, nếu cô ấy đặt con búp bê ở hộp $x$ khi trò chơi bắt đầu, và khi trò chơi kết thúc con búp bê sẽ ở hộp thứ $y$. Bạn hãy giúp Morgan tính ra con số này nhé.

## Input Format

Dòng đầu tiên chứa hai số $n$ và $m$, cách nhau bởi khoảng trắng ($1 \leq n, m \leq 10^5$) - Số lượng hộp và số lần Morgan có thể thực hiện đoán.

Dòng tiếp theo chứa $m$ số nguyên $a_1, a_2, \ldots, a_m$, cách nhau bởi khoảng trắng ($1 \leq a_i \leq n$), số $a_i$ là hộp mà Morgan đoán trong lần đoán thử thứ $i$.

## Output Format

In ra số lượng ngữ cảnh trên một dòng duy nhất, hoặc số lượng cặp số ($x,\ y$) ($1 \leq x,\ y \leq n$), mà trong đó nếu Natalia đặt con búp bê vào hộp $x$ khi trò chơi bắt, sau khi trò chơi kết thúc con búp bê nằm trong hộp $y$ và Natalia chiến thắng trò chơi.

## Constraints

Dòng đầu tiên chứa hai số $n$ và $m$, cách nhau bởi khoảng trắng ($1 \leq n, m \leq 10^5$) - Số lượng hộp và số lần Morgan có thể thực hiện đoán.

Dòng tiếp theo chứa $m$ số nguyên $a_1, a_2, \ldots, a_m$, cách nhau bởi khoảng trắng ($1 \leq a_i \leq n$), số $a_i$ là hộp mà Morgan đoán trong lần đoán thử thứ $i$.
