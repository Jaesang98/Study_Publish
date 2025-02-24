## 💡 part3-11 레이아웃 만들기 4 : CSS Grid 레이아웃

### 🔹 Grid

- 격자를 만드는 레이아웃

```html
<div class="grid-container">
  <div></div>
</div>
```

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr; /*가로4칸*/
  grid-template-rows: 100px 100px 100px; /*세로3칸*/
  grid-gap: 10px;
}
```

### 🔹 예시

```css
display: grid;
grid-template-columns: 1fr 1fr 1fr 1fr;
grid-template-columns: 100px 100px 100px 100px;
grid-template-rows: 100px 100px 100px;
grid-template-areas: "헤더 헤더 헤더 헤더";
grid-column: 1/4;
grid-row: 1/3;
```
