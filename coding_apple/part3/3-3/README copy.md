html css js 밖에 없는 사이트를 발행하려면 방법 2개가 있습니다.

1. Github Pages 이용법 (그냥 누구에게 보여줄 포트폴리오가 빠르게 필요할 때)

2. 일반 유료 호스팅 이용법

이외엔 요즘 Vercel, Netlify 이런 곳들도 빠르게 html css js를 배포할 수 있습니다.

1. Github Pages 를 이용해 쉽게 사이트를 띄워보도록 합시다.

1) github.com 에서 가입하시고 로그인합니다.

2) 우측 상단 + 버튼을 눌러 New repository를 만들어줍니다. 이제부터 중요한 내용이 출현합니다.

3-1) 만들 때 repository name 섹션엔 여러분 왼쪽에 뜨는 아이디.github.io로 적어주시면 됩니다. 저의 경우엔 yogoho210.github.io가 되겠네요. 임의로 다른 이름으로 적으시면 실패합니다.

3-2) 마지막에 README 파일생성란에 체크해주시면 됩니다. 그리고 밑에있는 초록버튼을 눌러줍니다.

4. 그럼 요런 화면이 나오는데 여기다가 여러분의 html,css,js 파일을 그대로 업로드하시면 됩니다. 그냥 여기다가 원하는 파일들을 전부 한번에 드래그 앤 드롭하시면 됩니다.

5. 업로드가 잘 되었으면 사이트 발행 성공이고

이제 여러분아이디.github.io 라는 주소로 접속하면 여러분 사이트가 뜹니다.

안뜨면 5~10분 기다려보거나 여러분아이디.github.io/index.html로 접속해봅시다.

6. 원래 웹사이트들은 기본 주소로 들어가면 index.html 이라는 파일을 자동으로 보여주는데

내가 다른 html 파일을 열람하고 싶다면 html 파일의 경로를 적어주시면 되겠습니다.

예를 들면 layout.html 보여주고 싶으면 여러분아이디.github.io/layout.html 로 접속하면 되는데

이제 집에가서 부모님께 자랑해봅시다.

7. HTML/CSS 변경사항이 있어서 파일을 업데이트 했다면 업데이트한 파일을 그대로 아까랑 똑같이 드래그합시다.

8. 문제가 생겼다면 repository를 삭제후 다시 만들면 됩니다.

9. 아마 설정 들어가면 내가 구매한 도메인도 등록할 수 있습니다.

2) 일반 호스팅을 이용해서 프로젝트를 발행해보도록 합시다.

1. 가장 많은 유저가 있는 cafe24.com 으로 가셔서 웹호스팅을 아무거나 제일 싼거 선택한 후 결제합니다.

보통 PHP + 리눅스 환경을 제공합니다.

설치비 5천원에 월500원입니다. (SSD어쩌구 추천)

1-1) 결제하시다보면 DB아이디나 비밀번호 설정부분도 있을 텐데 까먹지맙시다.

2. 결제마치시면 cafe24.com에서 찾을 수 있는 관리자 화면으로 들어갑니다. 로그인 하신 후에 "나의 서비스 관리" 이런거 찾아서 누르시면 될걸요?

3. 여러분의 '서비스 접속정보'를 누르셔서 FTP 접속정보를 확인합니다.

앞으로 이 주소로 접속해서 여러분의 HTML 파일들을 업로드할겁니다.

그럼 어떻게 FTP 주소로 접속하냐고요?

4. FTP 프로그램을 이용합니다. 알FTP 혹은 Filezilla 라는 프로그램을 다운받아 설치합니다. 사람들 많이 쓰는 Filezilla를 씁시다.

5. Filezilla를 실행시키면 빈칸이 나옵니다. 여기에 아까 관리자페이지에서 확인한

호스트(FTP 주소)

사용자명(FTP 아이디)

비번(아마도 DB비번)

그리고 21이라는 포트 번호를 적어넣습니다.

그리고 연결을 누르시면 여러분 사이트가 하단에 뿅하고 뜹니다.

6. 이것이 바로 여러분의 호스팅 공간에 담긴 파일들입니다.

다른건 건들 필요 없고 www 폴더 안으로 접속하셔서 아까처럼 html,css 파일들 다 드래그앤 드롭해서 업로드하시면 발행이 끝납니다.

끝

7. 그럼 여러분 사이트 접속 주소가 어떻게 되냐고요? 관리자 페이지 여기에 아마 나와있을겁니다.

아마 어쩌구.cafe24.com 일걸요?

8. 나만의 도메인을 설정하고 싶다면

8-1) 도메인을 구입합니다. 개인적으로 name.com이 가장 저렴해보입니다.

8-2) 어떤 사이트에서 도메인을 사든 간에 결제까지 하시면 도메인 관리페이지가 활성화됩니다. 여기선 name.com이라고 합시다.

8-3) name.com 도메인 관리페이지에서 네임서버(NS) 등록하기 페이지가 있는데 거기서 네임서버들을 cafe24 네임서버로 전부 바꾸어줍니다.

cafe24 네임서버가 어딨냐고요? cafe24 관리자 페이지 어딘가에 숨겨져있습니다.

8-3) cafe24 관리자 페이지로 돌아옵니다. '도메인 연결관리' 들어가셔서 아까 샀던 도메인을 등록하시면 됩니다. 4시간 정도 기다리면 그 도메인으로 접속가능합니다.

끝입니다.

9. 여러개 html 페이지가 있는데 각각 어떻게 접속하나요?

- 브라우저 주소창에 URL을 잘 써주시면 됩니다.

여러분도메인.com/index.html

여러분도메인.com/layout.html

이렇게 경로를 / 기호로 잘 적어주면 잘 접속가능
