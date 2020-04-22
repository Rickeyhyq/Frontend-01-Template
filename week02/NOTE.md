# 第二周作业

### 写一个正则表达式 匹配所有 Number 直接量
```javascript
// 整数
var str1 = "123";
var reg = /^-?\d+$/g;
console.log(reg.test(str1));
// 浮点数
var str2 = "11.1234";
var reg = /^(-?\d+)(\.\d+)?$/g;
console.log(reg.test(str2));
// 二进制
var str3 = "0b00110011";
var reg = /^0[bB][01]+$/g;
console.log(reg.test(str3));
// 八进制
var str4 = "0o66117711";
var reg = /^0[oO][0-7]+$/g;
console.log(reg.test(str4));
// 十六进制
var str5 = "0xaf1e7d11";
var reg = /^0[xX][0-9a-fA-F]+$/g;
console.log(reg.test(str5));
// Number
var reg = /^-?\d+$|^(-?\d+)(\.\d+)?$|^0[bB][01]+$|^0[oO][0-7]+$|^0[xX][0-9a-fA-F]+$/g;
```
### 写一个正则表达式，匹配所有的字符串直接量，单引号和双引号
```javascript
var reg = /[\u0021-\u007E]{6,16}|[\x21-\x7E]{6,16}|(['"])(?:(?!\1).)*?\1/g
```
### 写一个 UTF-8 Encoding 的函数
```javascript

```

### 本周总结