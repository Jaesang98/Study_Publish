## 💡 part1-10 배경 이쁘게 넣는 스킬들 & margin collapse

### 🔹 백그라운드 이미지 스타일링
```css
background-image: url(../img/shoes.jpg);
/* 배경 이미지 적용 */
/* 여러 개의 이미지 사용 시 쉼표(,)로 구분하여 겹쳐서 표현 가능 */

background-size: cover;
/* 요소의 크기에 맞춰 배경을 꽉 채움 */
/* 비율이 유지되며 잘릴 수도 있음 */

background-size: contain;
/* 배경이 잘리지 않도록 조절 */
/* 요소 크기 안에서 비율을 유지하며 맞춤 */

background-repeat: no-repeat;
/* 이미지 반복 없이 한 번만 표시 */

background-position: center;
/* 이미지를 요소의 가운데 정렬하여 배치 */

filter: brightness(70%);
/* 밝기 조절 (단, 내부 요소도 함께 적용됨) */

background-attachment: fixed;
/* 스크롤 시 배경을 고정하거나 다양한 방식으로 동작하도록 설정 */

```

### 🔹 margin collapse
- 두 요소의 테두리가 겹쳐있을 때 마진이 하나로 합쳐지는 현상
- 테두리 안붙게 하면된다