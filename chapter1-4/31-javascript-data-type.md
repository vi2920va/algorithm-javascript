# 문제 31 : JavaScript 자료형의 복잡도

### 문제 31 : JavaScript 자료형의 복잡도

다음 배열 내장 함수의 시간 복잡도가 O\(1\)이 아닌 것을 모두 고르시오.

1. arr\[i\]
2. arr.push\(5\)
3. **arr.slice\(\)**
4. arr.pop\(\)
5. **arr.includes\(5\)**

### 문제 답안

시간 복잡도는 알고리즘이 문제를 처리하는 데 얼마나 시간이 걸리는지 알려준다. 이러한 알고리즘 성능을 수학적으로 표현해주는 표기법이 **Big-O**  표기법 이라고 부른다. 즉, O\(1\)은 입력되는 데이터의 크기와 상관없이 알고리즘 문제를 해결해하는 속도가 모두 일정할 때 O\(1\)를 표기해준다. 

문제의 정답으로는 **3, 5번**이다. 그 이유는 **3번 `arr.slice()`**메서드는 매개변수만큼 잘라서 새로운 배열을 반환하는데, 배열의 크기가 커지면 사용되는 메모리가 많아지기 때문에 O\(1\)이 아니다. 마지막으로 **5번 `arr.includes(5)`**메서드는 매개변수가 배열에 들어잇는지 확인하는 메서드로 배열의 크기가 커지면 탐색해야 하는 값도 많아지기 때문에 O\(1\)이  아니다.





