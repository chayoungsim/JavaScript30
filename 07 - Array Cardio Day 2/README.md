# Array Cardio Day 2

## Array​.prototype​.some()
 * 배열을 순회하면서 특정조건을 배열의 값들이 만족시키는지 검사 
 * some 은 일부만 만족해도 true 를 return 한다.
 * 빈 배열에서 호출하면 무조건 false를 반환합니다.
 * true 를 만족하는 첫번재 원소를 만나면 순회를 중단하고 결과값으로 true 를 return

## Array​.prototype​.every()
 * 배열을 순회하면서 특정조건을 배열의 값들이 만족시키는지 검사 - 
 * every() 모든 값이 조건을 만족해야 true 를 return 한다.
 * 빈 배열에서 호출하면 무조건 true를 반환합니다.
 * every 메서드는 false 를 만족하는 첫 번째 원소를 만나면 순회를 중단하고 결과 값으로 false 를 return 한다

#### every나 some 함수의 경우 배열내 값이 존재하는지 확인할때나 조건에 맞는(혹은 맞지 않는) 값이 있는지 확인 할 때 등 활용이 가능합니다.
#### 모든배열요소가 조건을 만족하는지 알고싶다면 every 그렇지 않다면 some을 사용하면 된다.

## Array.prototype.find()
 * 메서드는 주어진 판별 함수를 만족하는 첫 번째 요소의 값을 반환합니다

## Array.prototype.findIndex()
 * 주어진 판별 함수를 만족하는 배열의 첫 번째 요소에 대한 인덱스를 반환합니다. 만족하는 요소가 없으면 -1을 반환합니다.


## splice()  - 삭제,교체 새요소를 추가하여 배열의 내용을 변경합니다.
 * array.splice( start, count )

## ...SPREADS