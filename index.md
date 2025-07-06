---
layout: home
author_profile: true
---

## 안녕하세요! 👋

**DongGeon Park**의 블로그에 오신 것을 환영합니다.

### 🚀 저는 누구인가요?
- 개발자로서 새로운 기술을 배우고 공유하는 것을 좋아합니다
- 블로그를 통해 지식을 나누고 성장하고 있습니다
- 현재 Jekyll과 GitHub Pages로 블로그를 운영하고 있습니다

### 🏷️ 카테고리
- [블로그](/categories/#블로그) - 블로그 관련 글들
- [개발](/categories/#개발) - 개발 관련 글들 (예정)
- [일상](/categories/#일상) - 일상 이야기들

### 🔍 찾아보기
- [모든 글 보기](/posts/)
- [태그별 보기](/tags/)

### 📝 최근 글
{% if paginator %}
  {% assign posts = paginator.posts | slice: 0, 3 %}
{% else %}
  {% assign posts = site.posts | slice: 0, 3 %}
{% endif %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% include documents-collection.html entries=posts type=entries_layout %}
</div>

{% include paginator.html %}

---

*더 많은 내용으로 채워나가겠습니다! 😊* 