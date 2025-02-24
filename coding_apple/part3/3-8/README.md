## 💡 part3-8 HTML video, audio 다루기

### 🔹 비디오

- <video>에는 여러 형식이 있기 때문에 안에 source태그와 그곳안에 타입을 적어주는게 좋다
  => 호환성을 챙길 수 있음 (각 브라우저마다 지원하는 확장자가 다르기 때문)
  그래서 여러 소스 태그를 박아놓는게 좋다

- video태그에는 controls, autoplay muted 사용이가능
  (muted는 크롬 브라우저 정책때문에)

- preload="none"
  => 미리다운x

- preload="auto"
  => 미리다운o

- preload="metadata"
  => 미리다운 적당히

- poster="경로" (썸네일)

- loop (무한재생)

### 🔹 오디오

- <audio>를 사용함

- controls (요거는 필수)

- muted (음소거된 상태)

- autoplay 말고 비디오처럼 sorce태그 나 다른 스타일링이 가능
