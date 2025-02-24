## 💡 part3-9 transform & animation 으로 매끄러운 애니메이션 만들기

### 🔹 transform

- rotate(10deg); translate(10px, 20px); scale(2); skew(30deg);
  => rotate는 회전, translate는 좌표이동, scale은 확대축소, skew는 비틀기 (두개이상도 쓸 수 있음)

### 🔹 @keyframes

- @keyframes 함수 {0% {transform: 스타일링} 50% {transform: 스타일링}} 이렇게 사용 후
  animation-name : 함수; animation-duration: 1s 이런식으로 사용

### 🔹 margin으로 움직인 것과 transform으로 움직였을 떄 차이점

- 변경이 transform가 더 빠름
- 렌더트리 - 레이아웃 - 페인트 - 컴포사이트 이 순으로 화면이 그려지는데
  margin으로 변경 시 레이아웃부터 다시그리지만 transform으로 변경 시 컴포사이트부터 바꾸기 때문에 부담이 덜하다
- js html css 등의 기능은 웹 브라우저의 한 스레드에서만 사용하지만 애니매이션은 다른 스레드에서 사용함

### 🔹 성능 빠르게 잡는 법

- will-change (바뀔 내용을 미리 렌더링해주는 속성)
  => https://dev.opera.com/articles/ko/css-will-change-property/
  (뭔가 이상하게 버벅일 때만 쓰고 애니메이션이 스무스하게 잘 된다면 쓸 이유는 없음
  이상하게 많이 쓰면 브라우저 자체가 더 느려질 수 있다.)

- 하드웨어 가속
  => 애니메이션이 너무 많아 CPU만으로 전부 연산이 불가능하다면 GPU의 도움을 받을 수도 있음
  (transform: translate3d(0, 0, 0);)
