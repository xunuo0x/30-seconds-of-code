### chunk

将数组以特定的size分成更小的块（数组）

`Array.from()`创建新数组
> `Array.from(arrayLike, mapFn, thisArg)`

- arrayLike 想要转换成数组的伪数组对象或可迭代对象
- mapFn (可选参数) 如果指定了该参数，**新数组中的每个元素会执行该回调函数**；名字里都有map，其参数类似`map(function callback(currentValue, index, array))`
- thisArg (可选参数) 可选参数，执行回调函数 mapFn 时 this 对象

- `Array.slice()`用于分割数组
> `slice()` 方法返回一个从开始到结束（不包括结束）选择的数组的一部分浅拷贝到一个新数组对象。且原始数组不会被修改。

```js
const chunk = (arr, size) =>
  Array.from({length: Math.ceil(arr.length / size)}, (v, i) => arr.slice(i * size, i * size + size));
```

```js
chunk([1,2,3,4,5], 2) // [[1,2],[3,4],[5]]
```
