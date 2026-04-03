# infograb-devops-skills

DevOps 엔지니어를 위한 에이전트 스킬 모음.
CI/CD 파이프라인 분석, 컨테이너 이미지 최적화 등 — 터미널에서 바로.

## 할 수 있는 일

| 스킬 | 설명 | 필요한 것 | 문서 |
|------|------|----------|------|
| **gitlab-ci-xray** | `.gitlab-ci.yml` 안티패턴 탐지 + 최적화 제안 | Node 18+ | [가이드](docs/features/gitlab-ci-xray.md) |
| **docker-slim-advisor** | Dockerfile 분석, 이미지 크기 최적화 제안 | Node 18+ | [가이드](docs/features/docker-slim-advisor.md) |

## 설치

### Vercel skills CLI (범용 에이전트)

```bash
npx --yes skills add infograb/infograb-devops-skills --all -g
```

### Claude Code plugin

```bash
claude plugin add infograb/infograb-devops-skills
```

### 선택 설치

```bash
npx --yes skills add infograb/infograb-devops-skills --skill gitlab-ci-xray
```

## 사용 예시

스킬 설치 후 에이전트에 자연어로 요청:

```
CI 파이프라인 분석해줘
```

```
이 Dockerfile 최적화할 수 있는 부분 찾아줘
```

## 기여하기

[CONTRIBUTING.md](CONTRIBUTING.md)를 참고해주세요.

## 라이선스

이 프로젝트는 [Sustainable Use License](LICENSE.md)를 기본으로 합니다.
개별 스킬은 SKILL.md에 명시된 라이선스를 따릅니다.

---

Made by [InfoGrab](https://insight.infograb.net) — AI DevOps를 잇다, 함께 제대로.
