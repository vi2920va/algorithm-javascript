# 문제 35 : Factory  함수 사용하기

### 문제 35 : Factory 함수 사용하기

2제곱, 3제곱, 3제곱을 할 수 있는 Factory 함수를 만들려고 합니다.

&lt;pass&gt;에 코드를 작성하여 two 함수를 완성하세요.

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

