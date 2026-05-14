# Claude Design 프롬프트 — 연제경 Android 개발자 포트폴리오

> 이 파일을 Claude Design(또는 새 Claude 대화)에 그대로 붙여넣어 디자인 초안을 받으세요.

---

## 프롬프트 (복사해서 사용)

---

다음은 Android 개발자 이직용 포트폴리오 사이트의 UI 디자인 초안을 요청하는 프롬프트입니다.

---

### 요청 내용

나는 Android 개발자이고, GitHub Pages(Jekyll)로 운영하는 포트폴리오 사이트의 UI를 새로 디자인하려 한다.
아래의 **내 정보**와 **레퍼런스 방향**을 참고해서 **완성도 높은 단일 HTML 파일** 디자인 초안을 만들어줘.

---

### 내 정보 (콘텐츠)

**이름**: 연제경 (Yeon Je-kyung)  
**직군**: Android Developer  
**연락처**: yllh325@gmail.com / GitHub: yeonchaking / Blog: nockcha-log (티스토리)

#### 소개
Android 앱 개발자로서 기능 구현부터 아키텍처 설계까지 전반을 다루고 있습니다.  
현재는 실시간 영상 처리와 하드웨어 연동(BLE, Camera2) 도메인에서 일하고 있습니다.

#### 경력
**Cybertel | Android Developer**  
2024.07 ~ 현재  
- 경찰청 BodyCam 앱 개발 (Camera2 기반 녹화 파이프라인, H.264/H.265 인코딩, BLE TeamSync)  
- Vodafone GC App 신규 기능 개발 및 UI 최적화  
- MCLoc 앱 기능 개발 및 유지보수

#### 프로젝트
**BodyCam** (경찰청 바디캠 Android 앱)
- Camera2 API 기반 실시간 영상 녹화 파이프라인 설계 및 구현
- H.264 / H.265 하드웨어 인코딩 + MediaMuxer 기반 MP4 저장 처리
- BLE TeamSync 기능 설계 및 구현 (팀원 간 녹화 동기화)

**Vodafone GC App** (기업용 그룹 통신 앱)
- 신규 기능 개발 (기능 상세는 NDA 제약으로 생략)
- 화면/UI 동작 최적화

**MCLoc** (위치 추적 Android 앱)
- Android 앱 기능 개발 및 유지보수

#### 기술 스택
| 분류 | 기술 |
|------|------|
| Language | Kotlin, Java |
| Android | Jetpack, Hilt, Camera2, BLE, MediaMuxer |
| Architecture | MVVM, Clean Architecture |
| Data / Network | Room, SharedPreferences, Retrofit, JSON |
| Tools | Git, Figma |

#### 학력 및 자격증
- 전북대학교 (2014 ~ 2020)
- SSAFY 9기 (2023.01 ~ 2023.12)
- 정보처리기사
- SQLD

---

### 디자인 방향 & 레퍼런스 스타일

**참고 레퍼런스 (이런 느낌으로)**:
- brittanychiang.com — 다크 테마, 사이드바 고정, 섹션별 스크롤, 깔끔한 타이포그래피
- taniarascia.com — 심플하고 가독성 중심, 기술적 신뢰감
- leerob.io — 미니멀 화이트, 콘텐츠 집중형
- read.cv 스타일 — 이력서 느낌의 세로 레이아웃, 여백 중심

**원하는 톤 & 무드**:
- 다크 테마 또는 라이트/다크 토글 지원
- 과도한 애니메이션 없이 — 콘텐츠가 주인공
- 기술력이 느껴지는 단정하고 전문적인 느낌
- 모바일 반응형 필수
- 한국 채용 담당자도 읽기 쉬운 가독성

**레이아웃 아이디어**:
- 상단: 이름 + 직군 + 한줄 소개 + 연락처 링크 (깔끔한 히어로)
- 좌측 고정 사이드바 OR 상단 네비게이션 (Experience / Projects / Skills)
- 기술 스택: 뱃지/태그 형태로 시각화
- 프로젝트: 카드 레이아웃, "문제 → 해결 → 결과" 구조가 눈에 띄게
- 하단 Contact 섹션

**절대 피해야 할 것**:
- 화려한 파티클/웨이브 배경 애니메이션
- 과도한 색상 사용 (2~3색 팔레트 유지)
- 정보보다 비주얼이 앞서는 디자인

---

### 출력 요청

1. **완성된 단일 HTML 파일** — CSS 인라인 포함, 외부 CDN은 Google Fonts / 최소한만
2. Jekyll에서 그대로 쓸 수 있도록 `<body>` 내부 콘텐츠 + `<style>` 블록 형태로도 분리 제공
3. 색상 팔레트, 폰트 선택에 대한 간단한 설명
4. 추가로 개선하면 좋을 UX 포인트 2~3개 제안

---

### 추가 컨텍스트

- 현재 Jekyll + minimal-mistakes 테마 사용 중
- 이 디자인은 기존 테마를 교체하거나 `assets/css/main.scss`에서 override 할 예정
- 완성 후 GitHub Pages(main 브랜치 push)로 자동 배포
- 최종적으로는 한국 IT 기업 채용 담당자에게 보낼 포트폴리오 링크로 사용 예정

---

이 정보를 바탕으로, 내 포트폴리오 사이트의 **디자인 초안 HTML**을 만들어줘.
단순한 레이아웃 스케치가 아니라 실제로 브라우저에서 열어볼 수 있는 완성도 있는 결과물을 원해.
