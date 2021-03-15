## Vòng lặp For - lap cho den khi dieu kien thoa man~

### for / in - Lặp qua key của đối tượng

```javascript
var langues = {
    name: 'PHP',
    date: '2020'
}
var langues2 =[
    'PHP',
    'JAVA'
]

for (var key in langues){
    console.log(langues[key])
}
for (var key in langues2){
    console.log(langues[key])
}
```

### for / of - Lặp qua value của đối tượng

````javascript
var totalCoin = 0;
for (var course of coures){
    totalCoin+= course.coin
}
````

### Etc

https://anonystick.com/blog-developer/su-khac-biet-giua-forin-forof-and-foreach-trong-javascript-2020041337746860

### while - Lặp khi điều kiện đúng

### do / while - Lặp ít nhất 1 lần, sau đó lặp đến khi điều kiện đúng

### break - dung`  de dung vong lap

### continue – dung de bo qua 1 buoc, tiep tuc lan lap tiep theo



