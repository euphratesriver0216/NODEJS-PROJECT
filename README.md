# 다이쪼 팀

### 팀장 : 이성현 <a href="https://github.com/Mr-butter"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub&logoColor=white"/></a>
### 팀원 : 김현호 <a href="https://github.com/Hyerin1208"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub&logoColor=white"/></a> , 박해민 <a href="https://github.com/euphratesriver0216"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub&logoColor=white"/></a>, 이민주 <a href="https://github.com/codecocosl"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub&logoColor=white"/></a> 
---------------------------------------
## DAITZOSHOP
https://daitzoshop.herokuapp.com/
---------------------------------------

### 로컬DB 환경에서 실행 방법
Install the dependencies:
```
yarn install
yarn start
```

```
index.js 에서 connect 부분 MONGODB HOST 본인꺼로 수정
```

[http://localhost:3000](http://localhost:3000) 로컬에서 실행된 어플리케이션을 확인할 수 있습니다.


### 프로젝트 기간 : 2021-10-01 ~ 2021-10-15 (총 14일)

### 개요
MongoDB, Express, EJS, Node 기반의 쇼핑몰 플랫폼 개발

### 목적
Node 및 Database 스킬 숙련을 위한 자체 팀 프로젝트
1. 간단한 회원가입과 상품 등록 구현으로 DB 연동 숙련 
2. 결제 API를 통해 API 기술 숙련
3. socket.io를 통해 채팅 구현

### 사용기술 요약
- Node(socket.io, Express, passport, cookie)
- MongoDB(Compass, Atlas)
- EJS(views)
- iamport(결제 API)

### 개발환경
EJS, html, css, javascript, Node, MongoDB


### 페이지 별 프로젝트 내 사용 기술

|      페이지      | 구현 기능 |
--------|------------
회원 가입  | 회원정보등록
상품 페이지 | 남성, 여성, 악세사리로 크게 구별
채팅 페이지 | admin과 혹은 일반 유저끼리의 소통으로 상품정보나 개인 소통
admin 페이지 | 상품 등록, 베너 등록, 구매 조회
장바구니 페이지 | cookie로 저장하며, 결제 API 통해서 결제시 장바구니 초기화
결제 페이지 | 배송지 정보 입력 후 결제 가능


### 프로젝트 팀 구성 및 역할
#### 이성현 (팀장)
Back : Server 구축 및 DB 구조 설계, 배포

#### 김현호
Back : 결제 API 및 채팅 구현

#### 박해민
Front :  admin 상품 등록 및 user 상품 페이지 구현

#### 이민주
Front : 채팅 및 장바구니, 결제, 회원가입/로그인 페이지 구현


> **사용 모듈**
"nodemon": "^2.0.7",
    "body-parser": "^1.18.3",
    "cheerio": "^1.0.0-rc.2",
    "co": "^4.6.0",
    "connect-flash": "^0.1.1",
    "connect-mongo": "^3.2.0",
    "cookie-parser": "^1.4.3",
    "csurf": "^1.9.0",
    "ejs": "^2.6.1",
    "express": "^4.16.3",
    "express-paginate": "^1.0.0",
    "express-session": "^1.15.6",
    "iamporter": "^1.4.2",
    "mongodb": "^3.6.6",
    "mongoose": "^5.12.5",
    "mongoose-auto-increment": "^5.0.1",
    "mongoose-plugin-autoinc": "^1.1.9",
    "morgan": "^1.9.1",
    "multer": "^1.4.1",
    "passport": "^0.4.0",
    "passport-facebook": "^2.1.1",
    "passport-local": "^1.0.0",
    "path": "^0.12.7",
    "request": "^2.88.0",
    "socket.io": "^2.4.1",
    "yarn": "^1.22.10"

## **발생한 이슈와 해결방법**

1.  DB 스키마 이슈

-   처음엔 쿠키가 아니라 장바구니 스키마를 만들어 관리하려 했으나 스킬 부족으로 구현을 실패
-   경험을 통해 데이터베이스 다루는 기술의 중요성을 깨달음

2.  코로나로 인한 비대면 이슈

-   협업툴 활용 정해진 시간에 리뷰
-   진행상황 공유하여 내용 숙지

3.  배포 이슈

-   AWS로 배포를 시도하였으나 숙련도 부족으로 Heroku로 배포를 진행함.
-   Caffeine으로 서버가 닫히지 않게는 하였지만 그 전에는 수면상태에 들어가 접속 시 지연이 있었음.
