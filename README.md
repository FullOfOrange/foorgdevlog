# Devlog

한달짜리로 간단하게 만들어서 사용할 블로그를 next.js 랑 golang 배우는 겸 해서 만들 예정

## 기초 설계

### Page

1. 내가 써놓은 글을 볼 수 있는 메인페이지 - 카드형식

2. md 파일을 업로드하는 페이지 - 내가 따로 로그인을 할 수 있는 장치가 필요함. 서버에 캐싱하기

   md파일을 html 로 변경하는 부분은 Client에서 하기.

3. 글 하나씩 볼 수 있는 페이지

기초 형태는 velog 또는 medium 을 따름. 카드 형식 그리드뷰에 적당히

### DB

글만 있으면 될 듯. mongo보다는 mariaDB 를 사용하는 방향으로 가자. 유저 정보는 일단 어드민을 위해서 테이블 하나만 만들기

글 - 제목, 생성 시각, 내용

글 뷰 - 글 뷰 개수, 좋아요 개수

유저 - 유저 네임 아이디 이메일 등등 ( 이것은 나중에 만들어도 됨.)