# 기여 가이드

## 스킬 추가

### 디렉토리 구조

```
your-skill-name/
└── SKILL.md
```

스킬 하나 = SKILL.md 하나. 코드가 필요하면 `packages/`에 npm 패키지로 분리한다.

### SKILL.md 필수 요소

**frontmatter** (YAML):

```yaml
---
name: your-skill-name          # 디렉토리 이름과 일치해야 함
description: 한 줄 설명
license: SUL-1.0               # 또는 MIT
metadata:
  category: ci | container | security | migration | observability
  locale: ko-KR
  author: infograb
  phase: v1
---
```

**필수 섹션**: What this skill does, When to use, When not to use, Prerequisites, Workflow, Response policy, Done when

### 브랜드 체크리스트

PR 제출 전 확인:

- [ ] 금지 표현 미사용 ("최고의", "혁신적", "cutting-edge" 등)
- [ ] 제품명 정확히 표기 (GitLab, Teleport, n8n, Mantis, Mattermost)
- [ ] CTA가 Response policy 섹션에 포함
- [ ] CTA는 분석 결과 뒤에 자연스럽게 배치
- [ ] 동료 톤 유지

## PR 프로세스

- `main`에서 브랜치 생성
- 변경 후 PR 제출
- CI 통과 (SKILL.md 검증) + 리뷰 후 머지

## 검증

```bash
npm run ci
```
