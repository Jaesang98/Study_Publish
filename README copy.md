## part 1-1 HTML 기초와 개발환경 셋팅

    1. HTML
        - 자료들이 어떻게 생겼나 구조로 표현하기 위한 언어
        - Hypertext Markup Language의 약자
        - Markup Language

    2. 세팅
        1) Extention
            - live server

## part 1-2 HTML 기본 태그로 글 작성해보기

    1. 기본적인 태그의 설명

## part 1-3 기본적인 웹페이지 스타일링

    1. 기본적인 스타일의 설명
        - 이미지 가운데 정렬
            display: block; margin-left: auto; margin-right: auto;

        - 폰트
            font-family

        - 자간조정
            letter-spacing

## part 1-4 CSS 파일 만들고 첨부하는 법

    1. css파일 만들어서 사용
        - Cascading Style Sheet (스타일 보관파일)

        - 셀렉터의 우선순위
            style="" (1000점)
            #id (100점)
            .class (10점)
            p (1점)

## part 1-5 웹레이아웃의 기초 : div를 이용한 네모네모 박스 디자인

    1. box에서 자주쓰는 스타일링
        - border: 4px solid black (두께, 선의 종류, 색)
        - display : block (가로행을 전부 차지한다)
            => 대부분 태그가 가지고있다

    2. inherit
        - 일부 스타일은 자동으로 부모에 적은 스타일링이 자식에게도 전달된다

## part 1-6 레이아웃 만들기 1 : 호환성 좋은 float

    1. 시작 전
        Wrapper or Container라는 셀렉터로 화면전체를 감싸는 박스를 하나 만들어두는게좋다

    2. float
        - 요소를 띄워서 배치시킴 (left or rigth)
        - float후에 적을 요소는 clear (left, right, both)를 사용함

## part 1-7 레이아웃 만들기 2 : 귀찮은 inline-block

    1. display
        - block : 한 행을 전부 차지
        - inline-block : 내 크기만큼 차지 (태그사이에 공백도 width를 포함함)
            => vertical-align 스타일을 저거로 했을 때 사용가능

    ************ inline-block 이거 쓰지말자 ************

## part 1-8 레이아웃 만들기 숙제 : Blog 글목록 만들기

    1. 숙제

## part 1-9 셀렉터를 이용해 CSS 코드 양 줄이기

    1. 태그 명
        각 역할에 맞는 태그 쓰는게 좋다 (nav, footer 등등)

    2. 셀럭터 사용법
        - 클래스명 태그
            => 클래스명 안에있는 태그에 스타일 적용

        - 클래스명>태그
            => 클래스명 안에있는 직계자식태그

    3. 스타일링 꿀팁
        text-decoration: none; 이렇게 하면 a태그 밑줄 없어짐

## part 1-10 배경 이쁘게 넣는 스킬들 & margin collapse

    1. 백그라운드 이미지 스타일링
        background-image: url(../img/shoes.jpg);
            => url 적용
            => ,사용해서 url더 적어주면 이미지가 겹침

        background-size: cover;
            => 사이즈를 알아서 잘 채워준다

        background-size: contain;
            => 배경짤리지 않도록한다

        background-repeat: no-repeat;
            => 이미지 반복 x

        background-position: center;
            => 이미지를 가운데부터 채운다

        filter: brightness(70%);
            => 필터 (대신 그안에 있는 요소 전부 필터가 먹힌다)

        background-attachmen
            => 스크롤될 때 배경이 신기하게 동작하게 만들 때 사용

    2. margin collapse
        => 두 요소의 테두리가 겹쳐있을 때 마진이 하나로 합쳐지는 현상

## part 1-11 position과 좌표 레이아웃 만들기

    1. position
        - position: relative; 후에 top bottom등을 주어 좌표이동이 가능
            => 이건 현재 공중에 쓴 상채

        - position: static;
            => 좌표이동 x

        - position: fixed;
            => 현재화면에서 고정 (스크롤 내릴때 메뉴 계속 보이는걸 생각하면될듯)

        - position: absolute
            => 내 부모 태그 기준으로 움직인다
                (대신 relative를 가진 부모만)

## part 1-12 position 숙제 & 반응형 width & box-sizing

    1. z-index
        - 높을수록 앞에온다
        - 비교대상 둘다 position 스타일링을 써야한다

    2. 반응형
        - 반응형은 대부분 %를 사용한다
        - max-width 등등

    3. padding, border포함 사이즈 측정하기
        - box-sizing: border-box;
            => 이게 좋은듯

        - box-sizing: content-box;
            => 요건 그대로 라는 뜻

    4. 브라우저마다의 호환성 있도록 하는 CSS
        - normalize.css
            => 각 브라우저마다 UI가 다르게 보이는것을 없애준다
            https://github.com/necolas/normalize.css/blob/master/normalize.css

## part 1-13 form & input

    1. form
        => 서버관련 태그

    2. input
        => 여러가지 타입이 있다

## part 1-14 form & input 숙제 : Contact Us 섹션 만들기

    1. 숙제하면서 깨달은점
        - border-radius는 꼭 써야하겟다
        - 재사용 클래스 스타일을 사용하자

## part 1-15 쓸데 많은 Table 레이아웃과 vertical-align속성

    1. table 사용 시 스타일링
        - table { border-collapse: collapse;}
            => 표 사이의 간격을 없애준다\

    2. 글자의 위 아래 크기 조정
        - vertical-align
            => inline/ inline-block일때사용
                (inline은 항상 옆으로 채워지는 폭과 너비가 없는 요소)

        - vertical-align에 여러가지 스타일링을 줄 수 있는데
            table같은경우에는 top middle bottom밖에 못준다

## part 1-16 Table 레이아웃 숙제 : Cart 페이지 만들기

    1. 셀렉터 태그:nth-child(2)
        => 셀렉터 밑에 있는 태그 중 2번쨰에 적용
            순서마다 스타일링을 줘야할 때 사용

    2. 테이블 열 합칠 때는 colapse

## part 1-17 pseudo-class로 인터랙티브 버튼 만들기

    1. pseudo-class
        - 상태에 따라서 스타일을 줄 수 있음

    2. 스타일링
        - 셀렉터:hover {} 마우스 갓다댔을때

        - 셀렉터:active 클릭했을 때

        - 셀렉터:focus 포커스됬을 때 (인풋 클릭 시 테두리 변할 때 사용)
        (순서는 h f a 순으로 적기)

        - 방문적 링크와 방문 후 링크는 link, visited 순으로 적용

## part 1-18 코드양이 줄어드는 class 작명법 (OOCSS, BEM)

    1. Object Oriented CSS
        - 유틸리티 스타일링
        - CSS작성 시 뼈대와 살점을 만들어 편리하고 유지보수 하기 좋게 만든다

    2. BEM
        - Block_Element--Modifier 의 약자
        - 클래스명 작성할 때 창의력이 딸리는경우에 사용하는 기법
        - class="덩어리이름__역할--세부특징"
            => 대부분 근데 덩어리-역할 이런식으로함

---

## part 2-1 HTML CSS 웹폰트 넣는 법과 안티앨리어싱

    1. @font-face
        - 폰트파일을 css에서 사용가능하게 등록
        - ttf는 너무 크니까 웹 모드는 woff를 사용하자
        - 한글폰트는 엄청 크니까 적게사용하자

    2. font-weight
        - 그냥 주면 안이쁘니까 font-family에 font-weight를 작성해주자
        - 혹은 각 텍스트에 주는것도 좋음

    3. 구글폰트
        - fonts.google.com

    4. 폰트를 줬을 떄 깨지는 현상
        - transform: rotate(0.03deg) 정도를 주면 깨짐이 덜하다.

## part 2-2 레이아웃 만들기 3 : 편리한 Flexbox

    1. flex
        - display : flex; 를 하면 쉽게 요소를 가로에 둘 수 있다

    2. justfy-content
        - flex를 사용한 요소에서 사용가능
        - center(가운데), flex-end(오른쪽), flex-start(왼쪽), space-between(사이간격)

    3. flex-direction
        - row, colum을 사용하여 가로 세로 배치가 가능하다

    4. flex-wrap
        - 넘치면 밑으로가기

    5. align-items
        - flex부모 밑의 요소 위아래로 상하정렬이 가능

    6. flex-grow
        - 배수만큼 칸을 차지하는건데 대부분 헤더의 로고랑 메뉴바 사이 간격 벌릴 때 사용

## part 2-3 HTML CSS 코드짤 때 유용한 Emmet 그리고 부가기능들

    1. 재밌는 부가기능
        - Power Mode, Emmet

## part 2-4 head 태그에 들어갈 내용 정리

    1. head
        - <link href="css/main.css" rel="stylesheet">
        - <title>네이버입니다</title>
        - <meta charset="UTF-8">
            => 인코딩 형식

        - 사이트의 검색 결과 화면에 뜨는 글귀
            <meta name="description" content="html 잘하는 코딩애플입니다.">
                => 구글 검색시 파란 제목으로 뜨는 글귀
            <meta name="keywords" content="HTML,CSS,JavaScript,자바스크립트,코딩">
                => 검색에 도움을 주는 키워드

        - 사이트 초기 zoom 레벨이나 폭
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
            => initial-scale=1 이 부분은 접속시의 화면 줌레벨

        - facebook이 만든 og 라는 메타태그
        <meta property="og:image" content="/이미지경로.jpg">
        <meta property="og:description" content="사이트설명">
        <meta property="og:title" content="사이트제목">

        - 아이콘이
        <link rel="icon" href="아이콘경로.ico" type="image/x-icon">

## part 2-5 반응형 레이아웃 만들기

    1. 단위
        - vw : 브라우저 폭에 비례
        - vh : 브라우저 높이에 비례
        - rem : 기본 폰트사이즈에 비례 (1rem = 16px)
            => 디자인할떄 px외우기 귀찮을 때 사용
                이전에는 폰트 확대하는 기능 때문에 사용을 했었다

    2. media query
        @media screen and (max-width:1200px)
            => 1200px 이하일때 이 스타일 적용

        * 1200px (테블릿) 768px 576px(모바일)

## part 2-6 반응형 레이아웃 숙제 : 가로정렬 레이아웃

    1. 하면서 꺠달은점
        - height는 웬만하면 auto로
        - flex-direction 사용 많이해보기

## part 2-7 크롬 개발자 도구와 IE호환성 잡기

    1. 개발자 도구 사용하기
        - 주황색 : margin
        - 파랑색 : content
        - 초록색 : padding

    2. 호환성
        익스플로러 X 버전 이하에서만 적용할 수 있는 CSS파일을 첨부
        <!--[if lt IE 9]>
            <link rel="stylesheet" type="text/css" href="css/ie8.css" />
        <![endif]-->

## part 2-8 Font Awesome 아이콘 넣기

    1. cdn
        - <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css" integrity="sha512-Kc323vGBEqzTmouAECnVceyQqyqdsSiqLQISBL29aUW4U/M7pSPA/gEUZQqv1cwx4OnYxTxve5UMg5GT6L4JJg==" crossorigin="anonymous" referrerpolicy="no-referrer" />

        -https://fontawesome.com/icons

        => 크기는 폰트사이즈를 적용하면된다

## part 2-9 Transition 속성으로 CSS 애니메이션 구현하기

    1. transition
        - transition: 스타일 초s : 스타일이 변하면 초만큼 서서히 변경한다
            => 스타일은 all로 줘도된다

    2. transition-timing-function
        - 점점 빠르게 or 점점 느리게 스타일 변화를 줄 수 있음

## part 2-10 Transition 숙제 : 상품진열 레이아웃과 애니메이션

    1. .test:hover .test2{}
        => 이런식으로 hover 시 다른 클래스에 이벤트가 발생을 일으킬 수 있다.

## part 2-11 Portfolio 실습 1 : Landing Page

    1. 하면서 느낀점
        - box-size 잘 체크하기 padding 잘 주기

    2. 새롭게 안거
        - Linear Gradient (한쪽에서 다른한쪽으로 색상 변화)
        - Radial Gradient (중심에서부터 바깥쪽으로 색상이 변화)

## part 2-12 Bootstrap 설치와 사용법

    1. 유틸리티 쓸만한게 많아보임

## part 2-13 Bootstrap Grid 레이아웃

    1. 반응형 레이아웃
        - row col
            => col-숫자를 통해서 간격을 나눌 수 있음 (row가 최대12쪼갬)

        - col-반응형-숫자
            => 반응형으로 저 숫자만큼 쪼개며 스타일링을 적용한다
                (xl = 1200px) (lg = 992px) (md = 768px) (sm = 576px)

        - order-숫자
            => 요소들의 순서를 정할 수 있음
                (order-반응형-숫자) 이런것도 가능

    2. 반응형 만들 때 팁
        - 부트스트랩을 쓸 때는 모바일 레이아웃먼저 만들면 쉽다

## part 2-14 Bootstrap Grid 레이아웃 숙제 해설

    1. 반응형에 사용하기 좋은 셀렉터는 일단 나중에 내꺼를 만든다고 하더라도
        많이 사용해보고 하자

## part 2-15 CSS 덮어쓰기 잘하는 법 & 어떤 코드가 좋은 코드인가요

    1. CSS덮는법
        - 그냥 같은 클래스명 하단에 쓰기
            => 더 밑에 작성된게 적용이 된다 (가끔 안될 수 있음)

        - 우선순위 높이기
            => 아이디 적기 oor !important; 를 적용한다 (우선순위가 제일높음)

        - specificity 높이기
            => 위에 부모 클래스나 자식클래스나 이런거를 하나 더 덮는다

    2. 좋은코드
        - 수정관리가 쉬움
        - 확장성이 좋음
        - 양이 적음

    3. 부트스트랩
        - 웬만하면 수정을 안한다
        - 클래스를 추가하는게 좋다

## part 2-16 Portfolio 실습 2 : SNS Profile

    1. 하다가 귀찮아서 안함

## part 2-17 Portfolio 실습 2 : SNS Profile (해설편)

    1. 부투스트랩 잘 찾아보자

---

## part 3-1 약간 쓸데없는 Pseudo-element

    1. Pseudo-element
        - .클래스::수도클래스
            => 내부의 일부분만 스타일을 줄 때 사용

    2. 자주쓰는 수도 클래스
        - first-letter , first-line
            => 첫번째 글자, 첫번째 줄

        - after
            => 내부 맨 뒤에 뭔가 추가할 때 사용

        -  before
            => 내부 맨 앞에 뭔가 추가할 때 사용

## part 3-2 딥다크한 어둠의 공간 Shadow DOM

    1. 숨겨진 요소 보는 법
        - 개발자 도구 => 설정 => Preference => Element => show user agent shadow DOM 체크하기
            => 이렇게 숨겨진 요소들을 shadow DOM이라고 함

    2. -webkit-
        - 크롬 사파리 Edge 에서만 적용되는 스타일

    3. appearance: none
        - 브라우저 기본 CSS 안보이게

## part 3-3 만든 사이트 발행하기

    1. 사이트 발행법
        - 깃허브
        -  cafe24.com Filezilla 사용

## part 3-4 쉽게 배우는 Sass 기초 1편 : 셋팅

    1. 세팅
        1) live sass com 설치
        2) scss 파일 만든 후 아래 watching 누르면 알아서 변환됨
            (MAP은 디버깅용)

    2.  SASS 스타일 변수 생성
        - $변수 : 스타일
            => px같은 숫자는 연산 가능함

    3. CSS 스타일 변수 생성
        - :root { --변수명: 스타일 }선운 후  var(--변수명)를 써야함
        - 연산 : ex) calc(숫자 - 숫자)

## part 3-5 쉽게 배우는 Sass 2편 : 핵심문법

    1. SCSS 와 SASS차이점
        - SCSS는 CSS처럼 {}를 쓰지만 SASS는 괄호를 안적어도된다

    2. nesting 문법
        - .클래스 { .클래스{} } 이런게 가능함

    3. @extend
        하나의 임시클래스에 이걸 박아놓은 다음에
        이거를 @extent 임시클래스 이렇게 쓰면 임시클래스이 값들을 쓸 수 있다
            => %임시클래스

## part 3-6 쉽게 배우는 Sass 3편 : Mixin, use 등

    1. mixin
        - 스타일의 값을 파리미터로
            @minxin 함수명 ($파라미터1, $파라미터2) { 스타일 } 적은 후
            @include 함수명 ($파라미터1, $파라미터2) 이렇게 적으면 된다

        - 스타일을 파라미터로
            mixin에서는 #{ $파리미터 } : -1px;
            @include 함수명 (파라미터1, 파라미터2)
                => 이렇게 적용도 가능

    2. use
        - import같은거임
        - @use '파일명'; 이렇게 적으면 됨
        - import는 css에서도 된다
        - 다른 파일의 변수를 쓰려면 파일명.$변수 이렇게 써야한다


    3. 자동 컴파일 되는 scss
        - _파일명.scss 이렇게 하면 된다

## part 3-7 쉽게 배우는 Sass : 숙제 해설

    1. 꿀팁
        - 먼저 기본 css를 짜보고 축약을 해보는 연습을 하자

## part 3-8 HTML video, audio 다루기

    1. 비디오
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

    2. 오디오
        - <audio>를 사용함

        - controls (요거는 필수)

        - muted (음소거된 상태)

        - autoplay 말고 비디오처럼 sorce태그 나 다른 스타일링이 가능

## part 3-9 transform & animation 으로 매끄러운 애니메이션 만들기

    1. transform
        - rotate(10deg); translate(10px, 20px); scale(2); skew(30deg);
            => rotate는 회전, translate는 좌표이동, scale은 확대축소, skew는 비틀기 (두개이상도 쓸 수 있음)

    2. @keyframes
        - @keyframes 함수 {0% {transform: 스타일링} 50% {transform: 스타일링}} 이렇게 사용 후
            animation-name : 함수; animation-duration: 1s 이런식으로 사용

    3.margin으로 움직인 것과 transform으로 움직였을 떄 차이점
        - 변경이 transform가 더 빠름
        - 렌더트리 - 레이아웃 - 페인트 - 컴포사이트 이 순으로 화면이 그려지는데
            margin으로 변경 시 레이아웃부터 다시그리지만 transform으로 변경 시 컴포사이트부터 바꾸기 때문에 부담이 덜하다
        - js html css 등의 기능은 웹 브라우저의 한 스레드에서만 사용하지만 애니매이션은 다른 스레드에서 사용함

    4. 성능 빠르게 잡는 법
        - will-change (바뀔 내용을 미리 렌더링해주는 속성)
            => https://dev.opera.com/articles/ko/css-will-change-property/
                (뭔가 이상하게 버벅일 때만 쓰고 애니메이션이 스무스하게 잘 된다면 쓸 이유는 없음
                이상하게 많이 쓰면 브라우저 자체가 더 느려질 수 있다.)

        - 하드웨어 가속
            => 애니메이션이 너무 많아 CPU만으로 전부 연산이 불가능하다면 GPU의 도움을 받을 수도 있음
                (transform: translate3d(0, 0, 0);)

## part 3-10 transform & animation 숙제 해설 (움직이는 메뉴)

    1. 숙제

## part 3-11 레이아웃 만들기 4 : CSS Grid 레이아웃
