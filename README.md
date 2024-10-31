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