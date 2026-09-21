# 최수아 · Sooa Choi

**주니어 Technical PM 지향 · AI 서비스 기획자**

사용자 문제를 요구사항·운영정책·측정 지표로 구체화하고, 개발팀과 실제 서비스로 연결합니다.

Lovv, JobPocket, Olfít에서 시장조사·요구사항·UI/UX·트래킹 설계와 프로젝트 운영을 담당했고,
공공 데이터 기반 예측 모델 프로젝트로 한국디지털콘텐츠학회 대학생논문경진대회 은상을 받았습니다.
Python·React·AWS·RAG 구현 경험이 있어 개발팀과 기술적 제약, Trade-off를 구체적으로 논의합니다.

[![Email](https://img.shields.io/badge/Email-choicoa1202@gmail.com-informational?style=flat-square&logo=gmail&logoColor=white)](mailto:choicoa1202@gmail.com)
[![Docs](https://img.shields.io/badge/기획_문서_허브-Lovv_Docs-blue?style=flat-square&logo=github)](https://joraemon-s-secret-gadgets.github.io/oh_my_documents/)

> 아래 모든 프로젝트는 팀 프로젝트이며, **제 수행 범위와 팀 결과**를 구분해 표기했습니다.

---

## 대표 프로젝트

| 프로젝트 | 한 줄 정의 | 수행 역할 |
|---|---|---|
| **[Lovv](https://github.com/Joraemon-s-Secret-Gadgets/Lovv)** | 소도시 여행 추천 서비스 (RAG·Agent 기반 일정 생성) | 서비스 기획 · 사용자 조사 · 운영정책 · 관리자 콘솔 · Backend |
| **[JobPocket](https://github.com/Joraemon-s-Secret-Gadgets/job-pocket)** | RAG 기반 자기소개서 작성 서비스 | PL · 일정·작업 구조 설계 |
| **[Olfít](https://github.com/Joraemon-s-Secret-Gadgets/olfit)** | OOTD 이미지 분석 기반 향수 추천 | PM · 멀티도메인 일정·의존성 관리 |
| **재방문 의향 예측** | 국민여행조사 기반 국내 여행지 재방문 예측 모델 | 데이터 수집·전처리 · 권역 분석 |

---

## 기획 산출물

Lovv의 기획·설계 문서는 **[문서 허브](https://joraemon-s-secret-gadgets.github.io/oh_my_documents/)** 에 공개돼 있습니다.
그중 제가 작성·주도한 문서는 다음과 같습니다.

| 산출물 | 내용 | 링크 |
|---|---|---|
| **이벤트 트래킹 플랜** | 이벤트 25종의 이름·속성·발생 위치, funnel 5단계 검증 지표, 레이턴시 P50·P95, 실패 사유 분류, PII 비저장 정책 | [tracking-plan.md](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/blob/main/docs/95_aha_moment/tracking-plan.md) |
| **사용자 설문 (사전 84명 · 사후 31명)** | 서비스 사용 전 수요 설문과 사용 후 피드백 설문을 각각 설계·배포하고, 결과를 기능 우선순위와 발표 구조로 연결 | [96_market_research](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/tree/main/docs/96_market_research) |
| **Aha Moment UX 설계** | 화면별 설계 문서 + 와이어프레임(HTML) + A/B 재설계안 | [95_aha_moment](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/tree/main/docs/95_aha_moment) |
| **UI/UX 가이드** | 저장 일정 상세·관리자 승인 화면의 구성, 상태, 접근성 규칙 | [09_ui_ux_guide](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/tree/main/docs/09_ui_ux_guide) |
| **B2C 수요 검증 / B2B 수익 모델** | 한일 소도시 여행 수요 검증, 과금 범위·단가, 제휴 전략. 영리화 시나리오와 공익협력안을 분리 | [92_B2C](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/tree/main/docs/92_B2C) · [93_B2B](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/tree/main/docs/93_B2B) |
| **KICK 기능 설계** | 유사 조건 사용자가 공개 일정을 즉시 선택하도록 하는 전환 장치 | [94_kick](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/tree/main/docs/94_kick) |
| **프로젝트 기획서 · 요구사항** | 날씨 정책과 일정 알림 흐름을 요구사항·기획서 전반에 반영, 성공 기준과 사용자 흐름 정렬 | [00_project_plan](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/tree/main/docs/00_project_plan) · [01_requirements](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/tree/main/docs/01_requirements) |

[→ 커밋 기록 전체 보기](https://github.com/Joraemon-s-Secret-Gadgets/oh_my_documents/commits/main?author=sooa02)

---

## 프로젝트 상세

<details>
<summary><b>Lovv — 소도시 여행의 발견 비용을 줄이는 서비스와 운영 시스템 설계</b></summary>

<br>

**문제**
소도시 여행 의향이 있는 여행자도 유명 관광지로 회귀합니다. 목적지를 발견하기 어렵고, 정보가 흩어져 있으며, 신뢰도를 판단하기 어렵고, 추천 결과가 왜 나왔는지 납득하기 어렵기 때문입니다.

**핵심 의사결정 3**

1. **AI 적용 경계를 나눴습니다.** 자연어 의도 해석과 설명 생성에만 LLM을 쓰고, 핵심 선택·라우팅·권한·승인은 결정론적 로직과 정책으로 관리했습니다. 사용자 가치뿐 아니라 재현성·보안·운영 책임을 기준으로 삼았습니다.
2. **운영자 워크플로를 설계했습니다.** `데이터 제안 → 검토 → 승인·거절 → 월간 후보 → 게시 → 서비스 반영 → 이력 확인` 흐름에 역할별 권한, 고위험 작업 승인, MFA, 감사 로그, 실패 작업 재시도, 운영 지표를 붙였습니다.
3. **측정 가능한 제품으로 만들었습니다.** 화면 문서에 흩어져 있던 지표를 이벤트 25종의 단일 트래킹 플랜으로 통합하고, 대화 원문은 저장하지 않고 파생 신호만 담는 프라이버시 기준을 명시했습니다.

**역할 구분**

| 구분 | 내용 |
|---|---|
| 책임 및 기여 | 시장조사, 사전 수요 설문(84명)·사후 피드백 설문(31명) 설계와 배포, B2C/B2B·KICK·Aha Moment 설계, UI/UX 가이드, 이벤트 트래킹 플랜, 관리자 정책·페이지 설계, 발표자료 제작 및 발표, 요구사항·WBS와 GitHub Project/Issue 연결, 백엔드 검증 |
| 팀 결과 | 서비스 구현·배포 (4인 팀) |

**한계**
트래킹 플랜은 설계 단계까지이며, 실사용 로그로 검증한 지표는 아닙니다.


[문서 허브](https://joraemon-s-secret-gadgets.github.io/oh_my_documents/) · [관리자 콘솔](https://github.com/Joraemon-s-Secret-Gadgets/Lovv_admin_web) · [백엔드](https://github.com/Joraemon-s-Secret-Gadgets/Lovv_BE)

</details>

<details>
<summary><b>JobPocket — AI 결과 품질 문제를 제품 과제로 전환한 자기소개서 작성 서비스</b></summary>

<br>

**문제**
생성형 AI가 만든 문장은 사용자의 실제 경험과 멀어지기 쉽고, 한 번에 생성된 결과를 사용자가 통제하기 어렵습니다. 유사 이력서 검색 또한 의미적으로만 비슷하고 직무 키워드를 놓칩니다.

**핵심 의사결정**

- **PL로서 기술 명세를 실행 단위로 전환했습니다.** 기존 에픽 구조를 유지하면서 **신규 Story 17개와 하위 작업 57개**를 배치하고, Gitflow·PR·커밋 추적 체계를 설계해 팀 작업을 추적 가능하게 만들었습니다.
- **검색 품질 문제를 제품 과제로 재정의했습니다.** FAISS 임베딩 유사도만으로는 변별력이 낮다는 점을 발견하고, "유사 이력서 검색"의 목적 자체를 다시 정의한 뒤 BM25와 한국어 형태소 분석(Kiwi)을 결합하는 개선안을 만들었습니다.

> **사용자 결과 품질 문제를 진단하고 개발 가능한 개선 과제로 전환**했다는 점이 이 프로젝트의 핵심입니다.

</details>

<details>
<summary><b>Olfít — 멀티도메인 팀의 실행 구조 설계</b></summary>

<br>

FE·Backend·LLM·DB·Infra가 병렬로 진행되고 외부 AI·임베딩·DB 의존성이 얽힌 프로젝트였습니다.
**6인 · 에픽 10개 · 스토리 44개**의 실행 구조를 운영했습니다.

**직접 책임** — Jira 에픽·스토리 관리, GitHub–Jira–Discord 연동, 저장소 구조·브랜치·PR 규칙, 데일리 스크럼, 요구사항·README·발표자료, 향수 데이터 크롤링, 테스트·논리 정합성 검토

**팀 운영에서 확인한 기준**

- 짧은 일정일수록 기능 수보다 **완료 기준**이 중요합니다.
- 작업 분해는 문서화가 아니라 **충돌 방지 장치**입니다.
- 데이터 부족은 초기에 검증하지 않으면 일정 후반에 발생합니다.

</details>

<details>
<summary><b>재방문 의향 예측 — 국민여행조사 5,386건으로 재방문 결정요인을 해석한 분석 (학회 은상)</b></summary>

<br>

문화체육관광부 국민여행조사 원자료를 활용한 국내 여행지 재방문 의향 예측 모델.
**한국디지털콘텐츠학회 2026 하계종합학술대회 대학생논문경진대회 은상** (2026.07)

**검증된 결과**

| 항목 | 값 |
|---|---|
| 원자료 변수 | 2,227개 → 독립변수 37개 선별 |
| 표본 | 원자료 51,754건 → 목표값 결측 제외 23,863건 → 재방문 의향 4점 제외 최종 5,386건 |
| 분류 기준 | 재방문 의향 5점 = 높음, 1~3점 = 낮음 |
| 평가 데이터 | 별도 테스트셋 1,616건 (팀 Random Forest 분류 모델) |
| 정확도 | 0.88 |
| 소수 클래스(재방문 낮음) 재현율 | 0.86 |
| macro F1 | 0.86 |

**분석에서 도출한 시사점**
재방문 의향은 지출·소득 등 경제적 요인보다 **경험적 만족도**에 압도적으로 좌우되며, 모든 권역에서 만족도 3점 → 4점 구간에 비선형 급상승 임계점이 나타납니다. "보통 만족"은 재방문을 만들지 못합니다.

**직접 책임** — 원본 데이터 수집, 전처리(여행 횟수·1인 지출·성별·연령·가구소득·개인소득), 상관관계 히트맵·VIF 다중공선성 검증, 이상치 시각화, SMOTEENN 적용, SHAP·PDP 기반 변수 관계 평가, 전라권 모델 분석, 발표자료 제작·발표

**한계**
재방문 의향 4점 응답 제외로 인한 표본 선택 편향 · 설문 자기응답 기반이므로 실제 행동이 아닌 "의향" 측정 · 3개 권역 외 일반화 불가 · 단면 데이터라 인과 추론 불가

</details>

---

## 일하는 방식

**기획·협업** — Jira (에픽–스토리–하위작업) · GitHub Projects/Issues · Gitflow·PR 규칙 · 데일리 스크럼 · Figma · Notion

**문서 운영** — 기획 문서를 Markdown 원본과 공유용 배포본으로 분리하고, AI 에이전트가 원본을 읽어 HTML 문서를 생성하는 구조로 운영했습니다.

**기술 이해 범위** — 개발팀과 제약, Trade-off를 논의할 수 있습니다.

| 영역 | 내용 |
|---|---|
| Backend | Python, FastAPI, Django REST, AWS SAM·Lambda·S3·DynamoDB |
| Frontend | React, TypeScript, JavaScript |
| AI | RAG, LangGraph, Agent 파이프라인, 임베딩 검색, BM25·형태소 분석 |
| Data | 대규모 설문 원자료 전처리, EDA, SHAP·PDP, scikit-learn |

---

**Contact** — [choicoa1202@gmail.com](mailto:choicoa1202@gmail.com)
