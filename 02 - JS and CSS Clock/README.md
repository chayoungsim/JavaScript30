# JS and CSS Clock

### transform-origin : CSS transform 속성과 함께 사용되는 속성으로서, 회전 중심(원점·기준점)을 지정합니다.

* rotate(), skew() 등의 회전, 변형 속성을 사용하기 전에 기준점을 지정해 둡니다. 초기 값은 50% 50%으로 요소의 중심점이 됩니다.
* transform-origin의 속성 값은 백분율(%)과 키워드 중 하나로 지정할 수 있습니다.

### transition-timing-function : transition 의 진행 속도를 조절 할수 있다. IE10+ 지원
https://www.w3schools.com/csSref/css3_pr_transition-timing-function.asp

### new Date()
- new Date().toLocaleString(); // 2025. 12. 18. 오전 10:00:00
- new Date().toLocaleDateString(); // 2025. 12. 18
- new Date().toLocaleTimeString(); // 오전 10:00:00

- 

### setInterval(setDate,1000)

###  디지털 시계 표시 형식 개선 (0 붙이기)
- const formattedHours = String(hours).padStart(2, '0');
- String(hours) - 숫자를 문자열로 변환 이유: padStart()는 문자열 메서드이기 때문
- .padStart(2, '0') - 문자열의 길이가 2가 될 때까지 앞쪽에 '0'을 채움