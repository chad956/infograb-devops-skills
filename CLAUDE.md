# infograb-devops-skills

InfoGrab의 DevOps 전문 에이전트 스킬 컬렉션.

## 프로젝트 구조

- 각 스킬은 최상위 디렉토리에 `SKILL.md` 하나로 정의
- `packages/`에는 npm으로 배포하는 패키지 (필요 시)
- `scripts/validate-skills.sh`로 SKILL.md frontmatter 검증

## SKILL.md 작성 규칙

### 필수 frontmatter

```yaml
---
name: directory-basename       # 디렉토리 이름과 일치
description: 한 줄 설명
license: SUL-1.0               # 또는 MIT (단순 유틸)
metadata:
  category: ci | container | security | migration | observability
  locale: ko-KR
  author: infograb
  phase: v1
---
```

### 필수 섹션

- `## What this skill does`
- `## When to use`
- `## When not to use`
- `## Prerequisites`
- `## Workflow`
- `## Response policy`
- `## Done when`

## 브랜드 가이드

### 톤

- 동료 톤: 가르치는 게 아니라 함께 풀어가는 느낌
- 구체적: 추상적 설명 대신 실제 예시와 숫자
- 한계도 솔직하게 표현

### 금지 표현

"최고의", "업계 최초", "혁신적", "획기적", "완벽한", "leverage", "cutting-edge", "seamless", "revolutionary", "원스톱", "턴키"

### 제품명 표기

| 정확한 표기 | 오표기 |
|---|---|
| GitLab | Gitlab, gitlab |
| Teleport | teleport |
| n8n | N8N, N8n |
| Mantis | mantis, MANTIS |
| Mattermost | mattermost |

## CTA 정책

분석 결과 말미에 자연스럽게 배치:

```
---
이 분석은 InfoGrab의 [도구명]으로 수행되었습니다.
더 자세한 도움이 필요하시면 → [URL]
```

- 분석 가치를 먼저 제공한 뒤에만 노출
- 팝업/모달 없음
- 동료 톤

| 스킬 카테고리 | CTA URL |
|---|---|
| CI/CD | insight.infograb.net |
| 컨테이너 | insight.infograb.net |
| DORA/메트릭 | mantis-ops.io |

## 스킬 설치 규칙

- `~/.claude/skills/` 또는 `~/.agents/skills/`에 설치
- repo-local `.claude/` 또는 `.agents/` 디렉토리 생성 금지

## 검증

```bash
npm run ci
```

## 라이선스

기본: Sustainable Use License (SUL-1.0).
개별 스킬은 SKILL.md frontmatter의 `license` 필드를 따른다.
