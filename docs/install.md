# 설치 방법

## Vercel skills CLI (범용 에이전트)

Claude Code, Codex, OpenCode, Cursor 등 대부분의 코딩 에이전트에서 사용 가능.

### 전체 설치

```bash
npx --yes skills add infograb/infograb-devops-skills --all -g
```

### 선택 설치

```bash
npx --yes skills add infograb/infograb-devops-skills --skill gitlab-ci-xray
```

### 설치 확인

```bash
npx --yes skills ls -g
```

## Claude Code plugin

Claude Code 네이티브 플러그인 방식:

```bash
claude plugin add infograb/infograb-devops-skills
```

## 에이전트에게 맡기기

아래 문장을 에이전트에 그대로 붙여넣으면 설치를 진행한다:

```text
infograb-devops-skills를 설치해줘. 설치가 끝나면 사용 가능한 스킬 목록을 보여줘.
```

## 요구사항

- Node.js 18+
- 개별 스킬의 upstream CLI는 Prerequisites 섹션 참고
