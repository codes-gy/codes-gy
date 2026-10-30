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

### ⚡ 트러블슈팅

<details>
<summary><b>PG 조회 오류를 결제 실패로 확정해 "카드는 결제됐는데 예치금 미입금" 위험</b> · Kidly</summary>

- **문제**: 승인 중인 충전을 토스 조회로 확정하는 과정에서 401(키 교체·누락)이나 429(요청 제한)를 받으면 충전을 되돌릴 수 없는 `FAILED`로 끝냄. 토스에서는 실제로 `DONE`이었다면 카드는 결제됐는데 예치금은 들어오지 않음
- **원인**: 조회 API의 4xx를 모두 "결제 거절"로 해석함. 조회 오류는 결제 상태가 아니라 조회 요청 자체가 실패한 것이라 결과를 확정할 근거가 없음
- **해결**: 결제가 없다는 `NOT_FOUND_PAYMENT`만 거절로 보고, 나머지 4xx와 오류 코드 없는 4xx(프록시·게이트웨이 응답)는 **결과 모름(Unknown)** 으로 분리. 정리 스케줄러가 다음 주기에 다시 조회해 확정하도록 하고, 401·403·429 케이스 테스트 6건 추가 ([PR #355](https://github.com/prgrms-be-adv-devcourse/beadv8_8_BBCC_BE/pull/355))

</details>

<details>
<summary><b>주문 취소 이벤트 처리 실패 시 환불 유실</b> · Kidly</summary>

- **문제**: 주문 도메인의 취소 이벤트를 결제 도메인이 받아 예치금을 환불하는데, 처리 중 예외가 나면 환불이 영영 반영되지 않음
- **원인**: 이벤트 리스너가 한 번 실패하면 다시 처리할 경로가 없었음
- **해결**: 취소 처리를 `REQUIRES_NEW` 트랜잭션으로 분리해 실패분만 롤백하고, 실패한 주문을 재처리 테이블(주문 ID 유니크)에 시도 횟수·마지막 오류와 함께 기록. 1분 주기 스케줄러가 다시 처리하며, 환불 로직이 멱등이라 여러 번 실행돼도 한 번만 반영 ([PR #358](https://github.com/prgrms-be-adv-devcourse/beadv8_8_BBCC_BE/pull/358))

</details>

<details>
<summary><b><code>ddl-auto=update</code>로 어긋난 서버 스키마 때문에 INSERT 실패</b> · Kidly</summary>

- **문제**: dev 서버에서 주문 취소 환불, 구매확정 → 정산 대상 등록 INSERT가 실패
- **원인**: 서버가 `ddl-auto=update`로 기동되면서 엔티티에서 사라진 옛 NOT NULL 컬럼·테이블이 그대로 남아, Flyway로 만든 스키마와 달라짐
- **해결**: dev에 배포된 커밋 39개를 같은 조건으로 차례로 기동해 dev DB 이력을 로컬에서 재현하고, 새 DB와 컬럼·제약·인덱스를 비교해 차이를 찾음. 차이를 맞추는 `IF EXISTS` 마이그레이션을 추가하고 서버를 `ddl-auto=validate`로 전환해 스키마 변경을 Flyway로 일원화 ([PR #376](https://github.com/prgrms-be-adv-devcourse/beadv8_8_BBCC_BE/pull/376))

</details>

<details>
<summary><b>다른 회원의 주문 조회·상태 변경·결제 확정이 가능한 IDOR 취약점</b> · Smart Order</summary>

- **문제**: 로그인만 하면 `orderId`를 바꿔 다른 회원의 주문과 SSE 스트림을 조회하고, 아무 주문의 상태를 바꾸거나 남의 주문을 결제 완료 처리할 수 있었음
- **원인**: 인증(로그인 여부)만 확인하고 리소스 소유권과 역할(STORE_ADMIN)은 검증하지 않음
- **해결**: JWT principal과 주문의 회원 ID·매장 ID를 비교하는 소유권 검증을 추가하고, 매장 API는 Security 설정에서 STORE_ADMIN으로 제한한 뒤 서비스 계층에서 같은 매장인지 다시 확인. 결제 확정에서는 남의 결제 존재 여부가 드러나지 않도록 404로 응답

</details>

<details>
<summary><b>음성 채널에 들어가지만 소리가 나지 않는 문제</b> · 디스코드 봇</summary>

- **문제**: 봇이 음성 채널에 입장하고 재생 상태도 정상인데 소리가 전혀 들리지 않음
- **원인**: `@discordjs/voice`는 연결이 `Ready`가 되기 전에 보낸 오디오 패킷을 조용히 버리는데, 입장 직후 바로 `player.play()`를 호출함
- **해결**: 연결이 `Ready` 상태가 될 때까지 최대 15초 기다린 뒤 재생하고, 시간을 넘기면 연결을 정리하고 오류를 알림. 배포 로그에 Opus 인코더·암호화 라이브러리 로드 여부(의존성 리포트)를 남겨 같은 증상의 원인을 바로 확인할 수 있게 함

</details>

<details>
<summary><b>오프셋 페이징의 데이터 누락·중복 조회</b></summary>

- **문제**: 오프셋 페이징 중 데이터가 추가·삭제되면 특정 데이터가 누락되거나 중복 조회됨
- **원인**: 조회 사이에 전체 순번이 밀려 이전 페이지 데이터가 다음 페이지에 포함되거나 건너뛰어짐
- **해결**: 식별자 기반 커서 페이징을 도입해 밀림 현상을 없애고, 깊은 페이지에서의 조회 성능도 개선

</details>

<details>
<summary><b>Socket.io Handshake 인증 실패 및 무한 재연결</b></summary>

- **문제**: 일부 클라이언트 환경에서 소켓 인증이 실패하고, 400 에러와 함께 재연결이 무한 반복됨
- **원인**: HTTP 요청용 Passport 인증과 달리 Socket.io Handshake는 전달 구조가 달라 Authorization 헤더의 Bearer 토큰 추출과 예외 처리가 누락됨
- **해결**: Handshake 단계에서 headers의 Bearer 토큰을 직접 추출하는 인증 미들웨어를 추가하고, 실패 시 ExtendedError로 넘겨 클라이언트가 인증 실패를 명확히 받도록 처리

</details>

<details>
<summary><b>로컬 디스크 업로드로 인한 I/O 병목과 컨테이너 재배포 시 파일 유실</b></summary>

- **문제**: 파일 업로드가 몰리면 디스크 I/O 병목으로 다른 API 응답이 지연되고, 컨테이너를 재배포하면 업로드 파일이 사라짐
- **원인**: `multer.diskStorage()`로 서버 로컬 디렉터리에 직접 저장해 디스크 쓰기 부하가 커지고, 컨테이너의 무상태성(Stateless) 원칙에 어긋남
- **해결**: `multer-s3`로 파일 스트림을 AWS S3에 바로 전달해 서버 디스크 I/O를 제거하고 파일 저장소의 지속성 확보

</details>

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
- **Blog**: [dev-blog-topaz-rho.vercel.app](https://dev-blog-topaz-rho.vercel.app/)
- **GitHub**: [github.com/codes-gy](https://github.com/codes-gy)

<br/>

<div align="center">
  <b>감사합니다!</b>
</div>
