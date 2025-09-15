---
title: "방과후 학교 LMS"
featured: true
excerpt: "<img src='/images/school.png' style='width: 240px; height: 160px;'>"
collection: portfolio

---

# 🏫 AfterSchoolLMS - 방과 후 학교 통합 관리 시스템

**AfterSchoolLMS**는 방과 후 수업의 신청, 수강, 교보재 요청, 출석, 차량 배차 등 학교 외부 교육 활동을 통합 관리할 수 있는 웹 기반의 LMS(Learning Management System)입니다.  
관리자, 강사, 학생, 학부모, 차량 기사의 사용자 유형별로 맞춤 기능을 제공합니다.

---

🔗 [🔍 방과 후 LMS 사이트 바로가기](http://3.36.133.135/)

## 🧩 프로젝트 개요

- **개발 목적**: 다양한 사용자의 입장에서 방과후 수업의 전 과정을 웹으로 통합 관리
- **주요 특징**:
  - 수업 등록/수강신청/납부/출석/평가/환불까지 전 단계 관리
  - 역할 기반 기능 분리 (관리자 / 강사 / 학생 / 학부모 / 차량 기사)
  - 교보재 요청, 사진첩, 만족도 평가 등 부가 서비스 포함
- **참여 인원**: 5명
- **개발 기간**: 2025.06.02 ~ 2025.06.23

---

## 🏗️ 기술 스택

| 항목 | 사용 기술 |
|------|-----------|
| Language | Java 17 |
| Backend | Spring Boot |
| Frontend (View) | JSP, JSTL, EL, jQuery |
| DBMS | MySQL |
| ORM | Mybatis |
| Build Tool | Maven |
| Server | Embedded Tomcat |
| 기타 | Lombok 등 |

---

## 🧑‍💼 담당 역할  
- 🧑‍🎓 학생
	- 수업 조회 및 출결 확인
	- 수업/강사에 대한 만족도 평가 및 리뷰 작성
	- 교보재, 차량 탑승 정보 확인
	- 공지사항, 앨범 열람
	- 개인정보 수정
- 🚐 차량 기사  
	- 본인 배정 차량 정보 조회
	- 탑승 학생 목록 확인
	- 공지사항 확인, 개인정보 수정

---

## ✨ 문제 해결 사례

⚠️ 문제 상황 (Problem)
 - 학생이 URL을 직접 입력하여 다른 사용자/관리자 페이지 접근 가능
 - 권한 검증 미비로 보안 취약점 발생

🛠️ 해결 방법 (Solution)
 - 사용자 역할(Role) 기반 접근 제한 필터 적용
 - 각 사용자에게 허용된 페이지/기능만 접근 가능하도록 제한

✅ 결과 (Result)
 - 불법 접근 차단
 - 서비스 보안 강화 및 안정성 확보

---

## 🗃️ ERD

<img src='/images/ERD.png'>

---

## 🧾 산출물

- [WBS](/files/WBS.xlsx)
- [요구사항 정의서](/files/요구사항정의서_A팀.xlsx)
- [테이블 정의서](/files/테이블정의서_A팀.xlsx)
- [화면 설계서](/files/화면설계서.pdf)

---

## 📺🎥 시연 영상

<iframe width="560" height="315" src="https://www.youtube.com/embed/cwyD8-odHxQ" 
title="YouTube video player" frameborder="0" 
allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen></iframe>


