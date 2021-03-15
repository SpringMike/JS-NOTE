# Built-in 
// hàm có sẵn

## 1. Alert

```javascript
alert('hello world')
```

## 2.Console

```javascript
console.log('hello world')
```

## 3.Confirm

````javascript
// bật hộp thoại có được chọn CÓ hoặc CANCEL
confirm('hello my friends')
````

## 4.Prompt

````javascript
//bật hộp thoại có được chọn CÓ hoặc CANCEL và có input
prompt('ban co du 18 tuoi khong?')
````

## 5.Set timeout

````javascript
// chạy 1 lần một đoạn code sau 1 khoảng thời gian (1000 mil giây = 1 giây)
setTimeout(() => {
    alert('Hello!')
},1000)
````

## 6.Set interval

```javascript
// chạy nhiều lần một đoạn code sau 1 khoảng thời gian lặp đi lặp lại
setInterval( ()=> {
    console.log('day la hello' + Math.random())
},1000)
```

