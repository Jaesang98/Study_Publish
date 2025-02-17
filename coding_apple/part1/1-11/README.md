## 💡 part1-11 position과 좌표 레이아웃 만들기

### 🔹 position
```css
position: relative;
/* 현재 요소를 기준으로 top, bottom, left, right 값을 사용하여 이동 가능 */
/* 원래 위치에서 떠 있는 상태 (공중에 있는 느낌) */

position: static;
/* 기본값 (위치 이동 불가) */
/* top, bottom, left, right 적용 불가능 */

position: fixed;
/* 뷰포트를 기준으로 고정 (스크롤해도 움직이지 않음) */
/* 예: 항상 보이는 메뉴바 */

position: absolute;
/* 부모 요소를 기준으로 이동 (단, 부모가 position: relative를 가져야 함) */
/* relative가 없는 경우 body를 기준으로 배치됨 */

```