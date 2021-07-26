# 문제 21 : set은 어떻게 만드나요?

### 문제 21 : set은 어떻게 만드나요?

다음 중 set을 만드는 방법으로 올바른 것을 모두 고루시오.

1. const x = {1, 2, 3, 4, 5};
2. const x = {};
3. **const x = new Set\('javascript'\);**
4. const x = new Set\(range\(5\)\);
5. **const x = new Set\(\);**

### 문제 답안

**Set**객체는 **중복되지 않는 값\(value\)을 저장하는 데이터 구조**이다. Set을 만드는 방법으로  **옳은 것은 3번과 5번**이지만, **3번은 중복되는 문자가 있어서 의도치 않게 저장될 수도 있다는 점**을 어렴해야 한다.

```javascript
// set은 중복되지 않은 데이터를 저장하는 데이터 구조
const list = [1, 2, 2, 3, 4, 5, 5, 5, 6];

const setVal = new Set(list);
setVal.add(10);
console.log(setVal);

const x = new Set('javascript');
console.log(x); // javscript
console.log(x.size); // 9
```

#### Reference

Set [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Set)

