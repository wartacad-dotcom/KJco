---
layout: default
title: 홈
---

# 1인창업가를 위한 아이디어 디벨로퍼

막연한 아이디어를 노션 + Claude 템플릿으로 정리해 실행 가능한 사업계획으로 바꾸는 방법을 다룹니다.

- 아이디어 구조화 프레임워크
- 노션 템플릿 활용법
- Claude 프롬프트 실전 예시

## 최신 글

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}

---

### 노션+Claude 템플릿, 지금 시작하기

혼자 창업을 준비 중이라면, 아이디어를 사업계획으로 바꿔주는 템플릿을 19,000원(＄14.99)에 만나보세요.

<!-- CTA: Lemon Squeezy 결제 링크 -->
[지금 구매하기]({{ site.lemonsqueezy_checkout_url }})
