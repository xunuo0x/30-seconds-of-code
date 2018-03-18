### arrayLcm

计算数组最小公倍数

使用`Array.reduce()`，每次计算出的lcm为累加器的结果，参与下次计算；与计算数组GCD类似
> `Array.reduce()`对累加器和数组中每个元素应用一个函数，结果为最后一个值

```js
const arrayLcm = arr => {
  const gcd = (x, y) => !y ? x : gcd(y, x % y);
  const lcm = (x, y) => (x * y) / gcd(x, y);
  return arr.reduce((a, b) => lcm(a, b));
};
```

```js
arrayLcm([1,2,3,4,5]) // 60
arrayLcm([4,8,12]) // 24
```
