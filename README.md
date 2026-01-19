<div align="center">

# � 모바일 앱 QA 신입 교육 과정

### CVT QA 엔지니어를 위한 4주 완성 커리큘럼

[![Training](https://img.shields.io/badge/Duration-4%20Weeks-blue.svg)](.)
[![Level](https://img.shields.io/badge/Level-Beginner-green.svg)](.)
[![Format](https://img.shields.io/badge/Format-Hands--on-orange.svg)](.)
[![Language](https://img.shields.io/badge/Language-Korean-red.svg)](.)

[Week 1](#-week-1-기초-개념-및-도구-습득) • [Week 2](#-week-2-화면-분해-및-테스트-설계) • [Week 3](#-week-3-결함-발견-및-보고) • [Week 4](#-week-4-실전-cvt-운영) • [Additional Resources](#-추가-교육-자료)

</div>

---

## 📋 과정 소개

본 교육 과정은 **모바일 앱 QA 신입 사원**을 대상으로 하는 **4주 집중 교육 프로그램**입니다.

### ✨ 교육 목표

- 📱 **모바일 앱 QA 기초**: Android/iOS 앱 테스트의 핵심 개념 습득
- 🔍 **체계적 테스트 설계**: UI 분해부터 E2E 시나리오까지 단계별 학습
- 🐛 **결함 관리**: 발견-보고-트리아지-수정 검증의 전체 생명주기 이해
- 🚀 **실전 CVT 운영**: 실제 릴리스 검증 프로세스 시뮬레이션

### 📊 교육 방식

<table>
<tr>
<td width="25%">

#### ⏱️ 학습 시간
**하루 90분**
- 이론: 30분
- 실습: 60분

</td>
<td width="25%">

#### 📅 진행 기간
**총 4주 (20일)**
- 주당 5일 학습
- 주말 복습/과제

</td>
<td width="25%">

#### 🎯 학습 방법
**Hands-on 중심**
- 실제 앱으로 실습
- 매일 산출물 제출

</td>
<td width="25%">

#### ✅ 평가 방식
**산출물 기반**
- 일일 과제
- 주간 프로젝트
- 최종 CVT 리포트

</td>
</tr>
</table>

## 📅 4주 교육 커리큘럼

### 📘 Week 1: 기초 개념 및 도구 습득

**학습 목표**: 모바일 앱 QA의 기본 개념을 이해하고 필수 도구를 활용할 수 있다.

<details>
<summary><strong>📝 상세 커리큘럼 보기</strong></summary>

#### Day 1: 모바일 앱 QA 입문
- 모바일 앱 QA의 역할과 책임
- Android vs iOS 플랫폼 차이점
- QA 생명주기 이해

#### Day 2: 개발 환경 구성
- Android Studio & Xcode 설치
- ADB (Android Debug Bridge) 활용
- iOS 시뮬레이터 & 실기기 연결

#### Day 3: UI 부품 분류 체계
- 6가지 UI 컴포넌트 타입 (Button, Input, List, Dialog, Navigation, Custom)
- 4가지 상태 모델 (Normal, Disabled, Loading, Error)
- 실습: 샘플 앱 UI 분류표 작성

#### Day 4: 테스트 케이스 작성 & 실행
- 테스트 케이스 구조 (Precondition, Steps, Expected Result)
- 테스트 실행 및 결과 기록
- Pass/Fail 판정 기준

#### Day 5: 결함 보고 기초
- 좋은 버그 리포트의 조건
- JIRA/Bugzilla 사용법
- 첫 버그 리포트 작성 실습

#### 📦 주간 산출물
- [ ] 환경 구성 인증서 (스크린샷)
- [ ] UI 분류표 (최소 20개 컴포넌트)
- [ ] 테스트 실행 결과서 (5개 이상 케이스)
- [ ] 버그 리포트 3건 이상
- [ ] Mini-Project: 간단한 앱 전체 화면 UI 분류

</details>

**📄 문서**: [Markdown](CVT_QA_Week1_Detailed.md) | [HTML](CVT_QA_Week1_Detailed.html)

---

### 📗 Week 2: 화면 분해 및 테스트 설계

**학습 목표**: 복잡한 화면을 체계적으로 분석하고 효율적인 테스트를 설계할 수 있다.

<details>
<summary><strong>📝 상세 커리큘럼 보기</strong></summary>

#### Day 6: 화면 라우팅 분석
- Navigation Flow 다이어그램 작성
- 화면 전환 시나리오 (Push, Pop, Replace, Modal)
- 딥링크 & 알림 처리

#### Day 7: 데이터 흐름 추적
- Local Storage vs Server Sync
- 데이터 동기화 오류 패턴
- 캐시 무효화 테스트

#### Day 8: 조합 테스트 설계
- 3축 조합 (플랫폼 × 네트워크 × 로그인 상태)
- 2×2×2 = 8가지 시나리오 테스트
- Pairwise Testing 기법

#### Day 9: E2E 시나리오 작성
- 사용자 여정(User Journey) 정의
- Critical Path 식별
- Happy Path vs Error Path

#### Day 10: 테스트 설계 문서화
- 테스트 계획서 구조
- 테스트 범위 정의
- 리스크 분석 및 우선순위

#### 📦 주간 산출물
- [ ] 화면 플로우 다이어그램 (10개 이상 화면)
- [ ] 데이터 흐름 맵 (3개 이상 기능)
- [ ] 조합 테스트 표 (8가지 시나리오)
- [ ] E2E 시나리오 5개 이상
- [ ] Mini-Project: 실제 앱의 테스트 설계 문서

</details>

**📄 문서**: [Markdown](CVT_QA_Week2_Detailed.md) | [HTML](CVT_QA_Week2_Detailed.html)

---

### 📕 Week 3: 결함 발견 및 보고

**학습 목표**: 체계적인 결함 탐색 방법을 습득하고 효과적으로 보고할 수 있다.

<details>
<summary><strong>📝 상세 커리큘럼 보기</strong></summary>

#### Day 11: 탐색적 테스팅 (Exploratory Testing)
- Session-Based Test Management
- Charter 작성 및 실행
- Time-Boxed Testing

#### Day 12: 재현 가능한 버그 보고
- 7가지 필수 항목 (Title, Steps, Expected, Actual, Environment, Severity, Attachments)
- 100% 재현율 달성 방법
- 스크린 레코딩 & 로그 첨부

#### Day 13: Severity vs Priority
- Severity 4단계 (Critical, High, Medium, Low)
- Priority 3단계 (P0, P1, P2)
- 실전 사례 분석

#### Day 14: 버그 트리아지 시뮬레이션
- 트리아지 회의 역할 (QA, Dev, PM)
- 버그 상태 관리 (Open, In Progress, Fixed, Closed)
- Re-test & Verification

#### Day 15: 리그레션 테스팅
- 리그레션 테스트 체크리스트 작성
- 자동화 vs 수동 테스트 판단
- Side-Effect 탐지 방법

#### 📦 주간 산출물
- [ ] 탐색적 테스팅 Charter 3개 이상
- [ ] 재현 가능한 버그 리포트 5건 이상 (100% 재현율)
- [ ] 트리아지 시뮬레이션 결과
- [ ] 리그레션 테스트 체크리스트 (20개 항목)
- [ ] Mini-Project: 10개 버그 포트폴리오

</details>

**📄 문서**: [Markdown](CVT_QA_Week3_Detailed.md) | [HTML](CVT_QA_Week3_Detailed.html)

---

### 📙 Week 4: 실전 CVT 운영

**학습 목표**: 실제 릴리스 검증 프로세스를 경험하고 CVT 리포트를 작성할 수 있다.

<details>
<summary><strong>📝 상세 커리큘럼 보기</strong></summary>

#### Day 16: CVT 계획 수립
- CVT (Customer Validation Test) 정의
- 테스트 범위 결정 (7가지 핵심 질문)
- 리소스 & 일정 산정

#### Day 17: Smoke Test & Sanity Test
- Smoke Test 체크리스트 (핵심 기능 10개)
- Build Acceptance Test
- 빠른 Go/No-Go 판단

#### Day 18: E2E 테스트 실행
- 우선순위 기반 테스트 실행
- 실시간 이슈 트래킹
- Blocker 이슈 에스컬레이션

#### Day 19: 결함 처리 & 재검증
- 수정된 빌드 검증
- Side-Effect 테스트
- Regression Test 실행

#### Day 20: 최종 리포트 & Go/No-Go 결정
- CVT 결과 요약 (Pass/Fail/Blocked)
- 남은 이슈 리스크 분석
- Go/No-Go 권고안 작성

#### 📦 최종 산출물
- [ ] CVT 테스트 플랜 문서
- [ ] Smoke Test 체크리스트 & 결과
- [ ] E2E 테스트 실행 결과 (30개 이상 케이스)
- [ ] 버그 트리아지 시트 (10건 이상)
- [ ] 재검증 로그 (Side-Effect 포함)
- [ ] **최종 CVT 리포트** (Go/No-Go 결정 포함)

</details>

**📄 문서**: [Markdown](CVT_QA_Week4_Detailed.md) | [HTML](CVT_QA_Week4_Detailed.html)

---

## 📚 추가 교육 자료

### 📖 참고 문서

| 자료명 | 형식 | 설명 | 대상 |
|--------|------|------|------|
| **모바일 앱 결함 분류 체계** | [📄 MD](MOBILE_APP_DEFECT_TAXONOMY.md) / [🌐 HTML](MOBILE_APP_DEFECT_TAXONOMY.html) | 230+ 결함 유형을 7개 카테고리로 분류 | 중급 이상 |
| **모바일 교육자료 #2** | [📄 MD](모바일%20교육자료%20#2.md) / [🌐 HTML](모바일_교육자료_2.html) | 15분 Quick Start 가이드 | 초보자 |

> 💡 **HTML 버전**: Notion/Confluence 스타일로 제공되어 브라우저에서 바로 확인 가능합니다.

### 🛠️ 필수 도구

<table>
<tr>
<td width="50%">

#### Android 개발 환경
- **Android Studio**: 공식 IDE
- **ADB**: 디바이스 제어 도구
- **Logcat**: 실시간 로그 뷰어
- **Scrcpy**: 화면 미러링

</td>
<td width="50%">

#### iOS 개발 환경
- **Xcode**: 공식 IDE
- **Simulator**: iOS 시뮬레이터
- **Console.app**: 로그 분석 도구
- **Instruments**: 성능 프로파일링

</td>
</tr>
<tr>
<td width="50%">

#### 테스트 관리 도구
- **JIRA**: 이슈 트래킹
- **TestRail**: 테스트 케이스 관리
- **Confluence**: 문서화
- **Slack**: 커뮤니케이션

</td>
<td width="50%">

#### 유틸리티
- **Charles Proxy**: 네트워크 모니터링
- **Postman**: API 테스트
- **Git**: 버전 관리
- **VS Code**: 문서 편집

</td>
</tr>
</table>

---

## 🎯 학습 로드맵

```
Week 1 (기초)           Week 2 (설계)           Week 3 (발견)           Week 4 (실전)
    │                       │                       │                       │
    ├─ 도구 숙달            ├─ 화면 분해            ├─ 탐색적 테스팅        ├─ CVT 계획
    ├─ UI 분류              ├─ 데이터 흐름          ├─ 재현 가능 보고       ├─ Smoke Test
    ├─ TC 작성              ├─ 조합 테스트          ├─ 트리아지             ├─ E2E 실행
    ├─ 버그 보고            ├─ E2E 설계             ├─ 리그레션             ├─ 결함 처리
    └─ Mini Project         └─ 테스트 문서          └─ 버그 포트폴리오      └─ 최종 리포트
         │                       │                       │                       │
         └───────────────────────┴───────────────────────┴───────────────────────┘
                               ✅ QA 엔지니어 기본 역량 완성
```

---

## ✅ 학습 체크리스트

교육 과정을 진행하면서 아래 항목을 체크하세요:

### 🔰 기본 역량
- [ ] Android/iOS 디바이스를 개발 환경에 연결할 수 있다
- [ ] ADB 명령어를 사용하여 로그를 수집할 수 있다
- [ ] UI 컴포넌트를 6가지 타입으로 분류할 수 있다
- [ ] 테스트 케이스를 작성하고 실행할 수 있다
- [ ] 재현 가능한 버그 리포트를 작성할 수 있다

### 📊 중급 역량
- [ ] 화면 라우팅 다이어그램을 작성할 수 있다
- [ ] 데이터 흐름을 추적하고 문제를 발견할 수 있다
- [ ] 조합 테스트를 설계할 수 있다 (Pairwise)
- [ ] E2E 시나리오를 사용자 여정 기반으로 작성할 수 있다
- [ ] Severity와 Priority를 정확히 구분할 수 있다

### 🚀 고급 역량
- [ ] 탐색적 테스팅 Charter를 작성하고 실행할 수 있다
- [ ] 버그 트리아지 회의를 진행할 수 있다
- [ ] 리그레션 테스트 전략을 수립할 수 있다
- [ ] CVT 계획을 수립하고 실행할 수 있다
- [ ] Go/No-Go 결정을 위한 리포트를 작성할 수 있다

---

## 💡 학습 팁

<table>
<tr>
<td width="50%">

### 📝 효과적인 학습 방법
1. **매일 실습**: 이론만 읽지 말고 반드시 실제 앱으로 실습
2. **산출물 작성**: 모든 실습 결과를 문서화
3. **질문 기록**: 이해 안 되는 부분은 메모 후 멘토에게 질문
4. **복습**: 주말에 한 주 학습 내용 복습
5. **포트폴리오**: 4주 후 최종 결과물을 정리하여 보관

</td>
<td width="50%">

### ⚠️ 주의사항
- ❌ 이론만 공부하고 실습 생략하지 않기
- ❌ 산출물 대충 작성하지 않기
- ❌ 막히는 부분을 혼자 고민만 하지 않기
- ❌ 하루 학습량을 미루지 않기
- ❌ 버그 리포트를 애매하게 작성하지 않기

</td>
</tr>
</table>

---

## 📞 지원 및 문의

### 🙋‍♂️ 질문이 있으신가요?

- **멘토 문의**: 각 주차별 담당 멘토에게 Slack DM
- **기술 지원**: #qa-training 채널
- **산출물 피드백**: 매주 금요일 1:1 리뷰

### 📊 진도 관리

- **일일 체크인**: 매일 오전 학습 계획 공유
- **주간 리뷰**: 매주 금요일 산출물 제출 및 피드백
- **최종 평가**: Week 4 종료 후 최종 CVT 리포트 평가

---

## 🎓 수료 기준

아래 조건을 모두 충족하면 **CVT QA 엔지니어 교육 과정 수료증**이 발급됩니다:

### ✅ 필수 조건
1. **출석률**: 80% 이상 (16일 이상 참여)
2. **산출물 제출**: 주간 Mini-Project 4개 모두 제출
3. **최종 과제**: Week 4 CVT 리포트 제출 및 통과 (70점 이상)
4. **역량 평가**: 기본 역량 체크리스트 80% 이상 달성

### 🏆 우수 수료자 (90점 이상)
- 사내 QA 블로그 게시 기회
- 차기 교육 과정 멘토 자격
- 추천 이력서 작성 지원

---

## 📜 라이선스

본 교육 자료는 **사내 교육 목적으로만** 사용 가능합니다.

- ✅ 사내 공유 및 복사 허용
- ✅ 개인 학습 및 복습 허용
- ❌ 외부 유출 금지
- ❌ 상업적 사용 금지

---

<div align="center">

### ⭐ 함께 성장하는 QA 엔지니어가 되어봅시다!

Made with ❤️ for CVT QA Engineers

[📧 Contact](mailto:qa-training@company.com) • 
[📚 More Resources](https://wiki.company.com/qa) • 
[💬 Join Slack](https://company.slack.com/qa-training)

</div>


