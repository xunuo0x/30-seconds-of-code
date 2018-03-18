### arrayGcd

计算数组的最大公约数（GCD）

采用`Array.reduce()`方法，每次调用`gcd`方法（递归），将结果作为下次调用`gcd`的初始值

`Array.reduce()`的参数

- callback
  - accumulator 累加器
  - currentValue 当前值
  - currentIndex > 可选
  - array > 可选

- initialValue > 可选

```js
const arrayGcd = arr => {
  const gcd = (x, y) => !y ? x : gcd(y, x % y);
  return arr.reduce((a, b) => gcd(a, b));
};
```

```js
arrayGcd([1,2,3,4,5]) // 1
arrayGcd([4,8,12]) // 4
```
