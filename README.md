# Python_Study_2

1. Static file이란? Javascript, CSS, Image 처럼 웹 페이지에서 사용하려고 미리 준비해둔 정적 파일.
파일 자체가 고정되어있어 개발자가 바꾸지 않는 한Static 파일들은 변하지 않는다.

2. Layout 상속을 하는 이유? 모든 html에 하나하나 쓰기도 불편할 뿐더러, 한번 수정사항이 생기면 각각 들어가서 모든 코드를 바꿔주어야 하는 일이 발생.
그래서 layout상속을 이용해서 불필요한 노동을 줄임.

3. form.html : Form을 입력하면 Form의 내용을 볼 수 있음

4. CSRF란?
사용자가 자신의 의지와는 무관하게 공격자가 의도한 행위(수정, 삭제, 등록, 등등)을 특정 웹사이트에 요청하게 하는 공격.
장고 1,2버전부처 이러한 CSRF취약점을 막기 위해 CSRF토큰을 기본적으로 제공.
이를 사용하려면 모든 POST방식의 폼 전송에는 hidde필드로 세션에 따른 임의 키 값을 전송하며, 해당 키 값이 유효한지 매번 확인.
쉽게 말해 보안을 위해서 사용.

5. Get은 가져온다는 개념이고, POST는 수행한다는 개념
Get은 게시판에서 글의 내용에 대한 목록을 보여주는 경우나, 글의 내용을 보는데 사용
Ex) 글 목록 조화, 각각의 글 조회 .
POST는 서버상의 데이터 값이나 상태를 바꾸기 위해서 사용. 글쓰기를 예를 들면 글의 내용을 저장하고, 수정할 때 사용
  Ex) 글쓰기, 글 수정
