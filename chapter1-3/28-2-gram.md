# 문제 28 : 2-gram

### 문제 28 : 2-gram

2-gram이란 문자열에서 2개의 연속된 요소를 출력하는 방법입니다. 예를 들어 'JavaScript'를 2-gram으로 반복해본다면 다음과 결과가 나옵니다.

**입력으로 문자열 주어지면 2-gram으로 출력하는 프로그램**을 작성해주세요.

```javascript
// 입력
// JavaScript

// 출력
// J a
// a v
// v a
// a s
// s c
// c r
// r i
// i p
// p t
```

### 문제 답안

```javascript
const str = prompt().split('');

for (let i = 0; i < str.length - 1; i++) {
  console.log(str[i], str[i + 1]);
}
```

