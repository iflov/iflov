<p align="center">
  <img src="./assets/readme/hero.svg" width="100%" alt="이현태: TypeScript, Node.js, NestJS로 일하는 백엔드 개발자">
</p>

안녕하세요, 백엔드 개발자 이현태입니다.
사람과의 소통과 커뮤니케이션을 중시하는, 경청하는 개발자입니다.

## 하는 일

### 지금 · 2026.08 ~

- 의류 디지털 제품 여권(DPP)을 여러 사람이 동시에 편집하고 발행하는 서비스. Yjs 실시간 공동 편집, 공장·제품·Lot을 잇는 공급망 그래프
- 같은 도메인의 다른 플랫폼에서 백엔드·프론트엔드·관리자 콘솔·인프라를 맡음. Terraform으로 dev·상용 두 환경과 CodePipeline 배포를 관리하고, 회원 탈퇴·동의 기록·보유 기간이 지난 데이터 자동 파기까지 처리
- 시험성적서를 QR로 연결해 소비자가 바로 확인하고, QR 라벨 발주까지 처리하는 서비스
- Slack으로 들어온 개발 요청을 Jira 작업으로 접수하고 담당자에게 알려 주는 봇 (AWS Lambda, Terraform)

### 에이치투비즈 · 2025.12 ~ 2026.04

랜덤 상품 상자 서비스의 백엔드를 혼자 개발하고 운영했습니다.

- 예약 지급에서 포인트만 지급되고 쿠폰이 빠지는 문제를 추적해, 흩어진 DB 연결을 한 커밋 단위로 묶어 수정
- 판매중 상품 4,070건 중 77%가 3개월 넘게 거래되지 않은 것을 확인하고 회수 배치를 개발. 배포 뒤 대조 쿼리로, 로그에는 성공으로 남은 복원 누락 4건을 찾아 보정
- 예약 스케줄러가 멈춘 원인을 node-schedule 내부까지 따라가 찾고 수정 PR 제출

### 인휴먼즈 · 2025.04 ~ 2025.11

- B2B 구독 결제: 해지 신청과 이용 종료 시점이 다른 구독을 6개 상태와 결제 주기별 이력으로 관리. PG 예약은 갱신, 웹훅은 결과 반영, 배치는 해지와 연체 종료를 맡도록 나눔
- WebRTC 얼굴 변환 기술 검증: 브라우저에서 서버 워커를 거쳐 다시 브라우저로 돌아오는 영상 경로를 설계하고 개발 (ZeroMQ, msgpack)
- k6 부하 테스트 플랫폼: 3인 팀에서 백엔드와 인프라 담당. 제어 화면, 실행기, 부하 대상 서버를 나눠 측정 환경을 분리하고 Helm·ArgoCD로 배포

### 21세기전파상 · 2023.03 ~ 2024.10 (이후 2025.07까지 프리랜서로 유지보수)

중고 전자기기 커머스의 사용자 API, 운영 백엔드, 배치 등 서버 4개를 개발하고 유지보수했습니다.

- 여러 서버에서 며칠에 걸쳐 처리되는 매입을 16개 상태로 정의하고, 상태를 바꿀 때마다 필수 입력 검사와 변경 이력 기록
- 재고가 한 개뿐인 중고 상품이라 장바구니 조회와 결제 승인 직전에 가격과 재고를 다시 확인하고, 같은 결제 결과가 두 번 반영되지 않게 차단
- 추천순 상품 목록에서 상품마다 반복되던 주문 집계를 CTE 사전 집계로 변경

자세한 경력은 [블로그 About](https://iflov-github-io.vercel.app/about)에 정리했습니다.

## 최근 글

<!-- BLOG-POST-LIST:START -->
- [다이어그램을 비교했더니 달러 기호가 사라졌다](https://iflov-github-io.vercel.app/blog/archify-delta-dollar-labels) · 2026.09.21
- [exports 한 줄, except 한 줄, 그리고 내가 닫은 PR 하나](https://iflov-github-io.vercel.app/blog/one-line-open-source-contributions) · 2026.08.31
- [WebRTC × ZeroMQ × GPU Worker — 실시간 영상 AI를 클라우드로 옮긴 결정들](https://iflov-github-io.vercel.app/blog/webrtc-zeromq-gpu-worker-distributed-system) · 2026.05.21
- [K6 기반 부하 테스트 플랫폼을 GitOps-ready 구조로 확장하기](https://iflov-github-io.vercel.app/blog/k6-gitops-load-testing-platform) · 2026.05.20
- [node-schedule RecurrenceRule.year를 string으로 넘기면 무한 루프에 빠지는 이슈](https://iflov-github-io.vercel.app/blog/node-schedule-year-string-infinite-loop) · 2026.04.27
<!-- BLOG-POST-LIST:END -->

## 오픈소스

- NestJS TypeORM: CommonJS에서 패키지를 불러오지 못하던 exports 조건 수정 (병합)
- node-schedule: 숫자 문자열 연도를 넣으면 무한 루프에 빠지는 문제 수정, 회귀 테스트 포함 (PR 제출)
- Trail of Bits Skills: 잘못된 UTF-8 캐시 때문에 반복 실패하던 결함 수정 (병합)

## 직접 만들어 보는 것

- [SingRuler](https://github.com/iflov/singruler) (개발 중): 코인노래방 녹음을 pYIN으로 분석해 내 세션 추세를 보여 주고, 출처가 붙은 연습 피드백을 주는 서비스 (GKE, GCS, RAG)
- [auth-server](https://github.com/iflov/auth-server): MCP 클라이언트용 OAuth 2.1 인증 서버. PKCE, 토큰 교환·리프레시·무효화, 감사 로그 (NestJS, Drizzle)
- [barebones](https://github.com/iflov/barebones): DB와 ORM을 고르면 헥사고날 port·adapter 구조와 로컬 관측 스택(Prometheus, Grafana, Loki)까지 만들어 주는 NestJS 스캐폴드

## 기술

#### Backend

<p>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=000000" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js"/>
  <img src="https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white" alt="NestJS"/>
  <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white" alt="Express"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python"/>
</p>

#### Data

<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL"/>
  <img src="https://img.shields.io/badge/Redis-FF4438?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="MongoDB"/>
  <img src="https://img.shields.io/badge/TypeORM-FE0803?style=flat-square&logo=typeorm&logoColor=white" alt="TypeORM"/>
</p>

#### Infra · Ops

<p>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square" alt="AWS"/>
  <img src="https://img.shields.io/badge/Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white" alt="Terraform"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" alt="Kubernetes"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
  <img src="https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white" alt="k6"/>
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" alt="Grafana"/>
</p>

#### Frontend

<p>
  <img src="https://img.shields.io/badge/React-149ECA?style=flat-square&logo=react&logoColor=white" alt="React"/>
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
</p>
