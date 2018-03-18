### arrayMin

返回数组中最小值；也可以使用`reduce()`做
这里面则用到`...`展开运算符
> `spead operator`允许一个表达式在期望多个参数（用于函数调用）或多个元素（用于数组字面量）或多个变量（用于解构赋值）的位置扩展

```js
const arrayMin = arr => Math.min(...arr);
```

```js
arrayMin([10, 1, 5]) // 1
```