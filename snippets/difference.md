### difference

Returns the difference between two arrays.
返回两个数组间的差异

建立集合`Set`，集合的特点是：
> `Set`对象允许你存储任何类型的唯一值，无论是原始值或者是对象引用。
> `Array.filter()`保留通过测试的值

```js
const difference = (a, b) => { const s = new Set(b); return a.filter(x => !s.has(x)); };
```

```js
difference([1,2,3], [1,2,4]) // [3]
```
