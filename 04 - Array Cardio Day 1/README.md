# Javascript array method 

### filter() - 주어진 판별 함수를 통과하는 요소를 모아 새로운 배열로 만들어 반환합니다.
```javascript
var words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];
const result = words.filter(word => word.length > 6);
console.log(result);  // expected output: Array ["exuberant", "destruction", "present"]
```

### map() - 매핑..배열 내의 모든 요소 각각에 대하여 주어진 함수를 호출한 결과를 모아 새로운 배열을 반환합니다.
```javascript
var array1 = [1, 4, 9, 16];
  // pass a function to map
const map1 = array1.map(x => x * 2);
console.log(map1); // expected output: Array [2, 8, 18, 32]
```

### sort() - 배열의 요소를 적절한 위치에 정렬한 후 그 배열을 반환합니다.
```javascript
var array1 = [1, 3, 4, 2, 5];
array1.sort();
console.log(array1); // expected output: Array [1, 2, 3, 4, 5]
```

### reduce() - 배열의 각 요소에 대해 주어진 리듀서(reducer) 함수를 실행하고, 하나의 결과값을 반환합니다. - 누적계산기
```javascript
//배열.reduce((누적값, 현재값, 인덱스, 요소) => { return 결과 }, 초깃값); 

```
### includes() : 배열이 특정 요소를 포함 하고 있는지 여부를 확인하고  알맞게 true 또는 false를 반환한다.

### splice() : 메서드는 배열의 기존 요소를 삭제 또는 교체 하거나 새 요소를 추가여 배열의 내용을 변경합니다.

### split() : 문자열을 특정 구분자 기준으로 나누어 배열로 만드는 메서드입니다.

### Array.form() : 메서드는 유사 배열 객체(array-like object)나 반복 가능한 객체(iterable object)를 얕게 복사해 새로운 Array 객체를 만듭니다.

### reduce()
- 빈도수 집계(counting)에 가장 많이 사용되는 전형적인 로직입니다.

```javascript
const transportation = data.reduce(function (obj, item) {
  if (!obj[item]) { //해당항목이 처음 등장했다면
    obj[item] = 0;
  }
  obj[item]++;
  return obj;
}, {});

```
["car", "bike", "car", "bus", "bike", "car"]  ==> 

{
  car: 3,
  bike: 2,
  bus: 1
}