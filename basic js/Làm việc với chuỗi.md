# Làm việc với chuỗi

<u>var myString = 'Hoc JS tai F8'</u>

### length

````javascript
console.log(myString.length)
````

### index of

````javascript
console.log(myString.indexOf('JS',5))
//value, numberStart
//myString.lastIndexOf(..)

//Phương thức indexOf() sẽ tìm substring bên trong một string, nếu tìm được thì sẽ trả về vị trí kí tự đầu tiên của substring bên trong string, ngược lại sẽ trả về -1.
````

### cut string

````javascript
console.log(myString.slice(4,6))
//numberStart--> End
````

### replace

````javascript
console.log(myString.replace(/JS/g, 'JAVA'))
//oldValue --> newValue
````

### convert to upper case & lower case

````javascript
console.log(myString.toLowerCase())

console.log(myString.toUpperCase())
````

### trim

````javascript
console.log(myString.trim())
````

### spilt

````javascript
var myString2 = "java, JS, PHP"
console.log(myString.split(', '))
````

### get a character by index

`````javascript
console.log(myString.charAt(4))
console.log(myString[4])
`````

### search

`search()` được sử dụng khi bạn muốn tìm vị trí một string con trong string mẹ theo biểu thức chính quy. Nếu trong string mẹ xuất hiện nhiều lần string con cần tìm, thì trả về vị trí của string con đầu tiên. Phương thức này gần giống với `indexOf()`, khác ở chỗ `indexOf()` chỉ chấp nhận input là string, còn `search()` chấp nhận cả biểu thức chính quy.

````javascript
var n = str.search("Phambinh.net"); // 11
````

### more info

https://phambinh.net/bai-viet/cac-ham-lam-viec-voi-string-trong-javascript/#search

### kiểm tra String tồn tại Substring trong Javascript

https://viblo.asia/p/vo-van-cach-de-kiem-tra-string-ton-tai-substring-trong-javascript-1VgZv16rKAw