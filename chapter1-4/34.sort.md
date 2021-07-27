# 문제 34 : sort 구현하기

### 문제 34 : sort 구현하기

민주는 체육부장으로 체육시간이 되면 반 친구들이 제대로 키 순서대로 모였는지를 확인해야 한다. 그런데 요즘 민주는 그것이 너무 번거롭게 느껴져 한 번에 확인하고 싶어한다.

민주를 위해 **키가 주어지면 순서대로 제대로 섰는지 확인하는 프로그램**을 작성해보자. \(키는 공백으로 구분하여 입력됩니다\)

```javascript
// 입출력

// 입력 : 176 156 155 165 166 169
// 출력 : NO

// 입력 : 155 156 165 166 169 176
// 출력 : YES
```

### 문제 답안

먼저 `unsorted` 변수에 키를 입력 받아서 배열로 변환한 다음에 ****`arr.sort()`메서드를 통해서 오름차순 정렬해줘야 한다. 오름차순을 통해서 정렬된 배열은 문자열로 다시 바꿔준 다음에 입력 받은 값과 정렬된 값과 비교하여 그에 따른 결과값을 반환한다.

```javascript
const unsorted = prompt('');
let sorted = unsorted
  .split(' ')
  .sort((x, y) => x - y)
  .join(' ');

console.log(unsorted === sorted ? 'YES' : 'NO');
```

####  Reference

String.prototype.split\(\)[→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/String/split)

Array.prototype.sort\(\)[→\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)

Array.prototype.join\(\)[ →\(MDN\)](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array/join)

Conditional \(ternary\) operator [→\(MDN\)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_Operator)

