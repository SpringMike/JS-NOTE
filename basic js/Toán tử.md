# Toán tử

## toán tử so sánh

// Note

1. Khi sử dụng toán tử trừ (-) thì Javascript ưu tiên ép kiểu về dạng number rồi thực hiện phép trừ nhé. VD: '15' - 5 thì chuyển '15' thành 15, suy ra 15 - 5 = 10.

2. Với toán tử cộng (+) chỉ cần 1 vế không phải kiểu số thì JS sẽ ép sang kiểu chuỗi và thực hiện nối chuỗi. VD: 5 + '5' thì chuyển 5 thành '5', suy ra '5' + '5' = '55'.

//



/*

1. ===
2. !==

so sánh tuyệt đối, so sánh của value lẫn data type

*/



/*

var result = ‘a’ && ‘b’ && ‘c’

result = c

- check dk xem nó có thuộc 6 value k? thì lấy gán vào result

1. 0
2. NaN
3. False
4. undefind
5. ‘’
6. null

var result = ‘a’ || ‘b’ || ‘c’

- ngược lại bên trên, check xem nó có cái nào không thuộc 6 values thì gán

result = a

*/

## toán tử số học

1. ‘ + ’ -> Cộng
2. ‘ - ’ -> Trừ
3. ‘ * ’ -> Nhân
4. ‘ ** ’ -> Luỹ thừa ( vd: 3 ** 2 = 9)
5. ‘ / ’ -> Chia
6. ‘ % ’ -> Chia lấy số dư ( vd: 10 % 3 = 1)
7. ‘ ++ ’ -> Tăng lên một giá trị
8. ‘ – ’ -> Giảm đi một giá trị  

// prefix(trc) & postfix(sau)

```javascript
var a = 9
var result = a++ + a++ - --a;
// 9 + 10 - 10

/*
a++
Việc 1: sẽ copy a
Việc 2: sẽ lấy a + 1 
Việc 3: sẽ trả về a copy trươc khi cộng 1

--a
Việc 1: sẽ lấy a -1  
Việc 2: sẽ trả về a sau khi trừ 1
*/
```

## Toán tử logic

- && – And( và ) 
- || – Or( hoặc )
- ! – Not( Không phải ) 

