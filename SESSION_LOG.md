# SESSION_LOG

세션별 작업 목표·결과·인수인계를 기록한다.
새 세션 시작 시 이 파일을 먼저 읽고 마지막 인수인계 내용을 확인한다.

---

## 세션 로그 형식

```
## YYYY-MM-DD HH:MM | [세션 제목]

**목표**: 이번 세션에서 하려던 것

**결과**:
- 완료한 것
- 변경한 파일

**결정사항**:
- 내린 결정과 그 이유

**미완료 / 다음 TODO**:
- 다음 세션에서 이어받을 내용
```

---

## 2026-05-14 | 구조적 개선 세션

**목표**: 사이트에 보이는 모든 구조적 문제 파악 및 수정

**결과**:
- `_config.yml`: jekyll-remote-theme 플러그인 추가(테마 미적용 근본 원인 수정), avatar/author_profile/이메일 링크 추가, Follow 버튼 제거(repository 항목 삭제)
- `index.md`: 제목 정리(front matter title + 본문 h1 중복 제거), classes:wide 제거(사이드바 활성화), Skills 테이블 형식으로 재구성(Camera2/MediaMuxer 추가), Education+Certificate 섹션 통합, Contact 섹션 추가, 소개 문구 수정
- `_data/navigation.yml`: Experience/Projects/Skills 앵커 링크 추가
- `Gemfile`: jekyll-remote-theme 추가

**결정사항**:
- 소개 문구는 도메인 한정(영상처리+BLE)이 아닌 넓은 방향으로 — "기능 구현부터 아키텍처 설계까지 전반"
- Skills는 테이블 형식 유지 — 다음 템플릿 작업 때 뱃지/태그 UI로 교체하기 좋은 구조
- 세션 플랜 확정: 구조 → 내용 → 템플릿 순서로 진행

**미완료 / 다음 TODO**:
- Experience에 수치/성과 추가
- Projects "문제→해결→결과" 형식으로 재작성
- 소개 문구 추가 다듬기

## 2026-05-14 | 세션 운영 가이드라인 및 CLAUDE.md 정비

**목표**: AI 세션 운영 가이드라인을 수립하고 CLAUDE.md와 SESSION_LOG를 구축한다

**결과**:
- `CLAUDE.md` 전면 재작성 — 프로젝트 목표, 세션 운영 가이드라인, 워크플로 규칙 통합
- `SESSION_LOG.md` 신규 생성 — 세션 로그 형식 및 운영 방식 정의

**결정사항**:
- `작업기록.md`와 `SESSION_LOG.md`를 분리 유지 — 전자는 파일 변경 이력, 후자는 대화·결정·맥락 중심
- 세션 종료 트리거를 "세션 종료" 키워드로 고정
- 세션 시작 시 SESSION_LOG 읽기를 워크플로 첫 단계로 명시

**미완료 / 다음 TODO**:
- `index.md` 콘텐츠 보강 — 각 프로젝트에 "문제→해결→결과" 형식 및 수치 추가
