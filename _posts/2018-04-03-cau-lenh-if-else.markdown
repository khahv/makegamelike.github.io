---
layout: xxx
title:  "Câu lệnh if/else"
short-title: "C++ If/else"
sub-title: "Bài 7"
body: "alu"
date:   2018-04-02 23:11:45 -0800
categories: basic cplusplus
---
<!--{% include mycomponent.html %}-->

Câu lệnh `if/else` được dùng trong C++ để đưa ra quyết định cho từng trường hợp khác nhau. Ví dụ khi các bạn cân nặng trọng lượng cơ thể của mình, sau đó so sánh với chiều cao để tính ra chỉ số [BMI](https://vi.wikipedia.org/wiki/Ch%E1%BB%89_s%E1%BB%91_kh%E1%BB%91i_c%C6%A1_th%E1%BB%83).

- Nếu chỉ số `BMI` < **18.5** xin chia buồn bạn khá gầy.

- Nếu chỉ số `BMI` của bạn nằm trong khoảng **18.5-25**, xin chúc mừng cơ thể của bạn bình thường. 

- Nếu chỉ số `BMI` vượt quá **25**, bạn đã bị béo phì!

Như vậy ứng với mỗi kết quả `BMI` mà ta cần phải cho người cân biết tình trạng sức khoẻ của mình.


Chúng ta cùng xem ví dụ sau để hiểu rõ hơn:



{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  float BMI = 20;
  if (BMI < 18.5)
    cout<<"Cơ thể bạn quá gầy";
  else if (BMI >= 18.5 && BMI <=25)
    cout<<"Cơ thể bạn bình thường";
  else if (BMI > 25)
    cout<<"Bạn bị béo phì!";
  return 0;
}
{% endhighlight %}

Ở đoạn mã trên, chúng ta khai báo biến `BMI` thuộc kiểu `float` vì chỉ số BMI là kiểu số thực. Nếu chạy chương trình trên, kết quả in ra màn hình sẽ là `Cơ thể bạn bình thường`. Vì biến `BMI` có giá trị = 20.

Một lưu ý nữa là ở chương trình tên ta viết
{% highlight C %}
  else if (BMI >= 18.5 && BMI <=25)
{% endhighlight %}

Đây là cách ghi phối hợp giữa else và if. Khi đó nó sẽ là sự kết hợp của cả `"phần còn lại"` và `"điều kiện mới"`.

`"Phần còn lại"` ở đây là những giá trị nằm ngoài vùng bé hơn **18.5**, tức tất cả các số thực lớn hơn hoặc bằng **18.5**. `"Phần điều kiện mới"` là tất cả các số thực lớn hơn hoặc bằng **18.5** và bé hơn hoặc bằng **25**. Kết hợp 2 điều kiện này ta có điều kiện lớn hơn hoặc bằng **18.5** và bé hơn hoặc bằng **25**.

Các dấu `<, >, <=, >=` ở trên được gọi là toán tử so sánh. Ở phần sau ta sẽ tìm hiểu kỹ hơn các toán tử này.