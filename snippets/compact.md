### compact

Removes falsey values from an array.
移除数组中的值为`falsey`的元素

使用`Array.filter()`过滤false值，如`false`, `null`, `0`, `""`, `undefined`, `NaN`
> `filter()`方法创建一个新数组, 其包含通过所提供函数实现的测试的所有元素。
> var new_array = arr.filter(callback[, thisArg])
- callback 返回true|false，参数 (element, index, array)
- thisArg 可选。执行 callback 时的用于 this 的值

```js
const compact = arr => arr.filter(Boolean);
```

```js
compact([0, 1, false, 2, '', 3, 'a', 'e'*23, NaN, 's', 34]) // [ 1, 2, 3, 'a', 's', 34 ]
```
