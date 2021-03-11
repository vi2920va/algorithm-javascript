# 문제 5 : for문 계산

### 문제 5 : for문 계산

다음 코드의 출력 값으로 알맞은 것은 ?

```javascript
let a = 10, b = 2;

for (let i = 1; i < 5; i += 2) {
  a += i;
}
console.log(a + b);
```

1. 10
2. 12
3. 14
4. **16**

### 문제 5:  for문 계산\(풀이\)

#### for

for 문은 초기화, 조건, 증감 세 가지 작업을 표현식으로 명시하고 있는 반복문이다. 

{% code title="Syntax" %}
```javascript
for ([초기화]; [조건]; [증감]) { ... }
```
{% endcode %}

for문의 흐름은 먼저 반복문이 시작되기 전에 '초기화' 표현식이 한 번 평가되고, 만약 '조건' 표현식이 true이면 반복문이 실행하고자 하는 명령문을 실행하고, 마지막으로는 '증감' 표현식이 실행된다. 이렇게 조건이 false로 평가될 때 까지 같은 흐름을 반복한다.

```javascript
// 문제
let a = 10, b = 2;

for (let i = 1; i < 5; i += 2) {
  // for문 반복 흐름
  // 1 < 5 : true, a = 12
  // 3 < 5 : ture, a = 14
  // 5 < 5 : false, a = 14 + 2
  a += i;
}

// 출력
console.log(a + b); // 16
```

#### Reference

for  [→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Statements/for)





