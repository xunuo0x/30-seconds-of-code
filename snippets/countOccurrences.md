### countOccurrences

计算数组中特定元素出现次数

`Array.reduce()`函数中对每个element执行的回调函数的返回值作为累加器，累加器初始值为initialValue
> arr.reduce(callback[, initialValue])
- callback 执行数组中每个值的函数，包含四个参数：
  - accumulator 累加器累加回调的返回值; 它是上一次调用回调时返回的累积值；初始值为initialValue
  - currentValue
  - currentIndex 可选
  - array 可选
- initialValue 可选 用作第一个调用 callback的第一个参数的值。 如果没有提供初始值，则将使用数组中的第一个元素。 在没有初始值的空数组上调用 reduce 将报错。

```js
const countOccurrences = (arr, value) => arr.reduce((a, v) => v === value ? a + 1 : a + 0, 0);
```

```js
countOccurrences([1,1,2,1,2,3], 1) // 3
```
