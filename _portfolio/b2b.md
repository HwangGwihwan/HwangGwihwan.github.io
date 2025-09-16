---
title: "B2B 무역 구매·배송 서비스"
featured: true
excerpt: "<img src='/images/trade.png' style='width: 240px; height: 160px;'>"
collection: portfolio

---

# 🏬 B2B 무역 구매·배송 서비스

**B2B 무역 구매·배송 서비스**는 구매·배송 과정을 전자화하고 쇼핑몰 기능을 통합한 무역 중개 플랫폼입니다.  
기업과 개인 사용자를 위한 맞춤형 권한 기능을 제공하며, 계약서 작성부터 결제, 배송까지 End-to-End 프로세스를 지원합니다.

---

🔗 [🔍 B2B 무역 구매·배송 서비스 사이트 바로가기](http://3.36.133.135:9000/)

테스트 계정
<pre>
관리자	: admin001	1234
개인회원	: personal001	Qwer1234!
	: personal003	Qwer1234!
기업회원	: biz001	Qwer1234!
	: biz002	Qwer1234!
</pre>
## 🧩 프로젝트 개요

- **개발 목적**: B2B 무역의 구매·배송 과정을 전자화하여 효율적인 중개 시스템 구축
- **주요 특징**:
  - 계약서 작성, 결제, 배송까지 End-to-End 프로세스 지원
  - 기업/개인/관리자 권한 기반 맞춤형 기능 제공
  - 쇼핑몰 기능 통합 (상품 등록, 검색, 주문, 찜, 장바구니 등)
  - 회원·상품 관리의 디지털화 및 표준화된 데이터 설계
- **참여 인원**: 4명
- **개발 기간**: 2025.07.28 ~ 2025.09.10

## 🏗️ 기술 스택

| 항목 | 사용 기술 |
|------|-----------|
| Frontend | HTML5, CSS3, JavaScript, jQuery, Bootstrap |
| Backend | Java 17, Spring Framework, Servlets & JSP, AJAX |
| DBMS | MySQL |
| ORM | Mybatis |
| Server | Apache Tomcat, Jenkins |
| API | Kakao API (주소, 페이), 공휴일 API, 네이버 & 카카오 소셜 로그인 API |
| Email | JavaMail (Gmail SMTP) |
| Server | Apache Tomcat, Jenkins |
| 개발 환경 | Eclipse |

---

## 🧑‍💼 담당 역할  
- 상품 요청, 등록
- 상품 수정, 재고 관리
- 상품 목록 및 상세 페이지 관리
- 찜 및 장바구니 기능 개발
- 카테고리 및 옵션 관리

---

## ✨ 문제 해결 사례

⚠️ 문제 상황 (Problem)
 - 팀원의 주문 기능과 본인의 상품/장바구니 기능을 연동해야 했음
 - 원래는 DTO를 통해 결제 페이지로 데이터 전달 필요
 - 그러나 팀원의 주문 Controller가 DB에서 직접 값을 조회하도록 구현되어 구조 변경이 어려운 상황 발생

🛠️ 해결 방법 (Solution)
 - 상품 구매 시 주문 테이블에 데이터를 삽입하되 use_status를 **‘N’**으로 설정해 결제 전에는 구매 내역에 표시되지 않도록 처리
 - 결제가 완료되면 use_status를 **‘Y’**로 변경해 구매 내역에 반영되도록 구현
 - 기존 주문 Controller 코드를 수정하지 않고도 연동 가능하도록 설계

✅ 결과 (Result)

 - 팀원 코드 수정 없이 협업 효율성 유지
 - 구매 데이터 흐름의 일관성과 보안성 확보

---

⚠️ 문제 상황 (Problem)
 - 장바구니 기능에서 재고 변동으로 인한 수량 불일치 발생
 - 사용자가 담아둔 수량보다 실제 재고가 줄어든 경우 오류 및 결제 실패 위험 존재

🛠️ 해결 방법 (Solution)
 - 장바구니 진입 시 재고를 실시간 확인, 부족한 수량은 자동으로 조정
 - 결제 직전에도 재고 재검증을 수행해 부족할 경우 결제 차단
 - 변동 상황에서도 오류 없이 서비스가 동작하도록 설계

✅ 결과 (Result)
 - 사용자의 불편 최소화 (재고 부족 시 자동 처리)
 - 결제 오류 방지 및 서비스 안정성 확보
 - 서비스 신뢰성 향상

---

## 🗃️ ERD

<img src='/images/4. ERD_Y조(B2B 무역).png' style='width: 400px; heigth: 340px;'>

---

## 🧾 산출물

- [WBS](/files/1. WBS_Y조(B2B무역).xlsx)
- [요구사항 정의서](/files/2. 요구사항 정의서_Y조(B2B 무역).xlsx)
- [테이블 정의서](/files/3. 테이블 정의서_Y조(B2B 무역).xlsx)
- [화면 설계서](/files/5. 화면설계서_Y조(B2B 무역).pdf)

---

## 📺🎥 시연 영상

<iframe width="560" height="315" src="https://www.youtube.com/embed/m8-1TUBeuFU" 
title="YouTube video player" frameborder="0" 
allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen></iframe>






