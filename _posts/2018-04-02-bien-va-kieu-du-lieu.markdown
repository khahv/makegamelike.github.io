---
layout: xxx
title:  "Biến và kiểu dữ liệu"
sub-title: "Bài 3"
body: "alu"
date:   2018-04-02 01:11:45 -0800
categories: basic cplusplus
---
<!--{% include mycomponent.html %}-->


Khi khai báo một biến trong C++, chúng ta phải khai báo kiểu dữ liệu của biến đó.
Ví dụ:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable;
  return 0;
}
{% endhighlight %}

Ở ví dụ trên `myVariable` là tên của biến cần khai báo, mỗi biến cần có một cái tên để ta phân biệt chúng. `int` chính là kiểu dữ liệu của biến đó, là viết tắt của integer tức số nguyên. Điều này có nghĩa là biến `myVariable` của chúng ta thuộc kiểu [số nguyên](https://vi.wikipedia.org/wiki/S%E1%BB%91_nguy%C3%AAn) (-1, 0, 1, 2...). Tức là `myVariable` là một số nguyên, chúng ta gọi nó là "biến", vì nó có thể thay đổi giá trị.

Thay đổi giá trị trong C++ gọi là phép gán. Ta gán một biến trong C++ bằng toán tử "=". 
Ví dụ:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable = 1;
  return 0;
}
{% endhighlight %}

Ở ví dụ trên, ta gán `myVariable` = 1, như vậy `myVariable` sẽ có giá trị bằng số nguyên 1.

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable = 1;
  myVariable = 2;
  myVariable = 3;
  return 0;
}
{% endhighlight %}

Sau đó ta cũng có thể gán lại giá trị của `myVariable` bằng một giá trị khác (2, 3). Như vậy `myVariable` có thể thay đổi được giá trị bằng phép gán sử dụng dấu "=".

Dưới đây là danh sách một số kiểu dữ liệu trong C++:

`int`: integer là kiểu số nguyên. Ví dụ: -1, -2, 0, 1.

`float`: là kiểu số thực. Ví dụ: 1.0, 2.5, 3.222

`bool`: là kiểu đúng hoặc sai. Ví dụ: true, false

`char`: kiểu ký tự. Ví dụ: 'a', 'b','@', ' '

Ở bài sau chúng ta sẽ cùng tìm hiểu một số toán tử cơ bản trong C++.

Học C++ thật dễ dàng đúng không các bạn!


