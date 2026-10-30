<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=220&section=header&text=Ji%20Geunyeong%20%7C%20Backend%20Developer&desc=Java%20%C2%B7%20Spring%20Backend&fontSize=28&descSize=16&animation=fadeIn&fontAlignY=38" width="100%"/>
</div>

<br/>

보험 · 금융 도메인에서 PG · 은행 연동과 대용량 계약 조회를 맡았던 **Java · Spring 백엔드 개발자**입니다.\
결제 승인 재조회부터 환불 · 정산까지, 실패 흐름을 테스트로 먼저 확인합니다.\
요즘은 AI와 RAG에 관심이 많아, 답이 매번 달라지는 기능도 테스트로 믿을 수 있게 만드는 방법을 찾고 있습니다.

**🔗 포트폴리오 [ji-geunyeong.kro.kr](https://ji-geunyeong.kro.kr/)** · **📄 [이력서 PDF](https://ji-geunyeong.kro.kr/resume.pdf)**

### 핵심 역량

- **보험 · 금융 도메인**: 보험료 가상계좌 입금 매칭, 계약 관리 · 사고접수, 상품 가입 · 보장분석 시스템 개발과 운영
- **결제**: 토스페이먼츠 결제 · 예치금 충전 · 환불 · 정산 흐름, 결과를 모르는 승인을 실패와 따로 다루는 설계
- **성능**: 실행 계획 분석과 복합 인덱스 설계로 계약 목록 조회 4.2초 → 0.6초, 쿼리 재구성으로 보장분석 리포트 3초 → 0.5초
- **동시성 · 정합성**: 멱등 키 + DB 유니크 제약으로 중복 주문 방지, Redis 기반 대기열(k6 가상 사용자 5,000명, p95 3.25ms)
- **설계 · 품질**: 전략 패턴으로 상품 가격 계산 분리(신규 상품 공수 60% 절감), 팀 계층 규칙을 ArchUnit 테스트로 고정
- **자동화 · 협업**: CI job 분리 · 빌드 캐시로 CI 시간 약 28% 단축, PR · MR 승인 규칙 기반 코드 리뷰, 배포 · 작업 요약 슬랙 알림

---

### 기술 스택

<p>
  <img src="https://skillicons.dev/icons?i=java,spring,kotlin,nodejs,postgres,redis,docker,githubactions,aws,nginx,react,nextjs,git&perline=13" alt="Java, Spring, Kotlin, Node.js, PostgreSQL, Redis, Docker, GitHub Actions, AWS, Nginx, React, Next.js, Git"/>
</p>

- **Backend**: **Java · Spring Boot · JPA · MyBatis · Node.js** · QueryDSL · Kotlin · WebFlux · Spring AI
- **Data**: **PostgreSQL** · Redis · Flyway · Oracle
- **Infra**: **Docker · GitHub Actions** · AWS(EC2 · S3) · Nginx · Vercel · Heroku
- **Test**: **JUnit** · Testcontainers · ArchUnit · k6 · Playwright
- **Frontend**: React · Next.js
- **Tools**: **Git · Swagger** · Claude Code

<sub><b>굵은 글씨</b>는 주력 기술</sub>

---

### 경력

**삼동흥산(주)** · Backend Developer (프리랜서) | *2024.07 ~ 2025.06*\
보험 판매 플랫폼 — 보험료 수납 · 계약 관리 · 사고접수 시스템 개발과 운영

- **보험료 가상계좌 입금 매칭**: 계약별 가상계좌 실시간 채번 · 은행 전문 거래 번호로 중복 수신 차단, 금액 불일치 건은 미매칭으로 분류 → 월평균 **1만 건 이상 자동 매칭**, 수작업은 미매칭 건(약 2%)만
- **대용량 계약 조회 Full Table Scan 제거**: 조회 조건 순서에 맞춘 복합 인덱스 설계 · 조건절 컬럼 가공 제거 → 계약 목록 조회 **4.2초 → 0.6초 (86% 단축)**
- **사고접수 연계**: GPS 신호가 약하면 기지국 · Wi-Fi 정보로 위치 보정, 첨부 파일은 파일 헤더로 형식 검사 → 음영지역 테스트 접수 50건 **위치 오차 200m 이내**

**디비에프아이에스** · Backend Developer (프리랜서) | *2021.11 ~ 2024.06*\
보험 판매 플랫폼 — 상품 가입 · 보장분석 · 상담 운영 시스템 개발과 운영

- **보험 상품 가격 계산 전략 패턴 재설계**: 상품별 if-else 계산을 Interface 기반 전략으로 분리 → 신규 상품 추가 공수 **5일 → 2일 (60% 절감)**
- **적합성 자가진단 · 불완전판매 검증**: 진단 결과와 가입 저장을 한 트랜잭션으로 묶고 가산점은 서버에서 계산 → 도입 후 1년간 가입 약 3만 건 **진단 누락 0건**
- **보장분석 리포트 최적화**: 보험사별로 먼저 집계한 뒤 결합하도록 쿼리 재구성 → APM 평균 응답 **3초 → 0.5초 (83% 단축)**

---

### 프로젝트

> 각 프로젝트의 화면 · 흐름도 · 설계 결정은 포트폴리오의 **상세** 링크에서 볼 수 있습니다.

**[Kidly](https://github.com/prgrms-be-adv-devcourse/beadv8_8_BBCC_BE)** — 키즈 패션 이커머스 예치금 결제 · 팀(프로그래머스 데브코스) | *2026.09 ~ 2026.10*
- **결제 도메인 전담 · CI 개선**: 토스페이먼츠 결제 · 예치금 충전 · 환불 · 정산을 도메인 이벤트로 연동
- 한 job에서 차례로 돌던 검사를 정적 검사 · 단위/통합 · 기능 테스트 3개 job으로 나누고 Gradle 빌드 캐시를 켜 **CI 시간 약 28% 단축**
- Java 25 · Spring Boot 4.1 · PostgreSQL 18 · QueryDSL · Flyway · Toss Payments · [상세](https://ji-geunyeong.kro.kr/projects/kidly) · [서비스](https://dev.kidly.kro.kr/)

**[지금이니?!](https://github.com/2609-swyp-team5/swyp)** — 중고 상품 판매 타이밍 추천 · 팀(스위프 웹 15기) | *2026.09 ~ 2026.10*
- **백엔드 — 시세 분석 · AI 연동 · 상품 등록 · 알림**
- 최근 1주일 매물에서 중복 · 구매 글 · 이상값을 거르고 AI로 같은 물건만 고른 뒤, 신뢰도를 매겨 규칙으로 판매 · 구매 시점 추천 — AI가 다르게 답해도 같은 데이터면 같은 추천, 6시간마다 배치 재분석
- Java · Spring Boot 4.1 · Spring AI(Gemini · OpenAI) · PostgreSQL · Redis · Flyway · Playwright · [상세](https://ji-geunyeong.kro.kr/projects/jigeumini) · [서비스](https://www.jigeumini.live/)

**[문단속](https://github.com/codes-gy/mundansok)** — 기업 외부 노출 점검 서비스 · 개인 | *2026.10 ~ 진행 중*
- 공격자와 같은 시선으로 회사 도메인을 먼저 점검해, 노출된 설정 파일 · 만료된 인증서 등 열려 있는 곳과 고치는 방법을 위험도순으로 안내
- Java 21 · Spring Boot 4.1 · Spring Data JPA · Flyway · PostgreSQL · GitHub Actions · [상세](https://ji-geunyeong.kro.kr/projects/mundansok) · [서비스](https://mundansok.vercel.app/)(평일 11:30 ~ 23:00)

**[LineUp](https://github.com/codes-gy/lineup)** — WebFlux · Redis 기반 고성능 대기열 서버 · 개인 | *2026.07*
- 1초마다 내 순번을 보여 주고, 대기를 취소하면 줄에서 바로 빼 뒤 사람들의 순번을 당김 — 입장은 도착 순서대로 분당 약 100명
- k6 부하 테스트(가상 사용자 5,000명): **p95 3.25ms, 실패율 0.00%**
- Java 21 · Spring Boot 4.1 · Spring WebFlux · Reactive Redis · k6 · [상세](https://ji-geunyeong.kro.kr/projects/lineup)

**[Smart Order](https://github.com/codes-gy/smart-order)** — 카페 실시간 선주문 & 픽업 플랫폼 · 개인 | *2026.08 ~ 2026.09*
- 요청마다 **멱등 키**를 받아 같은 키면 이미 만든 주문을 돌려주고, 동시에 들어와도 **DB 유니크 제약**으로 하나만 남김 — 같은 요청을 몇 번 보내도 주문은 하나
- Kotlin · Spring Boot 4.1 · JPA · PostgreSQL · Flyway · Redis · Next.js · [상세](https://ji-geunyeong.kro.kr/projects/smart-order) · [서비스](https://smart-order-eta.vercel.app/)

**[QuantPilot](https://github.com/codes-gy/QuantPilot)** — 전략 기반 주식 자동매매 · 개인 | *2026.09*
- 실시간 시세마다 해당 종목 전략만 골라 이동평균 교차 · 가격 기준으로 매수 · 매도를 판단하고 주문 · 체결 확인 · 손익 반영까지 자동화 — 백엔드 테스트 34개로 검증
- Python 3.12 · FastAPI · SQLAlchemy(async) · Celery · Redis · PostgreSQL · Flutter · [상세](https://ji-geunyeong.kro.kr/projects/quantpilot)

**[위리브](https://github.com/team1-organization/nb07-welive-team1)** — 아파트 관리 · 입주민 소통 플랫폼 · 팀(코드잇) | *2026.03 ~ 2026.05*
- **백엔드 — 인증 · 실시간 알림 · 스키마 · 배포**
- 역할 · 아파트 단위 승인 흐름의 인증 API, 받는 사람별 방으로 보내는 실시간 알림, 반복 조회를 SSE 연결로 전환 — 권한 시나리오 8가지를 통합 테스트로 고정, main 머지 시 자동 배포
- TypeScript · Express 5 · PostgreSQL · Prisma · Socket.io · Jest · AWS(EC2 · S3) · [상세](https://ji-geunyeong.kro.kr/projects/welive) · [서비스](https://nb07-welive-team1.vercel.app/)(평일 11:30 ~ 19:00)

그 밖에: [디스코드 봇](https://github.com/codes-gy/discord-bot) — 유튜브 음악 재생 · TTS 읽어주기 봇(Node.js · TypeScript · discord.js v14 · Redis)

---

### 활동 · 교육

**젝커톤 2026 — 젝트 X 스위프 AI 해커톤** | *2026.11.14 · 참가 예정*
- AI 에이전트로 4시간 동안 MVP를 만드는 바이브톤(주제: 스포츠, 4인 팀)

**프로그래머스 데브코스 백엔드 단기심화 8기** | *2026.09 ~ 진행 중*
- 팀 프로젝트 [Kidly](#프로젝트)(5인)에서 결제 도메인 전담 · 팀 PR 263건 중 66건 작성
- CI · Claude 코드 리뷰 워크플로 구성, 배포 결과 슬랙 알림 · 하루 작업 요약 자동화, 팀 공통 계층 규칙 9개를 ArchUnit 테스트로 고정

**스위프(SWYP) 웹 15기** | *2026.09 ~ 2026.10 · 완료*
- 5인 다직군 팀 프로젝트 [지금이니?!](#프로젝트)에서 백엔드 담당 · 배포 서비스 운영
- 팀 저장소 커밋 387건 중 285건 작성, MR 승인 2명 이상 · 직접 push 금지 규칙, MR마다 도는 GitLab CI(백엔드 테스트 · 프론트 검사 · Playwright e2e)

**코드잇 클라우드 기반 Node.js 백엔드 엔지니어 부트캠프** | *2025.10 ~ 2026.05 · 수료*
- K-Digital Training · 팀 프로젝트 [위리브](#프로젝트)에서 백엔드 담당 · PR 27건 작성, CI 초기 설정 · main 머지 시 배포 자동화 담당

### 학력

**고려사이버대학교 컴퓨터공학과** | *2023.03 ~ 2027.02 (졸업 예정)* · 학점 3.8 / 4.5
- 재직하면서 병행 · 자료구조, 알고리즘, 운영체제, 컴퓨터 네트워크 등 전공 핵심 과목 이수

### 자격증

- **정보처리기사** | 한국산업인력공단 *(2024.09)*
- **SQL 개발자 (SQLD)** | 한국데이터산업진흥원 *(2024.09)*

---

### 연락처

- **Portfolio**: [ji-geunyeong.kro.kr](https://ji-geunyeong.kro.kr/)
- **Email**: [podojjang_kr@naver.com](mailto:podojjang_kr@naver.com)
- **GitHub**: [github.com/codes-gy](https://github.com/codes-gy)

<br/>

<div align="center">
  <b>감사합니다!</b>
</div>
