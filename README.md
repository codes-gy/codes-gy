<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=auto&height=220&section=header&text=Ji%20Geunyeong%20%7C%20Backend%20Developer&desc=Java%2FSpring%20%C2%B7%20Node.js%2FTypeScript&fontSize=28&descSize=16&animation=fadeIn&fontAlignY=38" width="100%"/>
</div>

<br/>

**금융·SI 도메인 실무 4년차 백엔드 개발자**입니다.
Java/Spring과 Node.js/TypeScript로 서비스를 만들고, 쿼리 최적화·보안·동시성 문제를 수치로 개선해 왔습니다.

### 핵심역량

- **금융·결제 도메인**: 보험 상품·계약·대출 비즈니스 로직, 대외기관 연동, 토스페이먼츠 결제·예치금 시스템 개발
- **성능 최적화**: 조인 쿼리 분석·인덱스 튜닝으로 계약/대출 조회 응답 3초 → 2초 미만 단축
- **보안**: 금융 민감정보 마스킹, 개인정보 암호화, API 접근 권한 보완 등 보안 취약점 조치
- **실시간·동시성**: SSE 주문 상태 실시간 동기화, Redis Sorted Set 기반 대기열(p95 113ms), Socket.io 실시간 알림, 멱등성 키 기반 중복 주문 방지
- **설계**: 도메인 이벤트 기반 모듈 연동, ArchUnit으로 강제하는 Layered Architecture
- **인프라·자동화**: Docker, AWS S3, GitHub Actions CI(테스트 병렬화·빌드 캐시), Slack 알림 자동화
- **협업**: PR 리뷰 중심 개발(최소 2인 승인), 기획·디자인·마케팅 직군과의 원활한 커뮤니케이션

---

### 기술 스택

**Language**<br/>
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=OpenJDK&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=Kotlin&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=TypeScript&logoColor=white)

**Backend**<br/>
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=Spring%20Boot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=Spring%20Security&logoColor=white)
![Spring WebFlux](https://img.shields.io/badge/Spring%20WebFlux-6DB33F?style=flat-square&logo=Spring&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=Node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=Express&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=Socket.io&logoColor=white)

**Frontend**<br/>
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=React&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=Next.js&logoColor=white)

**ORM / Data Access**<br/>
![JPA/Hibernate](https://img.shields.io/badge/JPA%2FHibernate-59666C?style=flat-square&logo=Hibernate&logoColor=white)
![MyBatis](https://img.shields.io/badge/MyBatis-B9271C?style=flat-square&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=Prisma&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=Flyway&logoColor=white)

**Database**<br/>
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=PostgreSQL&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=Oracle&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=Redis&logoColor=white)

**Test**<br/>
![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=flat-square&logo=JUnit5&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=Jest&logoColor=white)
![k6](https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white)

**Infra / Tools**<br/>
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=Docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=GitHub%20Actions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=Git&logoColor=white)

---

### 경력사항

**보험사 대고객 홈페이지 운영 및 고도화** · 백엔드 개발 (프리랜서) | *2021.11 ~ 2025.06*
- 계약/대출 조회 쿼리의 조인 구조 분석 및 인덱스 최적화로 **평균 응답 3초 → 2초 미만 (약 33% 단축)**
- 주민등록번호·계좌번호 등 금융 민감정보를 비즈니스 레이어 진입 전에 마스킹하는 유틸리티 구축
- 무결성 검증 로직을 강화해 상품·대출 처리 중 발생하던 정합성 오류를 해소하고, 이후 운영 기간 **재발 0건** 유지

<details>
<summary>상세 보기</summary>

- **주요 직무**
  - 대고객 대표 홈페이지(웹/모바일) 운영, 보험 상품 개정·신규 개발
  - 장기 계약 대출 API 설계·구현 및 대출 원장 반영 파이프라인 개발
  - 본인인증, 타 금융사·대외기관 연동 인터페이스 모듈 개발
- **추가 성과**
  - 대용량 고객 조회 및 보험 청구 처리 프로세스 개선을 위한 RESTful API 재설계 및 쿼리 최적화
  - 개인정보 암호화, API 접근 권한 검증 보완 등 보안 취약점 점검 결과 조치 완료
  - 신규 상품 출시·이벤트 페이지 오픈 시 시스템 안정화 대응
- **사용 기술**: Java, Spring, MyBatis, Oracle, JUnit, TFS

</details>

**고객사 웹/앱 서비스 SI 구축** · 백엔드 개발 | *2021.04 ~ 2021.11*
- 요구사항 분석 기반 DB ERD 설계 및 핵심 비즈니스 로직 RESTful API 개발
- 인덱스 최적화로 핵심 API **평균 응답 시간 30% 단축**
- 에러가 임계치를 넘으면 팀에 즉시 알림을 보내는 모니터링 기능을 구현해, 사용자 문의 전에 장애를 먼저 인지하는 체계 마련

<details>
<summary>상세 보기</summary>

- Swagger 도입으로 API 명세 작성을 자동화하여 화면 설계 변경 시 프론트엔드와의 연동 기간 단축
- 개인정보 암호화, API 접근 권한 미들웨어 보완 등 보안 취약점 점검 결과 조치 완료

</details>

---

### 주요 프로젝트

**[BBCC](https://github.com/prgrms-be-adv-devcourse/beadv8_8_BBCC_BE)** · 팀 프로젝트 (프로그래머스 데브코스 단기심화) | *2026.10 ~ 진행 중*
- **결제·예치금 도메인 담당** (PR 67건)
- 토스페이먼츠 결제 승인·취소·조회 클라이언트와 예치금 충전 요청·승인·취소 API 구현
- 토스에서 직접 취소된 충전을 웹훅으로 동기화하고, 미확정·만료 충전을 스케줄러로 정리해 결제 상태 불일치 방지
- 주문 결제 요청 → 예치금 차감, 주문 취소 → 환불, 정산 지급 → 판매자 입금을 **도메인 이벤트**로 연동하고, 수신 실패 시 재처리
- 공통 기반 설계: 도메인 이벤트 공통 형식, ProblemDetail 오류 응답, 소프트 삭제 엔티티, traceId 로깅 필터, ArchUnit 계층 의존 규칙
- CI 테스트 병렬화·Gradle 빌드 캐시, Flyway 스키마 관리, Slack 배포·이슈 진행률 알림 자동화
- **사용 기술**: Java, Spring Boot, JPA, PostgreSQL, Flyway, Docker, GitHub Actions

**[카페 스마트오더 플랫폼](https://github.com/codes-gy/smart-order)** · 개인 프로젝트 | *2026.08 ~ 2026.09*
- 출근 시간대 몰리는 음료 선주문을 처리하고, 매장의 조리·픽업 상태를 사용자에게 실시간으로 전달하는 스마트오더 서비스
- **SSE**로 주문 상태 변경을 실시간 브로드캐스트하고, 구독 즉시 현재 상태를 보내 재연결 시에도 상태 누락 방지
- 15초 주기 하트비트로 프록시·로드밸런서의 유휴 연결 종료를 막고, 끊긴 연결은 전송 실패 시점에 정리
- **멱등성 키(X-Idempotency-Key)**로 네트워크 재시도에 의한 중복 주문 생성 방지
- 주문 시점의 메뉴명·가격을 스냅샷으로 저장해 메뉴 변경 후에도 과거 주문 이력 정합성 보장
- 카카오·Apple 소셜 로그인 + JWT 기반 Spring Security 인증, Haversine 거리 계산과 커서 페이징으로 주변 매장 조회
- **사용 기술**: Kotlin, Spring Boot, Spring Security, JPA, PostgreSQL, Redis, Flyway, GitHub Actions

**[대규모 트래픽 대기열 시스템](https://github.com/codes-gy/waiting-api)** · 개인 프로젝트
- 티켓 오픈 같은 순간 트래픽이 핵심 DB에 직접 몰리지 않도록 Redis 버퍼 대기열로 받는 시스템
- Redis Sorted Set에 타임스탬프 기반 Score를 부여해 요청 순서대로 대기 순번과 예상 대기 시간 계산
- 순번이 된 사용자에게만 TTL 5분짜리 진입 토큰을 발급하고, 필터에서 검증해 우회 접근 차단
- k6 부하 테스트(최대 300 VUs): **실패율 0.00%, p95 113ms** (목표 200ms 미만 달성)
- **사용 기술**: Java 21, Spring Boot, Spring WebFlux(Netty), Reactive Redis, k6

**WeLive** · 팀 프로젝트 (코드잇 부트캠프) | *2026.04 ~ 2026.05*
- 아파트 입주민과 관리사무소를 잇는 실시간 관리 플랫폼 (권한별 대시보드, 입주민 명부, 민원/투표/공지, 실시간 알림)
- JWT 인증과 슈퍼관리자/관리자/입주민 3단계 역할 기반 인가 미들웨어 구현
- 아파트·동·호수·입주민 명부 관계형 스키마를 설계하고 입주민 자동 가입 승인 로직 구현
- Socket.io로 공지 등록·민원 상태 변경 시 실시간 알림 전송
- 기능 단위 브랜치 전략을 주도하고 `최소 2인 승인 후 머지` 규칙으로 코드 결함 최소화
- **사용 기술**: Node.js, TypeScript, Socket.io, JWT, AWS S3

**[디스코드 봇](https://github.com/codes-gy/discord-bot)** · 개인 프로젝트
- 유튜브 음악 재생, TTS 채널 읽어주기, 서버 유틸리티를 제공하는 디스코드 봇
- 서버별 독립 재생 대기열과 버튼 기반 플레이어 조작(재생/스킵/반복/셔플) 구현
- 음악 재생 중 TTS가 들어오면 음악을 일시정지하고 TTS를 먼저 재생한 뒤 이어서 재생하는 우선순위 인터럽트 처리
- Redis에 채널 설정·사용자별 TTS 언어·재생 통계를 저장해 재시작 후에도 유지
- GitHub Actions로 PR마다 빌드 검증 후 Render에 자동 배포
- **사용 기술**: Node.js, TypeScript, discord.js v14, Redis, esbuild, GitHub Actions

---

### ⚡ 트러블슈팅

<details>
<summary><b>PG 조회 오류를 결제 실패로 확정해 "카드는 결제됐는데 예치금 미입금" 위험</b> · BBCC</summary>

- **문제**: 승인 중인 충전을 토스 조회로 확정하는 과정에서 401(키 교체·누락)이나 429(요청 제한)를 받으면 충전을 되돌릴 수 없는 `FAILED`로 끝냄. 토스에서는 실제로 `DONE`이었다면 카드는 결제됐는데 예치금은 들어오지 않음
- **원인**: 조회 API의 4xx를 모두 "결제 거절"로 해석함. 조회 오류는 결제 상태가 아니라 조회 요청 자체가 실패한 것이라 결과를 확정할 근거가 없음
- **해결**: 결제가 없다는 `NOT_FOUND_PAYMENT`만 거절로 보고, 나머지 4xx와 오류 코드 없는 4xx(프록시·게이트웨이 응답)는 **결과 모름(Unknown)** 으로 분리. 정리 스케줄러가 다음 주기에 다시 조회해 확정하도록 하고, 401·403·429 케이스 테스트 6건 추가 ([PR #355](https://github.com/prgrms-be-adv-devcourse/beadv8_8_BBCC_BE/pull/355))

</details>

<details>
<summary><b>주문 취소 이벤트 처리 실패 시 환불 유실</b> · BBCC</summary>

- **문제**: 주문 도메인의 취소 이벤트를 결제 도메인이 받아 예치금을 환불하는데, 처리 중 예외가 나면 환불이 영영 반영되지 않음
- **원인**: 이벤트 리스너가 한 번 실패하면 다시 처리할 경로가 없었음
- **해결**: 취소 처리를 `REQUIRES_NEW` 트랜잭션으로 분리해 실패분만 롤백하고, 실패한 주문을 재처리 테이블(주문 ID 유니크)에 시도 횟수·마지막 오류와 함께 기록. 1분 주기 스케줄러가 다시 처리하며, 환불 로직이 멱등이라 여러 번 실행돼도 한 번만 반영 ([PR #358](https://github.com/prgrms-be-adv-devcourse/beadv8_8_BBCC_BE/pull/358))

</details>

<details>
<summary><b><code>ddl-auto=update</code>로 어긋난 서버 스키마 때문에 INSERT 실패</b> · BBCC</summary>

- **문제**: dev 서버에서 주문 취소 환불, 구매확정 → 정산 대상 등록 INSERT가 실패
- **원인**: 서버가 `ddl-auto=update`로 기동되면서 엔티티에서 사라진 옛 NOT NULL 컬럼·테이블이 그대로 남아, Flyway로 만든 스키마와 달라짐
- **해결**: dev에 배포된 커밋 39개를 같은 조건으로 차례로 기동해 dev DB 이력을 로컬에서 재현하고, 새 DB와 컬럼·제약·인덱스를 비교해 차이를 찾음. 차이를 맞추는 `IF EXISTS` 마이그레이션을 추가하고 서버를 `ddl-auto=validate`로 전환해 스키마 변경을 Flyway로 일원화 ([PR #376](https://github.com/prgrms-be-adv-devcourse/beadv8_8_BBCC_BE/pull/376))

</details>

<details>
<summary><b>다른 회원의 주문 조회·상태 변경·결제 확정이 가능한 IDOR 취약점</b> · 스마트오더</summary>

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

### 교육

**프로그래머스 · 데브코스 백엔드 단기심화 8기** | *2026.10 ~ 진행 중*
- Java/Spring 기반 팀 프로젝트 [BBCC](#주요-프로젝트) 진행 (결제·예치금 도메인 담당)

**코드잇 · 클라우드 기반 Node.js 엔지니어 부트캠프** | 수료 *(2025.10 ~ 2026.05)*
- Node.js·TypeScript 환경에서 계층형 아키텍처 기반 서버 개발
- 실무형 백엔드 팀 프로젝트 3개 기획·개발 (대표: [WeLive](#주요-프로젝트))
- PR 중심의 팀 코드 리뷰 프로세스, AWS 기반 CI/CD 파이프라인 및 Docker 컨테이너 배포 경험

### 자격증

- **정보처리기사** | 한국산업인력공단 *(2024.09)*
- **SQL 개발자 (SQLD)** | 한국데이터산업진흥원 *(2024.09)*

---

### 연락처

- **Email**: [podojjang_kr@naver.com](mailto:podojjang_kr@naver.com)
- **Blog**: [dev-blog-topaz-rho.vercel.app](https://dev-blog-topaz-rho.vercel.app/)
- **GitHub**: [github.com/codes-gy](https://github.com/codes-gy)

<br/>

<div align="center">
  <b>감사합니다!</b>
</div>
