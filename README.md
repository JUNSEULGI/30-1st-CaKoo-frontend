# cakoo 프로젝트
<img width="234" alt="스크린샷 2022-03-13 오후 7 58 05" src="https://user-images.githubusercontent.com/60570733/158056356-f913f84b-a0c9-4094-9c0b-e6b23c2d6faa.png">
케이쿠는 꾸까를 모티브로 해 케이크를 판매하는 이커머스 사이트로 구매하기까지의 로직에 집중하여 클론코딩을 진행하였습니다. 원하는 케이크 조건 검색, 케이크 리스트 조회, 케이스 상세 페이지, 상품 장바구니 넣기, 수량 선택, 주문까지 하나의 플로우를 구현했습니다.
<br><br>

### 🚀 개발 인원 및 기간
* 개발 기간 : 2022/2/28 ~ 2022/3/11 (2주간)
* 프론트엔드 3명, 백엔드 3명
    * Back-end   
        * 김기현 - Modeling, SignUp, Product List API, Order API
        * 이지원 - Modeling, Cart API
        * 박건규 - Modeling, SignIn, Product Detail API, Order API
    * Front-end  
        * 신윤숙 - Login, Order
        * 전슬기 - Product List, Product Detail
        * 김준영 - Sign Up, Cart 
     * <a href="https://github.com/wecode-bootcamp-korea/30-1st-CaKoo-frontend">프론트 github 링크</a>
<br><br>


# 📍 데모 영상

![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/60570733/158057150-f3502d34-5bee-4b4b-a78a-baccb133f661.gif)


<br><br>


# 🌷 Target site
<img src = "https://user-images.githubusercontent.com/90089275/158053540-dbe10e54-bdf5-40a6-8a10-2f8730f4abda.png" width="1000" height="400">

* ## 사이트 소개  
    [Site Link](https://kukka.kr)
    
    꽃을 일상에서 가볍게 즐기는 핀란드의 문화를 한국에 전파하는 것이 목표 

    우리는 한국에도 멋진 ‘꽃 브랜드’가 생길 수 있다고 믿고 행동하는 사람들이 모인 곳  

* ## 사이트 선정 이유
    * 깔끔한 UI
    * 이커머스의 기본 기능인 로그인, 회원가입, 상품 조회, 옵션 선택, 장바구니, 주문 기능을 모두 담고 있음

<br><br>


# 💡 초기기획 & ERD

## ERD
![image](https://user-images.githubusercontent.com/90089275/158053700-521e9dce-0720-49c7-933a-1c2781cae0a7.png)

## User flow
<img src="https://user-images.githubusercontent.com/90089275/158054162-33f65fd5-e4ca-4948-ae62-22c90769e04f.png">


## 초기기획 및 구현 목표
* 짧은 기간동안 기능구현에 집중해야하므로 사이트의 디자인과 기획만 클론
* 개발은 초기세팅부터 전부 직접 구현
* 사이트 카테고리 중 '꽃다발'만 소재를 케이크로 바꾸어 구현
* 필수 구현 사항을 회원가입, 로그인, 상품 조회, 장바구니, 주문기능으로 설정 
* 한 상품에 여러 옵션(사이즈)이 적용될 수 있게 기획

<br><br>



# 📝 적용 기술 및 구현 기능

* ## 기술 스택
    * ### Front-end  
        <a href="#"><img src="https://img.shields.io/badge/HTML-DD4B25?style=plastic&logo=html&logoColor=white"/></a>
    <a href="#"><img src="https://img.shields.io/badge/SASS-254BDD?style=plastic&logo=sass&logoColor=white"/></a>
    <a href="#"><img src="https://img.shields.io/badge/javascript-EFD81D?style=plastic&logo=javascript&logoColor=white"/></a>
    <a href="#"><img src="https://img.shields.io/badge/React-68D5F3?style=plastic&logo=react&logoColor=white"/></a>
    * ### Back-end  
        <a href="#"><img src="https://img.shields.io/badge/python-3873A9?style=plastic&logo=python&logoColor=white"/></a>
    <a href="#"><img src="https://img.shields.io/badge/Django-0B4B33?style=plastic&logo=django&logoColor=white"/></a>
    <a href="#"><img src="https://img.shields.io/badge/MySQL-005E85?style=plastic&logo=mysql&logoColor=white"/></a>
    <a href="#"><img src="https://img.shields.io/badge/AWS-FF9701?style=plastic&logo=aws&logoColor=white"/></a>
    <a href="#"><img src="https://img.shields.io/badge/bcrypt-525252?style=plastic&logo=bcrypt&logoColor=white"/></a>
     <a href="#"><img src="https://img.shields.io/badge/postman-F76934?style=plastic&logo=postman&logoColor=white"/></a>
    * ### Common  
        <a href="#"><img src="https://img.shields.io/badge/git-E84E32?style=plastic&logo=git&logoColor=white"/></a>
        <a href="#"><img src="https://img.shields.io/badge/RESTful API-415296?style=plastic&logoColor=white"/></a>
    * ### Communication  
        <a href="#"><img src="https://img.shields.io/badge/github-1B1E23?style=plastic&logo=github&logoColor=white"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Slack-D91D57?style=plastic&logo=slack&logoColor=white"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Trello-2580F7?style=plastic&logo=trello&logoColor=white"/></a>
        <a href="#"><img src="https://img.shields.io/badge/Notion-F7F7F7?style=plastic&logo=notion&logoColor=black"/></a>
* ## 구현기능
    * 회원가입 / 로그인
        - 유효성 검사 : input에 사용자가 입력한 값이 주어진 조건을 만족할 때만 버튼을 활성화
        - 백엔드와 통신을 통해 input으로 받은 값을 전달하고, 로그인 시 token을 받아 localStorage에 저장
        - token이 있을 때, 조건부 렌더링을 이용하여 페이지 상단 nav의 로그인/회원가입이 로그아웃/장바구니로 전환
    * 상품 리스트 페이지
        - query parameter를 이용해 판매 상품의 분류(크기)에 따른 filtering과 가격 및 출시순에 따른 sorting 적용
        - 페이지 하단의 "더보기" 버튼 클릭 시, 백엔드로부터 상품 정보를 더 받아와 보여주는 pagination 구현
    * 상품 상세 페이지
        - path parameter로 상품 id를 백엔드에 전달하여 상품 상세페이지에 필요한 데이터를 받아와 그려냄
        - 크기와 수량 옵션을 선택하여 장바구니로 저장
        - 로그인이 되어있을 때만 장바구니 담기 가능
        - 이미 담은 크기 옵션을 다시 선택할 시, alert로 사용자에게 알려주며 담을 수 없게 함
    * 장바구니
        - 백엔드와 통신하여 해당 사용자의 장바구니에 담긴 상품 정보 불러오기
        - 선택한 상품 즉시 삭제(백엔드 데이터베이스에까지 삭제됨)
    * 주문
        - 장바구니에 저장된 상품정보와 사용자 정보를 넘겨받아 그려냄
        - 백엔드에 주문서의 상품을 주문하는 요청을 보냄
<br><br>


## Trello
<img width="1669" alt="스크린샷 2022-03-13 오후 8 17 03" src="https://user-images.githubusercontent.com/60570733/158056941-78f7eece-2557-41c5-a1e3-f6b0407b535c.png">

* 트렐로를 이용해 모든 업무들을 세분화 시켜 하나의 티켓으로 만들었습니다.
* 팀원들과 공유해야할 내용은 공지 탭을 통해 단일화하였습니다.
* 전체 프로세스를 네 가지 카테고리로 나눠서 각각의 티켓을 과정에 따라 하나씩 이동 시키며 프로젝트의 모든 일정과 업무를 관리했습니다.
* 각자 데일리 스탠드업 미팅 로그를 작성하고 10~20분내로 짧게 진행상황 및 블로커를 점검했습니다.
* 스프린트 주기를 지켜 한 스프린트가 끝나고 회고미팅을 해 발전방향을 모색하였습니다.

<br>

# Reference
* 이 프로젝트는 [꾸까](https://kukka.kr) 사이트를 참조하여 학습목적으로 만들었습니다.
* 실수수준의 프로젝트이지만 학습용으로 만들었기 떄문에 이 코드를 활용하여 이득을 취하거나 무단 배포할 경우 법적으로 문제될 수 있습니다.
* 이 프로젝트에서 사용하고 있는 사진 대부분은 위코드에서 구매한 것이므로 해당 프로젝트 외부인이 사용할 수 없습니다
* 이 프로젝트에서 사용하고 있는 로고와 배너는 해당 프로젝트 팀원 소유이므로 해당 프로젝트 외부인이 사용할 수 없습니다

![Footer](https://capsule-render.vercel.app/api?type=waving&color=ffcc51&height=100&section=footer)


