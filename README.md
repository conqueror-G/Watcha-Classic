#  Watcha Classic
- Front: 김민석, 김은경, 이현범
- Back: 이태권, 박민하
![image](https://user-images.githubusercontent.com/50426259/176836350-67dbc6fa-eee8-4f0e-b675-d9da0865a350.png)
[시현 영상 보러가기](https://scrawny-opera-4c6.notion.site/ded2dbffac2140609d15bc3877219332)

<br>

## 프로젝트 소개
SNS와 평정 데이터를 활용한 클래식 영화 백과사전 사이트

<br>

## 사용기술 스택
- Front-end: <img src="https://img.shields.io/badge/html5-E34F26?style=flat-square&logo=html5&logoColor=white"/> <img src="https://img.shields.io/badge/Sass-CC6699?style=flat-square&logo=Sass&logoColor=white"/> <img src="https://img.shields.io/badge/javascript-F7DF1E?style=flat-square&logo=javascript&logoColor=white"/> <img src="https://img.shields.io/badge/react-61DAFB?style=flat-square&logo=react&logoColor=white"/> <img src="https://img.shields.io/badge/ReactRouter-CA4245?style=flat-square&logo=ReactRouter&logoColor=white"/>
- Back-end: <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"/> <img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=Django&logoColor=white"/> <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white"/>

<br>

## Front-end
| 역할 | 이름 |
|---|:---:|
| 로그인/회원가입 , 유저 프로필 페이지 | 이현범 |
| 정규 표현식을 활용한 로그인/회원가입 유효성 검사 | 이현범|
| 유저 프로필 목록 요청 | 이현범 |
| 메인 페이지/푸터/보고 싶어요 페이지 | 김은경 |
| 영화 목록 이미지 슬라이드 구현 | 김은경 |
| 보고 싶어요 목록 요청 | 김은경 |
| 상세 페이지 | 김민석 |
| 스켈레톤 UI, 보고 싶어요 UI, 코멘트 UI, 평가 별점 UI | 김민석 |

## Back-end
| 역할 | 이름 |
|---|:---:|
| 데이터 모델링 | 이태권 |
| 메인 페이지/프로필 페이지/보고 싶어요 API 구현 | 이태권 |
| 보고 싶어요 생성/삭제 기능 구현 | 이태권 |
| CSV | 박민하 |
| 로그인/회원가입 유효성 검사 | 박민하 |
| 로그인/회원가입/보고 싶어요 페이지 API 구현 | 박민하 |

## Front-end 필수구현 기능
> ### 1. 회원가입 / 로그인 페이지
  - 유효성 검사, back-end API 통신
  - Nav 버튼 클릭 시 로그인 / 회원가입 모달창 오픈

> ### 2. 메인 페이지
  - 라이브러리 없이 이미지 슬라이드 구현
  - 3개의 API 한 페이지에 받아오기
  - Advanced Router 사용하여 각각의 목록 클릭시 path parameter id 값 불러오기

> ### 3. 상세 페이지
  - 스켈레톤, 평가 별점, 보고싶어요 댓글 UI 구현
  - <보고싶어요> 버튼 클릭 시 보고싶어요 페이지로 데이터 전송

> ### 4. 프로필 페이지
  - 회원정보 보여주기
  - <보고싶어요> 담긴 갯수 보여주기 
 
> ### 5. 보고싶어요 페이지
  - 메인 페이지의 컴포넌트 재사용
  - 사용자가 보고싶어요 기능 사용한 데이터 받아오기

<br>

## :: 담당 구현 목표
1. (팀) 상세 페이지 레이아웃
2. (팀) 보고싶어요 UI
3. (팀) 평가하기 UI
4. (팀) 코멘트 UI
5. (개인) 상세 페이지 스켈레톤 UI

## :: 구현 사항 설명
1. (팀) 상세 페이지 레이아웃
- 반응형 웹 페이지를 추가 구현할 것을 생각하면서 작성했습니다.
![Uploading 상세페이지 레이아웃.gif…]()
2. (팀) 보고싶어요 UI
- 클릭하면 아이콘이 반시계 방향으로 45도 회전하고 핑크색 북 마크 아이콘으로 업데이트 됩니다.
- 클릭하면 코멘트를 달 수 있는 카드가 업데이트 됩니다.
- 클릭하면 아이콘이 반시계 방향으로 45도 회전하고 핑크색 북 마크 아이콘으로 업데이트 됩니다.
- 클릭하면 보고싶어요 요청이 백앤드 서버로 전송되고, 프로필 페이지와 보고싶어요 페이지로 응답해줍니다.
- 해제하면 아이콘이 시계 방향으로 45도 회전해서 원래 아이콘으로 돌아옵니다.
- 해제하면 삭제 요청이 백앤드 서버로 전송되고, 프로필 페이지와 보고싶어요 페이지에서도 응답 받으며, 삭제됩니다.
![보고싶어요 버튼](https://user-images.githubusercontent.com/90183279/177061825-df7fd669-5888-4c72-95ad-4b04ae07ac58.gif)
3. (팀) 평가하기 UI
- 마우스 오버를 하면 별이 체워지고, 클릭하면 별이 저장됩니다.
- 백엔드 서버와의 전송/응답은 추가 구현사항이기에 구현하지 못했습니다.
![평가별점기능](https://user-images.githubusercontent.com/90183279/177061829-c552c55c-a84d-4976-b7a0-ba7b19d28009.gif)
4. (팀) 코멘트 UI
- 코멘트 버튼을 통해 모달창을 열 수도 있고, 보고싶어요 UI를 통해 열리는 카드를 통해서도 모달창을 열 수 있습니다.
- 백앤드 서버와의 전송/응답은 추가 구현사항이기에 구현하지 못했습니다.
![코멘트 모달창](https://user-images.githubusercontent.com/90183279/177061845-37c9e955-df4d-4596-bde8-76547a9b4f99.gif)

5. (개인) 스켈레톤 UI
- (라이브러리 x) 서버로부터 응답을 받지 못했거나 불러오지 못했을 때 사용자에게 대신 보여주는 스켈레톤 UI를 구현했습니다.
![스켈레톤 ui](https://user-images.githubusercontent.com/90183279/177061834-9c996161-3438-43f5-8663-04a11758ea7c.gif)

## :: 성장 포인트
1. 컴포넌트를 너무 분리하면 안된다는 교훈을 얻었습니다. 팀원에게 설명할 수 있을 정도의 컴포넌트면 되지만, 자기 자신도 설명할 수 없을 정도의 컴포넌트 개수면 가독성이 떨어진다는 것을 알게되었습니다.
<img width="249" alt="스크린샷 2022-07-04 오전 9 02 00" src="https://user-images.githubusercontent.com/90183279/177061875-9a4fe8ae-7d46-41c5-8b2f-216a10301e50.png">
2. 레이아웃을 만들면서 자주 사용하게되는 스타일링이나, 동일한 마진과 페딩은 등록해놓고 쓰면 변경할 때나 사용할 때 아주 편하다는 것을 알았습니다.
```scss
@mixin 이름($w, $h) {
  width: $w;
  height: $h;
}
```

```scss
$margin10: 10px;
$margin20: 20px;
$padding10: 10px;
$padding20: 20px;
```

3.grid형 레이아웃에서 flexible box로 바꾸는 과정에서 처음 만들 때 잘 생각하고 만들자는 생각을 했습니다. 나중에 수정하려면 더 골치아프고 무엇보다 손이 많이 갑니다. 3일 전의 코드도 기억 못하는데.. 나중에 고치려면 기억이 없기 때문입니다.
<br>
4. 반응형 웹 페이지를 기획하고 만든다기보다는 처음 시작부터 뷰포트의 사이즈를 고려해서 잘 만들어야한다고 생각했습니다. 노트북의 화면에 맞추어 작업하면, 예상치 못한 일이 벌어집니다.
<br>
5. 새로 고침을 하거나 state가 업데이트되었을 때, 컴포넌트와 state에 대해 더 잘 알게 되었습니다. 진행 중 어려움을 2번 정도 경험했는데 내용은 다음과 같습니다.
- Uncaught TypeError : Cannot read properties of undefined
- 이 에러에 대해서는 블로그 글로 정리했습니다. https://conqueror-g.tistory.com/195
- 보고 싶어요 기능이 해제된 것처럼 보이는 현상
- 이 현상은 백앤드와의 데이터 수정이 어렵기 때문에 추가 구현사항으로 미루었습니다.
<br>
6. 간단한 데이터 가공은 Front-end에서도 할 수 있다는 것을 깨달았습니다.
- 앞으로는 백앤드와 소통하기 전에 Front-end에서는 할 수 있는 것이 없는지 확인하고 소통하기로 마음먹었습니다.
- 자세한 내용은 회고 글에 기록해두었습니다. https://conqueror-g.tistory.com/201
<br>

## 소통에 사용한 협업 툴
### Slack
<img width="942" alt="스크린샷 2022-07-01 오후 3 48 13" src="https://user-images.githubusercontent.com/50426259/176840075-30907e6a-8be6-4914-88d3-fe0d3742ad9c.png">

- Back-end와 자료 공유 및 개인적인 소통

### Trello
![trello](https://user-images.githubusercontent.com/50426259/176840626-5bc5b445-4c0b-4259-93bd-56d9f63f2485.gif)
- 미팅에서 각자의 작업 현황 공유

### Notion
![image](https://user-images.githubusercontent.com/50426259/176840968-aab75ef3-4a5c-4497-a532-db539a297b58.png)
- 매일 진행되는 Stand-up meeting에서 각자의 진행 상황과 블로커 파악 및 소통

### ERD
![image](https://user-images.githubusercontent.com/50426259/176841194-db70fa46-6f62-4a65-8638-3c2562092a32.png)
- Back-end의 ERD 자료 구성을 참고하여 Mockdata 및 실제 서버와 통신시 불러오는 key값 확인

## 프로젝트 회고
https://conqueror-g.tistory.com/201

