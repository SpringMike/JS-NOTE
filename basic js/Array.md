

# Array-1

**var array = ['js','java','php'];**

## to string

```javascript
console.log(array.toString());
```

## Join

```javascript
console.log(array.join(', '));
// giong to string nhung kiem soat duoc khoang cach trong giua 2 phan tu
```

## pop

````javascript
console.log(array.pop());
// xoa phan tu cuoi trong mang va tra ve phan tu day
````

## push

```javascript
console.log(array.push('dart'))
// them phan tu vao cuoi mang va tra ve do dai moi cua mang
```

## shift

```javascript
console.log(array.shift());
// xoa phan tu vao dau mang va tra ve phan tu day
```

## unshift

````javascript
console.log(array.unshift('dart2'))
// them phan tu vao dau mang va tra ve do dau moi cua mang
````

## splice

```javascript
// splice dung de xoa
array.splice(2,1,'minh','ha')
// splice dung de edit
array.splice(2,0,'minh','ha')
//splice dung de them vao vi tri index
array.splice(2,2,'dart')
console.log(array)
```

## concat

````javascript
var array2 = ['minh','hai','long']
console.log(array.concat(array2))
// noi giua 2 mang thanh 1
````

## slice

````javascript
console.log(array.slice(1,2))
// cat mang tu mot 1 vi tri den vi tri end
console.log(array.slice(0))
//copy ca mang
````

## inclues()

````javascript
// Làm bài tập tại đây
function run(input) {
    if(typeof input === 'string' || Array.isArray(input)){
        if(input.includes('F8')){
            console.log(true)
            return true
        }else{
            console.log(false)
            return false
        }
    }
    else{
        console.log(false)
        return false
    }
}
run('Học lập trình tại F8')
````





# Array-2



## forEach()

````javascript
courses.forEach(function (course,index){
    console.log(course, index)
})
//vd:
function getRequestBodyFromValues(formValues) {
    var obj={};
    formValues.forEach(function (item)
    {
        obj[item.field]=item.value;
    })
    return obj;
}
````

## every()

````javascript
var course = courses.every(function(course){
    return course.coin === 0
})
console.log(course)
// trả về boolean
//Dạng như là kiểm tra xem có ít nhất thằng nào trong array vượt qua được cuộc kiểm tra không. 1 thằng sai thì trả về false, tất cả đúng thì true

//vd:
function checkPositiveNumbers(numbers) {
    var result = numbers.every(function(number){
        return number > 0
    })
    return result
}
````

## some()

````javascript
var course = courses.some( function(course){
    return course.coin ===0
} )
// cũng return boolean
console.log(course)
//Nó check hết item trong mảng xem có item nào thoả mãn điều kiện rồi trả về true or false. có ít nhất 1 item thì true không thì false
//vd:
function hasFreeCourses(courses) {
    var result = courses.some(function(course){
        return course.vnd === 0
    })
    return result
}

````

## find()

`````javascript
var listCours = courses.find(function (course){
    return course.name ==== 'java'
})
console.log(listCours)
// hàm tìm kiếm chỉ trả về 1 item
//vd:
function findAMonsterByAttack(monsters) {
    var monsterFind = monsters.find( function(monster){
           return monster.attack === 150
    })   
    if(monsterFind){
        return monsterFind
    }
    else{
        return null
    }
}
`````

## filter()

````javascript
var listCourse = courses.filter(function(course){
    return course.name.toLocaleLowerCase() === 'java'
})
console.log(listCourse)
// hàm tìm kiếm trả về nhiều item 

//vd: 

function findStringsInArrayByKeyword(keyword, strings) {
    var arrayFind = strings.filter(function(string){
        return string.indexOf(keyword) !== -1
    })   
    if(arrayFind != null){
        console.log(arrayFind)
        return arrayFind
    }
    else{
        return null
    }
}
findStringsInArrayByKeyword('PHP', ['Javascript', 'PHP'])

// vd2: Input: [1, 2, 6, 8], [2, 9, 6] - Output: [2, 6]
function findEqualValues(array1, array2){
    return array1.filter(function(num) {
        return array2.indexOf(num) !== -1;
    })
}
findEqualValues(['Gấu'], ['Gấu', 'Hằng', 'Linh', 'Trang', 'Con gái'])
````

````javascript
--------------MyFilter()-----------------
    var courses = [
  {coin:123,name: 'PHP'},
  {coin:456,name: 'Javascript'},
  {coin:789,name: 'Ruby'},
  {coin:963,name: 'Python'},
];
Array.prototype.filters = function(callbacks){
  var output = [];
  for(var item in this){
     if(this.hasOwnProperty(item)){
       var result = callbacks(this[item],item,this);
       if(result){
         output.push(this[item]);
       }
     }
  }
  return output;
}

var newCourse = courses.filters((item,index,arr)=>{
  return item.coin > 460
});

console.log(newCourse);
````



## Map()

````javascript
// Làm việc tại đây
function convertToNumber(inputs) {
    
    var newArray = inputs.map(function(input){
        return input.join('')
       	return input*3
    })
    return newArray
}
//Map() nó tạo ra một array mới bằng việc ta xử lý những item của array cũ bằng phương thức của chúng ta xử lý.
````

`````javascript
---------------MyMap()--------------------
var courses = [
  'PHP',
  'Java',
  'Ruby'
]

Array.prototype.map2 = function(callback){
  var output=[]
  for(var i =0 ; i < this.length;i++){
  
    output.push(callback(this[i]))
  }
  return output
}

var html = courses.map2(function(course){
  return `${course}`
})
console.log(html.join('. '))
`````



## Reduce()

````javascript
// chả biết nói như nào nữa

function run(courses) {
    var result = courses.reduce(function(total,course){
        return total + course.coin
    },0) // có inital value thì sẽ bắt đầu từ 0
    // còn không có thì nó sẽ lấy đối tượng course làm biến lưu trữ rồi bắt đầu từ item course 2 trong 1 lần lấy... Hi vọng bro hiểu ^^
    return result
}
````

link: https://anonystick.com/blog-developer/25-truong-hop-su-dung-reduce-javascript-2020062089156060



## Etc…

https://anonystick.com/blog-developer/javascript-developer-javascript-nen-biet-nhung-method-arrays-nao-trong-javascript-x0ZB3R6E#t-3