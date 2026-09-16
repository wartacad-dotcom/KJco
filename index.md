---
layout: default
title: 홈
---

# 메모장에 잠들어 있는 아이디어, 오늘 깨우세요

노션 템플릿 + Claude 프롬프트 5개로, 기록을 기획서로 바꾸는 시스템입니다.

- 아이디어 구조화 프레임워크
- 노션 템플릿 활용법
- Claude 프롬프트 실전 예시

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
