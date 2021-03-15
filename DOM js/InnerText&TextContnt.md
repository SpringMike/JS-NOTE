## innerText & textContent

1. innerText là lấy ra những text trong 1 cái thẻ html ( h1, div , ...)

2. textContent là lấy hết những gì có trong HTML bao gồm cả thẻ tag

   <a>,<p>,<style>,<script>

````javascript
document.querySelector('.box').textContent='Học lập trình tại F8';
document.querySelector('div:nth-child(2)').textContent/*innterText*/='Thao tác với DOM qua bài tập tại F8';
````

