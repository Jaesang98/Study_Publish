## 💡 part2-2 레이아웃 만들기 3 : 편리한 Flexbox

### 🔹 Flexbox

```css
/* display: flex; 를 하면 쉽게 요소를 가로에 둘 수 있다 */
display: flex;

/* flex를 사용한 요소에서 사용 가능 */
justify-content: center; /* 가운데 정렬 */
justify-content: flex-end; /* 오른쪽 정렬 */
justify-content: flex-start; /* 왼쪽 정렬 */
justify-content: space-between; /* 사이 간격 정렬 */

/* row, column을 사용하여 가로 세로 배치가 가능하다 */
flex-direction: row;
flex-direction: column;

/* 넘치면 밑으로 가기 */
flex-wrap: wrap;

/* flex 부모 밑의 요소를 위아래로 정렬 가능 */
align-items: center;
align-items: flex-start;
align-items: flex-end;

/* 배수만큼 칸을 차지하는데, 주로 헤더의 로고와 메뉴바 사이 간격을 벌릴 때 사용 */
flex-grow: 1;
```
