

# Random note

````javascript
var commentText = 'Để hiển thị được chuỗi chứa dấu gạch chéo ngược (\\) ta phải thêm dấu \\ vào trước hoặc sau nó'

console.log(commentText)
````



## isSafeInteger

````javascript
Number.isSafeInteger(123) //true
Number.isSafeInteger(-123) //true
Number.isSafeInteger(5-2) //true
Number.isSafeInteger(0) //true
Number.isSafeInteger(0.5) //false
Number.isSafeInteger(Math.pow(2, 53)) //false
Number.isSafeInteger(Math.pow(2, 53) - 1) //true
Number.isSafeInteger('123') //false
Number.isSafeInteger(false) //false
Number.isSafeInteger(Infinity) //false
Number.isSafeInteger(-Infinity) //false
Number.isSafeInteger(0 / 0) //false
````

## isInteger

````javascript
Number.isInteger(123) //true
Number.isInteger(-123) //true
Number.isInteger(5-2) //true
Number.isInteger(0) //true
Number.isInteger(0.5) //false
Number.isInteger('123') //false
Number.isInteger(false) //false
Number.isInteger(Infinity) //false
Number.isInteger(-Infinity) //false
Number.isInteger(0 / 0) //false
````


## isFinite

```javascript
Number.isFinite(123) //true
Number.isFinite(-1.23) //true
Number.isFinite(5-2) //true
Number.isFinite(0) //true
Number.isFinite('123') //false
Number.isFinite('Hello') //false
Number.isFinite('2005/12/12') //false
Number.isFinite(Infinity) //false
Number.isFinite(-Infinity) //false
Number.isFinite(0 / 0) //false
```





