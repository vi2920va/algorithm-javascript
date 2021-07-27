# 문제 45 : getTime\(\)함수 사용하기

### 문제 45 : getTime\(\)함수 사용하기

Date객체의 메서드 중 하나인 `getTime()`은 1970년 1월 1일 0시 0분 0초 이후로부터 지금까지 흐른 시간의 천분의 1초 단위\(ms\)로 반환합니다.

이를 이용하여 **현재 연도\(2021\)년을 출력해보세요.**

### 문제 답안

#### 1\) 내가 풀은 답안

Date 객체의 `getFullYear()`메서드를 사용해서 현재 연도 출력

```javascript
const theDate = new Date();
console.log(theDate.getFullYear()); // 2021
```

#### 2\) 다른 답안

1년 단위 초를 구해서 ms단위로 변환해서 값을 구하면 손 쉽게 구할 수  있다.

```javascript
const theDate = new Date();
const yearMs = 60 * 60 * 24 * 365 * 1000;
console.log(Math.floor(theDate.getTime() / yearMs) + 1970);
```

#### Reference

Date[→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Date/Date)

