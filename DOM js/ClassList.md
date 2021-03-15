## add(*class1, class2, ...*)

```javascript
document.getElementById("myDIV").classList.add("mystyle");
//Thêm class "mystyle" vào phần tử <div>
```

## contains(*class*)

````javascript
console.log(h2Element.classList.contains('test'))

//Trả về giá trị Boolean, cho biết liệu một phần tử có tên class được chỉ định hay không.
````

## remove(*class1, class2, ...*)

````javascript
h2Element.classList.remove('test')

//Loại bỏ một hoặc nhiều tên lớp khỏi một phần tử.
//Note: Removing a class that does not exist, does NOT throw an error
````

## toggle(*class,* true|false)

```javascript
var h1Element = document.querySelector('h1')
h1Element.classList.toggle('red')

// cái thằng này nó sẽ kiểm tra xem cái thẻ h1 có class red chưa ? có thì nó sẽ xoá class red đi : còn không có thì nó sẽ thêm class red vào
```

