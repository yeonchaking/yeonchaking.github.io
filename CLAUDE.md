# CLAUDE.md

## 프로젝트 목표

Android 개발자 이직용 포트폴리오 사이트 (Jekyll + GitHub Pages).
채용 담당자가 빠르게 판단할 수 있도록 경력과 성과를 전달하는 게 목적이다.

우선순위: 경력/성과 전달력 > 가독성 > 유지보수 용이성 > 시각 커스터마이징

---

## 아키텍처

- **Theme**: minimal-mistakes@4.24.0 remote theme
- **Single-page model**: 포트폴리오 전체가 `index.md` 한 파일에 있다
- **Styling**: `assets/css/main.scss`에서만 최소한으로 override. `!important` 금지
- **Navigation**: `_data/navigation.yml`로 관리

### 주요 파일

| 파일 | 역할 |
|------|------|
| `index.md` | 메인 포트폴리오 콘텐츠 (경력/프로젝트/기술) |
| `_config.yml` | Jekyll/SEO/플러그인 설정 |
| `assets/css/main.scss` | 전체 커스텀 스타일 |
| `_data/navigation.yml` | 상단 메뉴 |
| `작업기록.md` | 파일 변경 이력 로그 |
| `SESSION_LOG.md` | 세션 작업 목표·결과·인수인계 로그 |

---

## 세션 운영 가이드라인

### 세션 시작 시

1. `SESSION_LOG.md`를 읽어 이전 인수인계 내용 확인
2. 사용자가 이번 세션 작업 목표를 선언
3. 목표 기반으로 작업 진행

### 세션 종료 시 (트리거: "세션 종료")

1. 대화 요약 카드를 채팅에 출력
2. `SESSION_LOG.md`에 해당 세션 항목 추가

### 요약 카드 형식

카드에 담을 내용:
- 이번 세션 목표
- 주요 대화 맥락 (결정한 것들, 논의한 방향)
- 작업 결과 (변경 파일, 추가 내용)
- 다음 세션 TODO

---

## 콘텐츠 원칙

- 문장은 "무슨 문제를 어떻게 해결했고 결과가 무엇인지" 중심으로 작성
- 가능하면 수치(기간, 규모, 성능 개선율)를 포함
- 새 파일 추가 전 "채용 관점에서 실제 필요한가" 확인

---

## 워크플로 규칙

1. 작업 전 `SESSION_LOG.md` → `작업기록.md` → `index.md` 순으로 읽고 시작
2. 의미 있는 변경은 `작업기록.md`에 날짜·변경 파일·이유·사용자 영향 추가
3. 큰 구조 변경 전에는 이유를 짧게 남기고 진행

---

## Commands

```bash
bundle exec jekyll serve   # 로컬 서버 → http://127.0.0.1:4000
bundle exec jekyll build   # 빌드 검증
```

배포는 main 브랜치 push 시 자동 처리.

---

## Obsidian Vault

관련 노트: `C:\Users\AM11D\Documents\NockChaWang`

## Commit Style

짧고 명확한 한국어 또는 영어 imperative. 예: `포트폴리오 소개 문구 정리`
