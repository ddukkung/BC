# 집밥선생
![메인](https://user-images.githubusercontent.com/88926356/143993110-fd70e0fb-6a5d-4900-802c-f9320c22bafa.png)

* 집밥선생은 반찬을 판매하는 쇼핑몰 웹 사이트 프로젝트입니다.
* [더반찬](https://www.thebanchan.co.kr/main/initMain.action) 사이트를 클론코딩하였습니다.
* 해당 레파지토리는 프로젝트 진행 도중 깃허브 사용 미숙으로 기존의 레파지토리가 사용 불가능해져 새로 만들어진 곳입니다. 이전의 커밋 기록 및 작업 내용을 보시려면 아래의 레파지토리를 참고해주십시오.
  * https://github.com/ITWILL1TEAM/Banchan

<br>

## 1. 제작 기간 & 참여 인원
* 2021년 10월 1일 ~ 11월 11일
* 8인 팀 프로젝트

<br>

## 2. 사용 기술
  * Java 8
  * Tomcat 8.5
  * JSP
  * MySQL 5.7
  * Ajax, JQuery
  * BootStrap

<br>

## 3. ERD 설계
![반찬-erd](https://user-images.githubusercontent.com/88926356/164419930-59b7c0d6-b9a1-4560-a789-5cf51aac1245.jpg)

<br>

## 4. 핵심 기능
회원 유형에 구매자, 판매자, 관리자가 있어 판매자는 판매하고자 하는 글을 등록할 수 있고 구매자는 물건을 구매할 수 있습니다. 
관리자는 판매자가 올린 글을 관리합니다.  
본인(**배재희**)이 맡은 파트는 **제품 상세 페이지와 장바구니**로, 아래에 제가 구현한 것 중심으로 기능에 대해 상세 설명하겠습니다.  

<br>

### Product
![product2](https://user-images.githubusercontent.com/88926356/142717270-67d160be-dbc1-426a-8c63-3225161e7f62.gif)
* 제이쿼리를 사용해 수량 조절 버튼 구현. 수량 조절 시 그에 따라 총 제품 금액 또한 변화된다.
* 로그인했을 경우에만 장바구니에 담거나 바로구매 가능
* 장바구니 버튼을 클릭할 경우 유저가 선택한 수량만큼 장바구니에 해당 제품이 담기며 장바구니 페이지로 이동
* 바로 구매 버튼을 클릭할 경우 결제 페이지로 이동하여 유저가 선택한 수량만큼 해당 제품 구매 가능

<br>
 
### Cart
![cart](https://user-images.githubusercontent.com/88926356/142717575-6c2ca539-c462-417e-9e84-2315d8f5ba98.gif)
* 수량 조절 버튼과 수정 버튼을 통해 수량 조절 가능. 수량 조절 시 그에 따라 수량, 구매금액, 주문 합계 금액이 변화된다.
* 개별 삭제와 선택 삭제를 통해 장바구니에서 삭제 
* 주문 버튼 클릭 시 배송지가 입력되지 않은 회원일 경우 배송지 입력 페이지로 이동
* 배송지가 입력된 회원이고 주문 금액이 10,000원 이상일 경우 결제 페이지로 이동

 <br>
