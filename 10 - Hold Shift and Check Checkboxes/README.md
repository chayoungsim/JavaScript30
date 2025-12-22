## Hold Shift check checkboxs

Shift 키를 누른 상태에서 체크박스를 클릭하면, 이전에 선택한 체크박스부터 현재 체크박스까지 한 번에 선택되도록 만드는 로직입니다. 이메일 목록 등에서 자주 사용하는 다중 선택 UX를 구현한 예시입니다.

### inBetween의 역할
이전 체크박스(lastChecked)와 현재 클릭한 체크박스(this) 사이에 있는지 여부를 나타내는 상태값입니다.
- true → 범위 안
- false → 범위 밖