---
layout: xxx
title:  "Một số toán tử đặc biệt trong C++"
body: "alu"
date:   2018-04-02 01:11:45 -0800
categories: basic cplusplus
---
<!--{% include mycomponent.html %}-->

Phần này sẽ giới thiệu một số toán tử mà trong toán học bình thường không có.

Toán tử cộng: ++

Toán tử này dùng để tăng giá trị của một biến lên 1 đơn vị. Tuy nhiên nó có 2 cách ghi như sau:
`myVariable++` và `++myVariable`. Trong đó `myVariable` là tên biến.

Sự khác nhau ở chỗ `myVariable++` sẽ tăng giá trị của `myVariable` lên sau khi đã thực hiện các toán tử khác trong cùng dòng lệnh. Trong khi đó `++myVariable` sẽ tăng giá trị của `myVariable` lên trước, rồi sau đó mới thực hiện các phép toán khác trên cùng dòng lệnh.

Chúng ta cùng xem ví dụ sau để hiểu rõ hơn:



{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable = 0;
  myVariable++;
  return 0;
}
{% endhighlight %}

Ở đoạn mã trên, khi kết thúc dòng lệnh `myVariable++` thì giá trị của `myVariable` sẽ bằng 1. Ở đây không có sự khác biệt giữa việc dùng `myVariable++` và `++myVariable`.

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable = 0;
  int total = 0;
  total = 2*myVariable++;//Kết quả total = 0, myVariable = 1
  return 0;
}
{% endhighlight %}

`myVariable` vẫn giữ kết quả = 0, `total = 2 * myVariable` => `total = 2 * 0` => `total = 0`.
Sau khi kết thúc dòng này, `myVariable` tăng lên = 1.



{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable = 0;
  int total = 0;
  total = 2*++myVariable;//Kết quả total = 2, myVariable = 1
  return 0;
}
{% endhighlight %}

`++myVariable` được thực hiện trước làm cho `myVariable`= 1, sau đó mới thực hiện phép tính `2*myVariable` => `2*1` = `2`. Kết thúc dòng lệnh này, `myVariable` cũng có giá trị bằng 1.

Bài sau chúng ta sẽ tiếp hiểu về cách hiển thị một biến ra màn hình.


