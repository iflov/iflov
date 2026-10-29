<p align="center">
  <img src="./assets/readme/hero.svg" width="100%" alt="이현태: TypeScript, Node.js, NestJS로 일하는 백엔드 개발자">
</p>

안녕하세요, 백엔드 개발자 이현태입니다.
사람과의 소통과 커뮤니케이션을 중시하는, 경청하는 개발자입니다.

## 다루는 문제

### 제품 여권과 공급망 데이터 (2026)

- 의류 디지털 제품 여권(DPP)을 여러 사람이 동시에 편집하고 발행하는 서비스. Yjs 실시간 공동 편집, 공장·제품·Lot을 잇는 공급망 그래프
- 같은 도메인의 다른 플랫폼에서 백엔드·프론트엔드·관리자 콘솔·인프라를 맡음. Terraform으로 dev·상용 두 환경과 CodePipeline 배포를 관리하고, 회원 탈퇴·동의 기록·보유 기간이 지난 데이터 자동 파기까지 처리
- 시험성적서를 QR로 연결해 소비자가 바로 확인하고, QR 라벨 발주까지 처리하는 서비스

### 중고 휴대폰 매입·판매 커머스 (2023–2025)

- 매입 신청, 수거 키트 배송, 검수, 입금, 반송으로 이어지는 주문 상태 흐름과 상태마다 나가는 카카오 알림톡
- 정산 엑셀(KST 기준 날짜 필터), 기종별 카테고리 정렬, 은행 점검 시간 예외 처리, 주문 배치 스케줄러
- 사용자 API, 관리자 API, 배치, 웹 클라이언트 네 저장소에 걸쳐 작업

### 구독 결제 (2025)

- PayPal·PortOne 정기결제 생성, 결제 대기(pending) 상태 처리와 그에 따른 구독 취소

### 개발 운영

- Slack으로 들어온 개발 요청을 Jira 작업으로 접수하고 담당자에게 알려 주는 봇 (AWS Lambda, Terraform)

## 직접 만들어 본 것

- [SingRuler](https://github.com/iflov/singruler): 코인노래방 녹음을 pYIN으로 분석해 내 세션 추세를 보여 주고, 출처가 붙은 연습 피드백을 주는 서비스 (GKE, GCS, RAG)
- [auth-server](https://github.com/iflov/auth-server): MCP 클라이언트용 OAuth 2.1 인증 서버. PKCE, 토큰 교환·리프레시·무효화, 감사 로그 (NestJS, Drizzle)
- [barebones](https://github.com/iflov/barebones): DB와 ORM을 고르면 헥사고날 port·adapter 구조와 로컬 관측 스택(Prometheus, Grafana, Loki)까지 만들어 주는 NestJS 스캐폴드
- k6 부하 테스트 플랫폼: 웹 화면에서 k6 테스트를 설정·실행하고 실시간 지표를 보는 도구 (Next.js, Express, InfluxDB, Kubernetes, ArgoCD)

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
