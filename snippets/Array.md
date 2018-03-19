# 数组操作集合

## Array.map()

> `map()`方法创建一个新数组，其结果是该数组中的每个元素都调用一个提供的函数后返回的结果

```javascript
let new_array = arr.map(function callback(currentValue, index, array) {
    // Return element for new_array
}[, thisArg])
```

## Array.concat()

> `concat()`方法用于合并两个或多个数组。此方法不会更改现有数组，而是返回一个新数组

```javascript
var new_array = old_array.concat(value1[, value2[, ...[, valueN]]])
```

## Array.filter()

> `filter()`方法创建一个新数组, 其包含通过所提供函数实现的测试的所有元素。

```javascript
var new_array = arr.filter(callback[, thisArg])
```

### 与Array.map()的区别

`map()`是所有都会保留，组成新数组，`filter()`只会保留通过测试的
`forEach()`甚至不会有返回值，原数组也不会变化

## Array.find()

> `find()`方法返回数组中满足提供的测试函数的第一个元素的值。否则返回 undefined。

```javascript
arr.find(callback[, thisArg])
```