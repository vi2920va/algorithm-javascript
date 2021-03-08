# 문제 6 : false

### 문제 6 : false

다 음은 JavaScript 문법 중에서 false로 취급하는 것들 입니다. 앗 false로 취급되지 않는 것이 하나 있네요! true를 찾아주세요.

1. NaN
2. 1
3. "" - 빈 문자 
4.  0
5. undefined

### 문제 6 : false\(풀이\)

JavaScript에서는 false로 취급되는 값을 **falsy**라고 하고,  true로 취급되는 값을 **truthy**라고 한다. fasly로 취급 되는 값들을 보면 NaN, ""-빈 문자, 0, undefined가 있다.여기서 숫자는 0을 제외한 모든 나머지는 true로 취급된다.

```javascript
// 논리 부정 연산자를 사용해서 결과를 반대로 출력.
console.log(!0); // true
console.log(!1); // false
```





