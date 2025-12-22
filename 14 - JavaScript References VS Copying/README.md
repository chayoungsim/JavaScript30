# JavaScript References VS Copying

### .slice()는 배열의 일부분을 선택하여 새로운 배열을 만듭니다.
### array.slice( start, end )
* start와 end에는 숫자가 들어갑니다. 배열의 start에 해당하는 요소부터 end 바로 전의 요소까지를 선택하여 새로운 배열을 만듭니다.
* end에 값이 없으면 해당 배열의 마지막 요소까지 선택합니다. 값이 음수면 마지막 요소를 기준으로 선택합니다.

### concat() 
- 메서드는 인자로 주어진 배열이나 값들을 기존 배열에 합쳐서 새 배열을 반환합니다. 

### Array.from() 
- 메서드는 배열의 형태를 갖거나 순회 가능한 객체로부터 얕게 복사한 Array 객체를 만듭니다.

### Object.assign() 
- 메소드는 열거할 수 있는 하나 이상의 출처 객체로부터 대상 객체로 속성을 복사할 때 사용합니다. 대상 객체를 반환합니다.
```javascript
  const obj={a:1};
  const copy = Object.assign({},obj);
  console.log(copy) // {a:1}
```

### JSON.parse() 
- 메서드는 JSON 문자열의 구문을 분석하고, 그 결과에서 JavaScript 값이나 객체를 생성합니다. 선택적으로, reviver 함수를 인수로 전달할 경우, 결과를 반환하기 전에 변형할 수 있습니다.
```javascript
const data1 = {"name":"sim","age":20,"weight":48}; // JSON 형식의 문자열
const person1= JSON.parse(data);  // JSON 형식의 문자열을 자바스크립트 객체로 변환함.       
console.log(person) //{name: "sim", age: 20, weight: 48}
```

### JSON.stringify()
- 메소드는 인수로 전달받은 자바스크립트 객체를 문자열로 변환하여 반환합니다.
```javascript
  const person = {
    name:'sim',
    age:20,
    weight:48
  } //자바스크립트객체 
  const data = JSON.stringify(person); //자바스크립트 객체를 문자열로 변환함.

  consol.log(data) //{"name":"sim","age":20,"weight":48} 
```
