## 💡 part1-9 셀렉터를 이용해 CSS 코드 양 줄이기

### 🔹 태그 명
- 각 역할에 맞는 태그 쓰는게 좋다 (nav, footer 등등)

### 🔹 셀럭터 사용법
#### 클래스명 안에있는 태그에 스타일 적용
```css
.navbar li {
  display: inline-block;
}
```

#### 클래스명 안에있는 직계자식태그
```css
.navbar>li {
  display: inline-block;
}
```