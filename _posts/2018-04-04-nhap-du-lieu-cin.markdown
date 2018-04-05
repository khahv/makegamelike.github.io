---
layout: xxx
title:  "Nhập dữ liệu cin"
short-title: "C++ cin"
sub-title: "Bài 10"
body: "alu"
date:   2018-04-04 20:11:45 -0800
categories: basic cplusplus
---
<!--{% include mycomponent.html %}-->

Nếu muốn nhận dữ liệu nhập từ bàn phím của người dùng, ta dùng hàm `cin>>`. Cùng xem chương trình mẫu dưới đây:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int number = 0;
  cout<<"Nhap vao mot so: ";
  cin>>number;
  cout<<"So vua nhap: "<< number; 
  return 0;
}
{% endhighlight %}

Ta cũng có thể nhập một lúc nhiều số bằng `cin`:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int numberA = 0;
  int numberB = 0;
  cout<<"Nhap vao hai so: ";
  cin>>numberA>>numberB;
  cout<<"Ban vua nhap so: "<< numberA << " va " << numberB;
  return 0;
}
{% endhighlight %}


Thêm một bài ví dụ kết hợp câu lệnh if/else và cin, cout:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int numberA = 0;
  int numberB = 0;

  cout<<"Nhap 2 so A, B ";
  cin>>numberA>>numberB;
  if (numberA > numberB)
  {
    cout<<"So A lon hon so B";
  }else if (numberA == numberB)
  {
    cout<<"So A va B bang nhau";
  }
  else
  {
    cout<<"So B lon hon so A"
  }
  return 0;
}
{% endhighlight %}


