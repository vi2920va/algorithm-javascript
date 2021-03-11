# 문제 9 : concat을 활용한 출력 방법

### 문제 9 : concat을 활용한 출력 방법

다음 소스 코드를 완성하여 날짜와 시간을 출력하시오.

{% code title="Problem" %}
```javascript
let year = '2021';
let month = '03';
let day = '11';
let hous = '15';
let minute = '32';
let second = '43';

// 아래의 result 변수에 빈 칸을 채워주세요.
let result;

// 출력 값 2021 / 03 / 11 /  15 : 32 : 43
console.log(result);
```
{% endcode %}

### 문제 9 : concat을 활용한 출력 방법\(풀이\)

#### 1\) String.prototype.concat\(\)

`concat()` 함수는 호출 문자열에 문자열 인수를 이어 붙인 결과를 반환한다. 원본 문자열과 결과 문자열의 변형은 서로에게 영향을 미치지 않는다. 만약 인수가 문자열이 아니면 계산 전에 문자열로 변환한다.

{% code title="Syntax" %}
```javascript
str.concat(string2, string3[, ..., stringN])
```
{% endcode %}

**매개변수\(Parameters\)**

`string2...stringN` 

합칠 문자열.

**반환 값\(Return Value\)**

주어진 문자열을 모두 붙인 새로운 문자열.





