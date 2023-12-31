# Petagram
### Tools
#### 설계
- Figma
- draw.io
#### 구현
- sts3
- Apache Tomcat 9
#### 협업
- Notion
  - https://www.notion.so/545ee808b70049b3842131f25d02f63d

### 역할
|기술|기능|
|:---:|---|
|Frontend|전체 CSS, 게시글 상세 페이지, 동물병원 페이지|
|Backend|게시글 상세 페이지, 동물병원 페이지|
|-|전체 코드 병합|

### 언어/프레임워크
|기술|언어/프레임워크|
|---|---|
|Frontend|HTML, CSS, JavaScript, jQuery, JSP|
|Backend|Java 11, Spring, Mybatis, MySQL|

### Open API
- NCP
  - Naver Map API(Web Dynamic Map API)
    - https://guide.ncloud-docs.com/docs/ko/maps-web-sdk
- 공공데이터
  - 경기도 동물병원 현황
    - https://www.data.go.kr/data/15057867/openapi.do

## 목차
1. [설계 UI](#설계-ui)
2. [Sequence Diagram](#sequence-diagram)
3. [ERD](#erd)
4. [API](#api)
5. [구현 페이지 상세 기능](#구현-페이지-상세-기능)
6. [결과 UI](#결과-ui)

## 설계
### 설계 UI
- https://www.figma.com/file/Aw0wHIoiv1QpA2iLDoPccw/Petagram?type=design&node-id=13-148&mode=design&t=kj88sPhJOeWiYudG-0

### Sequence Diagram
- https://gitmind.com/app/docs/fpml4zt9

![Sequence Diagram](https://github.com/meizzi04/Petagram/assets/86556226/fe2e9f62-23b0-4a81-9c3f-c4416dfa4574)

### ERD
![ERD](https://github.com/meizzi04/Petagram/assets/86556226/83f1160a-e687-42dd-a5be-c13f8aba9127)

## 구현
### API
- https://harmonious-canvas-592.notion.site/API-1e967a8c4ebb470386151be3141cbbc6?pvs=4

### 구현 페이지 상세 기능
- 게시글 상세 페이지
  - 게시글 Body
    - 제목, 내용, 작성자, 작성자, 작성날짜
  - 게시글 수정
    - 수정 권한 검사(작성자만)
    - 게시글 수정 페이지로 이동
  - 게시글 삭제
    - 삭제 권한 검사(작성자만)
    - 삭제 후 전체 게시글 페이지로 이동
  - 좋아요
    - 좋아요 수 기능
    - 한 게시물당 한번씩 추천 가능하도록 제한
  - 링크 복사
    - 해당 페이지 URL 복사
  - 댓글
    - 댓글 등록 및 삭제
    - 댓글 입력하지 않고 등록하면 팝업창 띄우기  
- 동물병원 페이지
  - Naver Map API 활용
    - 특정 동물병원 클릭 시 해당 병원에 대한 위치와 상세 주소 출력
  - 공공데이터 API 활용
    - 경기도 동물병원 리스트 DB 저장
    - 입력한 주소에 해당하는 모든 동물병원 출력

### 결과 UI
- 로그인 페이지
![Login](https://github.com/meizzi04/Petagram/assets/86556226/7b1acbfc-8b53-4245-b3be-bfc027ad0095)
- 회원가입 페이지
![Join](https://github.com/meizzi04/Petagram/assets/86556226/ff4d3bbf-0ce1-406c-9236-e32f34198f58)
- 홈페이지
![Home](https://github.com/meizzi04/Petagram/assets/86556226/fcd9efc7-a102-43f2-b015-c32627aacb01)
- 게시글 작성 페이지
![CreatePost](https://github.com/meizzi04/Petagram/assets/86556226/fd7b46ea-3ad1-4555-be2f-94394a16e590)
- 게시글 수정 페이지
![UpdatePost](https://github.com/meizzi04/Petagram/assets/86556226/3aaa33b2-f9cc-4063-950e-79371e2abab3)
- 전체 게시글 페이지
![ReadPostAll](https://github.com/meizzi04/Petagram/assets/86556226/bba8fbdc-fbf1-4a54-8764-f17657d72e23)
- 게시글 상세 페이지
![ReadPostOne](https://github.com/meizzi04/Petagram/assets/86556226/c6c8913d-8fc9-4fe3-a9af-f8a177b562f6)
- 마이페이지
![Mypage](https://github.com/meizzi04/Petagram/assets/86556226/17144355-c23f-4abe-9063-3b078d099937)
- 정보 수정 페이지
![ChangeInfo](https://github.com/meizzi04/Petagram/assets/86556226/0855dd03-bd6d-4275-84b8-0754c4a95b22)
- 동물병원 페이지
![HospitalInfo](https://github.com/meizzi04/Petagram/assets/86556226/28d5e278-f4ac-4e89-80c0-3661686f1f7d)
- 공지사항 페이지
![Inform](https://github.com/meizzi04/Petagram/assets/86556226/3ac8a8d1-9af9-44d6-ae4f-ba7d8845d49e)
