# LocalStorage

## setItem() - key, value 추가
## getItem() - value 읽어오기
## removeItem() - item 삭제
## clear() - 모든 item 삭제
## length - 전체 item 갯수
## key() - index로 key값 찾기

- localStorage에 아이템 추가 - localStorage.setItem(key, value);
- localStorage에 아이템 읽기 - localStorage.getItem(key);
- localStorage에 아이템 삭제 - localStorage.removeItem(key);
- localStorage에 모든 아이템 삭제 - localStorage.clear();
- localStorage에 아이템 갯수 - localStorage.length;

### 객체, 배열을 JSON 문자열로 변환
- const objString = JSON.stringify(obj);
- const arrString = JSON.stringify(arr); 
### setItem
- window.localStorage.setItem('person', objString);
- window.localStorage.setItem('nums', arrString); 
### getItem
- const personString = window.localStorage.getItem('person');
- const numsString = window.localStorage.getItem('nums')
### JSON 문자열을 객체, 배열로 변환
- const personObj = JSON.parse(personString);const numsArr = JSON.parse(numsString);

* localStorage 에는 문자열만 저장됩니다.따라서, localStorage에 객체나 배열를 저장하기 위해서는 객체를 문자열로 변환해서 저장해야 합니다.
* 여기서는 JSON.stringify() 함수를 사용하여 객체와 배열을 JSON 문자열로 변환하였습니다.



### event.preventDefault()
- 현재 이벤트의 기본 동작을 중단한다.

### reset()
- default 값으로 설정한다.

### join()
-  배열의 모든 요소를 연결해 하나의 문자열로 만듭니다.