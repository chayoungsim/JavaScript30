# JavaScript Drum Kit
- 특정 키보드 키를 눌렀을때 사운드 시작, 엑티스 클래스 추가 삭제
- 참고 : http://keycode.info/

## 과정
1. 해당키보드 키 눌렀을때 효과음 발생함수
2. audio 와 key 에 keyCode 일치하는 요소 담아둔다.
3. audio가 없다면 (!audio) 실행하지 않고. 아니면 audio.play();
4. 키 재입력 시간설정 연속재생 가능하도록 audio.currentTime = 0 
5. 효과종료시 playing 클래스 삭제 할수 있는 함수구성
6. transitionend 효과의 완료여부로 삭제 결정
 
## Search

### transitionend 
- transition이 완료된 이후에 발생한다. 
element.addEventListener('transitionend', (e) => {
  console.log('transition 완료');
  console.log(e.propertyName); // 어떤 속성이 끝났는지
});

element.addEventListener('transitionend', (e) => {
  if (e.propertyName !== 'transform') return;
  console.log('모든 효과가 끝났다고 간주');
});


### audio.currentTime = 0; 
- src,volume,currentTime audio 객체의 기본적인 속성
- 오디오 재생의 현재 위치를 0초로 이동함. 이로써 입력 후 다시입력하면 같은 소리를 재생시킬 수 있어 연속으로도 입력이 가능함

### Array.from() 
- 반환값 진짜 Array
- 모든 배열 메서드 사용 가능
- map, filter, find, reduce 등 사용 가능

### const keys = document.querySelectorAll('.key');
- 반환값 NodeList
- 유사 배열(Array-like) 객체
- length, 인덱스 접근 가능 (keys[0])
- 배열 메서드 일부만 사용 가능
- keys.forEach(...)   // 가능
- 간단한 반복 처리에 충분
