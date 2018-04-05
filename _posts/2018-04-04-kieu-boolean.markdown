---
layout: xxx
title:  "Kiểu dữ liệu Boolean"
short-title: "C++ Kiểu Boolean"
sub-title: "Bài 9"
body: "alu"
date:   2018-04-04 18:11:45 -0800
categories: basic cplusplus
---
<!--{% include mycomponent.html %}-->

Kiểu dữ liệu boolean là kiểu dùng để lưu trữ giá trị logic đúng hay sai. Trong C++ muốn khai báo một biến thuộc kiểu boolean, ta ghi như sau:

{% highlight C++ %}
  bool isCorrect;
{% endhighlight %}

Sau đó ta có thể gán biến isCorrect các giá trị true/false:

{% highlight C++ %}
  bool isCorrect;
  isCorrect = true;
  isCorrect = false;
{% endhighlight %}

Ngoài ra cũng có thể gán giá trị số nguyên, số 0 đồng nghĩa với giá trị false (sai), số từ 1 trở đi đồng nghĩa với giá trị true (đúng).

{% highlight C++ %}
  bool isCorrect;
  isCorrect = 1;//tương đương isCorrect = true;
  isCorrect = 0;//tương đương isCorrect = false;
  isCorrect = 100;//tương đương isCorrect = true;
{% endhighlight %}

Sau đây là cách sử dụng biến thuộc kiểu boolean với câu lệnh if:

{% highlight C++ %}
  bool isCorrect;
  isCorrect = true;
  if (isCorrect){
    cout<<"Đúng rồi đó!";
  }else{
    cout<<"Sai rồi!";
  }
{% endhighlight %}

Và kết hợp với toán tử logic `!`

{% highlight C++ %}
  bool isCorrect;
  isCorrect = true;
  if (!isCorrect){
    cout<<"Sai rồi!";
  }else{
    cout<<"Đúng rồi đó!";

  }
{% endhighlight %}

Bài sau ta sẽ học về cách nhận dữ liệu người dùng từ bàn phím.


