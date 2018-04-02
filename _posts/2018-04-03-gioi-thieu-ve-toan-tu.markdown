---
layout: xxx
title:  "Giới thiệu về toán tử"
body: "alu"
date:   2018-04-02 01:11:45 -0800
categories: basic cplusplus
---
<!--{% include mycomponent.html %}-->

Ở phần trước ta đã tìm hiểu cách khai báo một biến với kiểu dữ liệu trong C++, ở phần này ta sẽ sử dụng biến đó để tính toán các phép tính đơn giản.

Ví dụ nếu ta muốn tính bài toán 2*5+10 xem kết quả bằng bao nhiêu. Ta có thể gõ như sau:
Ví dụ:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable = 2*5+10;
  return 0;
}
{% endhighlight %}

Ở ví dụ trên biến `myVariable` được khai bao theo kiểu số nguyên, đồng thời được gán giá trị = 2*5+10. Như vậy phép tính 2*5+10 sẽ được C++ xử lý và cho ra kết quả 20, kết quả này được gán vào biến `myVariable`. Tất cả điều này diễn ra trước khi kết thúc dòng lệnh trên. Mỗi dòng lệnh được đánh dấu bằng dấu ";". Như vậy `myVariable` sẽ có kết quả là số nguyên 20.

Giả sử các bạn muốn cộng 2 biến với nhau thì sẽ làm như sau:
{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable = 2*5+10;
  int mySecondVariable = myVariable * 2;
  return 0;
}
{% endhighlight %}

Như giải thích ở trên ta đã biết sau khi kết thúc dòng lệnh tính toán đầu tiên, ta có kết quả 20 được gán vào biến `myVariable`. Ở dòng lệnh tiếp theo ta nhân `myVariable` với 2. Như vậy tương đương với 20 * 2 = 40. Kết quả 40 được gán vào biến `mySecondVariable`.

Một số toán tử trong C++:

`+`: phép cộng 2 số.

`-`: phép trừ 2 số.

`*`: phép nhân 2 số.

`/`: phép chia 2 số.

`(`: dấu mở ngoặc, có tác dụng gộp ưu tiên phép toán bên trong.

`)`: dấu đóng ngoặc, có tác dụng gộp ưu tiên.

`%`: phép chia lấy phần dư.

Lưu ý các phép toán trên toán tử đều được áp dụng quy luật ưu tiên theo toán học. Ví dụ như nhân chia trước, cộng trừ sau. Xem thêm ở link sau nếu các bạn quên:
[Độ ưu tiên toán tử](https://vi.wikipedia.org/wiki/%C4%90%E1%BB%99_%C6%B0u_ti%C3%AAn_c%E1%BB%A7a_to%C3%A1n_t%E1%BB%AD)
Nếu các bạn chưa hiểu rõ những toán tử trên thì cũng đừng lo, chúng ta sẽ tìm hiểu dần dần qua các bài sau.

Như vậy qua bài này ta đã biết cách tính toán dùng các toán tử trong C++.