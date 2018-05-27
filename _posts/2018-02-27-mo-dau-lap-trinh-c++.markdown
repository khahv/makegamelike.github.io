---
layout: xxx
title:  "Mở đầu về lập trình C++"
short-title: "C++ Mở đầu"
sub-title: "Bài 1"
body: "alu"
date:   2018-02-27 01:11:45 -0800
categories: basic cplusplus
---
<!--{% include mycomponent.html %}-->

Sau đây là ví dụ về một chương trình C++:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  cout << "Programming is great fun!";
  return 0;
}
{% endhighlight %}



Phần `#include...` chúng ta sẽ khai báo tên những thư viện cần thiết cho chương trình. Ở đây chúng ta dùng thư viện `'iostream'`
cần thiết cho hàm cout để in chuỗi ra màn hình. 

Sau khi khai báo các thư viện cần thiết, tiếp theo ta thấy dòng `using namespace std;`. Với người mới học C++, chúng ta không cần bận tâm về dòng này. Nếu không có nó, ta sẽ phải ghi 
`std::cout` thay vì `cout`. Cứ tạm thời nhớ như vậy đã nhé.

Kế tiếp là phần quan trọng nhất của một chương trình C++. Được gọi là phần body, chứa nội dung chạy chính của chương trình.
Hàm main() sẽ là nơi chương trình khởi chạy đầu tiên.
Tạm thời chúng ta chỉ cần ghi nhớ cú pháp `int main(){.... return 0;}` cái đã. Từ từ ở các bài sau sẽ chúng ta sẽ tìm hiểu kỹ hơn.

`cout<<"chuoi muon in ra man hinh"` là cách mà chúng ta sẽ hiển thị một chuỗi ra màn hình console, chuỗi nằm bên trong dấu ngoặc kép sẽ được in ra màn hình. Như trong ví dụ của chương trình trên, màn hình của chúng ta sẽ hiển thị dòng chữ:
`Programming is great fun!`.

Học C++ thật dễ dàng đúng không các bạn!


