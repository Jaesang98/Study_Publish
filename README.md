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