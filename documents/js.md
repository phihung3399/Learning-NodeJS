# Javascript căn bản:

## Khai báo biến:
Sử dụng 1 trong 3 từ khóa: 
- var
- let
- const

Không quan tâm kiểu biến lúc khai báo

```js
var a;
let b;
const c = "Hằng số";

// do something
a = "Hello";    // a -> string
b = 10;         // b -> int
c = "Abc";      // lỗi, hằng số ko cho thay đổi giá trị

// do other things
a = 10;     // a -> int, a tu dong chuyen tu string sang int
a = 10.5    // a -> float
```

## Xuất ra màn hình:

```js
console.log("Xuat dong nay ra man hinh")
```

## Nối chuỗi / Phép toán cộng:
- Nếu trong biểu thức **có ít nhất 1 giá trị là chuỗi** thì phép cộng là **nối chuỗi**.
- Nếu là các giá trị số thì sẽ thực hiện **phép toán cộng**.

```js
var soTuoi = 10
var hoi = "Toi " + soTuoi + " tuổi";    // Tôi 10 tuổi

var a = 10
var b = 20
var c = a + b;  // 30, a và b là số, thực hiện phép toán cộng

var a = 10
var b = 20
var c = "Nối chuỗi " + a + b;  // Nối chuỗi 1020, cộng chuỗi chứ ko cộng số
```

## Phép toán:
1. Phép toán `++` và `--`:

```js
// Cách thứ 1: ++ nằm trước biến
var c = 12;
console.log(++c); // kết quả là 13
console.log(c); // kết quả là 13

// Cách thứ 2: ++ nằm sau biến
var c = 12;
console.log(c++); // kết quả là 12
console.log(c); // kết quả là 13
```

2. Phép toán gán:
- `x += y`
- `x -= y`

3. Toán tử quan hệ:

```js
a >= b
a <= b
a == b
a === b
a != b
```

4. Phép toán true/false:
- Bao gồm:
  + Và `&&`
  + Hoặc `||`
  + Phủ định `!`

```js
var a = false;
var b = true;
console.log(a && b); // TRUE
console.log(a || b); // TRUE
console.log(!a); // TRUE
console.log(!b); // FALSE
```