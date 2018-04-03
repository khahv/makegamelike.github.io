---
layout: xxx
title:  "Các hiển thị một biến ra màn hình dùng cout"
sub-title: "Bài 6"
body: "alu"
date:   2018-04-02 02:11:45 -0800
categories: basic cplusplus
---
<!--{% include mycomponent.html %}-->

Muốn hiển thị ra màn hình một nội dùng nào đó trong C++, ta dùng 
{% highlight C %}
cout<<"Nội dung muốn hiển thị";
{% endhighlight %}

Nếu muốn hiển thị giá trị của một biến như là biến `myVariable`, ta dùng:
{% highlight C %}
cout<<myVariable;
{% endhighlight %}

Ta có thể kết hợp hiển thị vừa chuỗi nội dung vừa giá trị của biến như sau:
{% highlight C %}
cout<<"Biến myVariable = " <<myVariable;
{% endhighlight %}

Dấu `<<` được dùng để ngăn cách giữa phần "chuỗi" và phần biến. Lưu ý phần chuỗi phải để bên trong dấu nháy kép "chuỗi".

Áp dụng vào một chương trình hoàn chỉnh như sau:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable = 0;
  myVariable++;
  cout<<"Biến myVariable = " <<myVariable;//In ra màn hình: "Biến myVariable = 1"
  return 0;
}
{% endhighlight %}


Lưu ý là muốn dùng `cout`, ta phải khai báo thư viện `<iostream>` bằng dòng lệnh:

{% highlight C %}
#include <iostream>
{% endhighlight %}


{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  int myVariable = 0;
  int total = 0;
  total = 2 * myVariable++;
  cout<<"Biến myVariable = " <<myVariable;//In ra màn hình: "Biến myVariable = 0"
  return 0;
}
{% endhighlight %}


Bài sau chúng ta sẽ tiếp hiểu về câu lệnh if/else


