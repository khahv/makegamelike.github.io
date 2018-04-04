---
layout: xxx
title:  "Toán tử so sánh trong C++"
short-title: "C++ Toán tử so sánh"
sub-title: "Bài 8"
body: "alu"
date:   2018-04-03 18:11:45 -0800
categories: basic cplusplus
---
<!--{% include mycomponent.html %}-->

Phần này sẽ giới thiệu một số toán tử mà trong toán học bình thường không có.

Colons can be used to align columns.

| Toán tử so sánh        | Ý nghĩa           |
| ------------- |:-------------|
| <             | Số bên trái có nhỏ hơn số bên phải? |
| >             | Số bên phải có nhỏ hơn số bên trái?     |
| <=            | Số bên trái có nhỏ hơn hoặc bằng số bên phải?      |
| >=            | Số bên phải có nhỏ hơn hoặc bằng số bên trái?      |
| ==            | Hai số có bằng nhau?      |
| !=            | Hai số có không bằng nhau?      |


Lưu ý là toán tử `=` ta đã tìm hiểu ở bài trước là toán tử gán giá trị, còn toán tử `==` là toán tử so sánh xem 2 giá trị có bằng nhau hay không.

Các toán tử logic:

| Toán tử logic        | Ý nghĩa           |
| ------------- |:-------------|
| &&             | Đúng nếu cả 2 về đều đúng |
| \|\|             | Đúng nếu 1 trong 2 về đúng     |
| !              | đúng thành sai, sai thành đúng |

Lý thuyết như vậy là đủ rồi, cùng xem ví dụ sau đây để hiểu rõ hơn:

{% highlight C %}
  else if (BMI >= 18.5 && BMI <=25)
      cout<<"Cơ thể bạn bình thường";
{% endhighlight %}

Ở ví dụ trên của bài [if/else]({{page.previous.url}}) ta đã sử dụng toán tử so sánh `>=` để so sánh giữa 2 giá trị `BMI` và **18.5**, và cũng so sánh giá trị
của `BMI` và **25**. Đồng thời ta giao hai điều kiện này với nhau bằng toán tử logic`&&`. Như vậy nội dung bên trong câu lệnh else if{...} này chỉ chạy khi cả 2 điều trên cùng đúng (chỉ số `BMI` >= **18.5** và `BMI` <= **25**).


{% highlight C %}
  else if (BMI >= 18.5 || BMI <=25)
      cout<<"Cơ thể bạn bình thường";
{% endhighlight %}

Nếu ta đổi toán tử logic `&&` bằng `||`, thay vì giao giữa 2 điều kiện, ta chuyển thành hợp giữa 2 điều kiện. Nghĩa là một trong 2 về đúng, thì nội dung bên trong câu lệnh else if sẽ chạy.

Vd: 
BMI = 20 -> >=18.5 -> true
BMI = 100 -> => 18.5 -> true
BMI = 0 <= 25 -> true

Ở đây ta nhận thấy khi giao 2 điều kiện trên, mọi giá trị của BMI đều thoả điều kiện.

Ở ví dụ tiếp theo, giả sử ta muốn in ra màn hình khi biến BMI có giá trị khác 20, ta sẽ phải dùng câu lệnh else để lấy những giá trị ngược lại như sau:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  float BMI = 20;
  if (BMI == 20)
  {

  }else
  {
    cout<<"Chỉ số BMI của bạn không phải là 20";
  }
  return 0;
}
{% endhighlight %}


Đoạn mã trên có thể được viết lại dùng toán tử logic `!`:

{% highlight C %}
// A simple C++ program
#include <iostream>
using namespace std;

int main() 
{
  float BMI = 20;
  if (BMI != 20)
  {
    cout<<"Chỉ số BMI của bạn không phải là 20";
  }
  return 0;
}
{% endhighlight %}



