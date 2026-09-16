---
layout: default
title: 홈
---

# 메모장에 잠들어 있는 아이디어, 오늘 깨우세요

노션 템플릿 + Claude 프롬프트 5개로, 기록을 기획서로 바꾸는 시스템입니다.

<div class="kj-problem">
<p>아이디어가 떠오르면 메모장이나 노션에 일단 적어두긴 하는데, 그다음이 없어서 그대로 묻힌 적 있으신가요?</p>
<p>정리되지 않은 아이디어는 결국 다시 열어보지 않는 메모로 남습니다.</p>
</div>

## 무엇이 다른가요

<div class="kj-features">
<div class="kj-feature-card">
<div class="kj-feature-icon">🧩</div>
<h3>아이디어 구조화 프레임워크</h3>
</div>
<div class="kj-feature-card">
<div class="kj-feature-icon">📒</div>
<h3>노션 템플릿 활용법</h3>
</div>
<div class="kj-feature-card">
<div class="kj-feature-icon">🤖</div>
<h3>Claude 프롬프트 실전 예시</h3>
</div>
</div>

## 실제로 이렇게 정리됩니다

<div class="kj-window">
<div class="kj-window-bar">
<span class="kj-dot kj-dot-red"></span>
<span class="kj-dot kj-dot-yellow"></span>
<span class="kj-dot kj-dot-green"></span>
<span class="kj-window-title">노션 템플릿 미리보기</span>
</div>
<div class="kj-window-body">

<p class="kj-panel-label">아이디어 트래커</p>
<div class="kj-table-wrap">
<table class="kj-table">
<thead>
<tr><th>제목</th><th>카테고리</th><th>상태</th><th>연결된 프로젝트</th></tr>
</thead>
<tbody>
<tr><td>주말에만 운영하는 소규모 온라인 클래스</td><td>개인 프로젝트</td><td><span class="kj-badge kj-badge-done">프로젝트 전환</span></td><td>온라인 클래스 파일럿 1기</td></tr>
<tr><td>퇴근 후 30분 뉴스레터 요약 서비스</td><td>업무, 자기계발</td><td><span class="kj-badge">아이디어 단계</span></td><td>(없음)</td></tr>
<tr><td>중고 캠핑용품 큐레이션 카탈로그</td><td>기타</td><td><span class="kj-badge kj-badge-progress">AI 정리중</span></td><td>(없음)</td></tr>
</tbody>
</table>
</div>

<p class="kj-panel-label">프로젝트 트래커</p>
<div class="kj-table-wrap">
<table class="kj-table">
<thead>
<tr><th>제목</th><th>상세 내용</th><th>진행률</th><th>연결된 아이디어</th></tr>
</thead>
<tbody>
<tr><td>온라인 클래스 파일럿 1기</td><td>2026-01 첫 모집 시작, 신청 5명. 2026-02 1차 클래스 진행 완료, 만족도 설문 회수.</td><td>20%</td><td>주말에만 운영하는 소규모 온라인 클래스</td></tr>
</tbody>
</table>
</div>

</div>
</div>

## 최신 글

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}

---

### 노션+Claude 템플릿, 지금 시작하기

1인창업가를 위해 설계 — 실제로 매일 사용 중인 시스템입니다.

혼자 창업을 준비 중이라면, 아이디어를 사업계획으로 바꿔주는 템플릿을 19,000원(＄14.99)에 만나보세요.

<!-- CTA: Lemon Squeezy 결제 링크 -->
[템플릿 받고 바로 기획서 만들기]({{ site.lemonsqueezy_checkout_url }})

## 자주 묻는 질문

<div class="kj-faq">
<div class="kj-faq-item">
<p class="kj-faq-q">Q. 노션 유료 플랜이 필요한가요?</p>
<p class="kj-faq-a">A. 아니요, 무료 플랜에서도 사용 가능한 구성입니다.</p>
</div>
<div class="kj-faq-item">
<p class="kj-faq-q">Q. Claude 유료 계정이 필요한가요?</p>
<p class="kj-faq-a">A. 무료 플랜에서도 사용 가능한 구성입니다. 프롬프트 사용량이 많다면 유료 플랜이 더 편리할 수 있습니다.</p>
</div>
<div class="kj-faq-item">
<p class="kj-faq-q">Q. 환불 정책은?</p>
<p class="kj-faq-a">A. 결제 페이지 안내를 따라주세요.</p>
</div>
</div>
