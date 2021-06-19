# 문제 35 : Factory  함수 사용하기

### 문제 35 : Factory 함수 사용하기

2제곱, 3제곱, 3제곱을 할 수 있는 Factory 함수를 만들려고 합니다.

`<pass>`에 코드를 작성하여 two 함수를 완성하세요.

```javascript
function one(n) {
  function two() {
    // pass
  }
  return two;
}

const a = one(2);
const b = one(3);
const c = one(4);

console.log(a(10));
console.log(b(10));
console.log(c(10));
```

### 문제 35 : Factory 함수 사용하기\(풀이\)

 함수 `one`은 매개변수로 `n`를 받고 `two` 함수를 반환한다. 매개변수 n은 2제곱, 3제곱 등을 받은 수를 의미.

```javascript
function one(n) {
  function two(x) {
    // pass
    return Math.pow(x, n);
  }
  return two;
}

const a = one(2);
const b = one(3);
const c = one(4);

console.log(a(10)); // 100
console.log(b(10)); // 1000
console.log(c(10)); // 10000
```

#### Reference

Math.pow\(\)[→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/pow)

