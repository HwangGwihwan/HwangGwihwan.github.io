---
permalink: /
title: "함께 달리고 싶은 열정 지원자, 황귀환입니다."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
.skills {
  display: flex;
  flex-wrap: wrap;   /* 여러 줄로 자동 줄바꿈 */
  gap: 10px;         /* 태그 간격 */
}

.skill-tag {
  display: inline-block;
  padding: 6px 14px;
  border-radius: 20px;     /* pill 모양 */
  background-color: #f0f0f0;
  border: 1px solid #ddd;
  font-size: 14px;
  font-weight: 500;
  color: #333;
}

h2 {
  margin-top: 2rem;
  margin-bottom: 1rem;
  font-size: 1.5rem;
  border-bottom: 1px solid #ccc;
  padding-bottom: 0.3rem;
}
</style>

<h2>나의 스킬</h2>
<div class="skills">
  <span class="skill-tag">Java</span>
  <span class="skill-tag">Spring Boot</span>
  <span class="skill-tag">JSP</span>
  <span class="skill-tag">AJAX</span>
  <span class="skill-tag">JavaScript</span>
  <span class="skill-tag">MyBatis</span>
  <span class="skill-tag">MySQL</span>
  <span class="skill-tag">AWS</span>
  <span class="skill-tag">C</span>
  <span class="skill-tag">Kotlin</span>
  <span class="skill-tag">Swift</span>
</div>

<h2>문제 해결 사례</h2>
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

