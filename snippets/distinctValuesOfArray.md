### distinctValuesOfArray

- 数组去重，采用`Set`以及`...rest`剩余运算符去重。
- 也可以采用`Map`去重。

```js
const distinctValuesOfArray = arr => [...new Set(arr)];
```

```js
distinctValuesOfArray([1,2,2,3,4,4,5]) // [1,2,3,4,5]
```
