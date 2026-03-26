# 🌌 Holiverse

## 👑URECA 3기 최종 융합프로젝트 우수상👑

> **고객 데이터 기반 초개인화 통신 서비스 분석 및 추천 플랫폼**  
> 본 프로젝트는 분산된 고객 데이터를 통합하여 사용자에게는 최적의 상품을, 운영자에게는 정교한 비즈니스 인사이트를 제공하는 **CRM/CDP(Customer Data Platform)** 지향 서비스입니다.

---

## 🔗 바로가기

- **기술 문서 / 아키텍처 위키**: [GitHub Wiki](https://one-year-gap.github.io/docs/)
- **프로젝트 문서화**: [Notion](https://oxidized-cornflower-232.notion.site/2fd8a2b69065809fb671d47a8189b846)
- **이슈 / 스프린트 관리**: [Jira](https://tkv00123.atlassian.net/jira/software/projects/HSC/boards/2/timeline?atlOrigin=eyJpIjoiMGE4ZGY1NDVkYzZlNDY1YzgzMTQ2NDA0NmQ2MGM3ZDEiLCJwIjoiaiJ9)
- **API 명세서**: [Postman API](https://documenter.getpostman.com/view/50252872/2sBXcGFLPD)
- **화면 플로우 설계**: [Flow 차트](https://one-year-gap.github.io/docs/2026/03/12/%ED%99%94%EB%A9%B4-%ED%94%8C%EB%A1%9C%EC%9A%B0-%EC%84%A4%EA%B3%84/)
- **백엔드 시스템 아키텍처**: [Architecture Docs](https://one-year-gap.github.io/docs/2026/02/10/%EB%B0%B1%EC%97%94%EB%93%9C-system-architecture/)
- **도메인 아키텍처**: [Domain Architecture](https://one-year-gap.github.io/docs/2026/02/12/%EB%B0%B1%EC%97%94%EB%93%9C-domain-architecture/)
- **인프라 아키텍처**: [Infrastructure Architecture (V1)](https://one-year-gap.github.io/docs/2026/02/24/1%EC%B0%A8-mvp-infrastructure-architecture-v1/)
- **ERD / Flyway 형상 관리**: [ERD & Flyway Docs](https://one-year-gap.github.io/docs/2026/03/13/erd-%EC%84%A4%EA%B3%84-%EB%B0%8F-flyway-%EA%B8%B0%EB%B0%98-db-%ED%98%95%EC%83%81-%EA%B4%80%EB%A6%AC/)

---

## 📚 목차

1. [📌 프로젝트 소개](#-프로젝트-소개)
2. [🎯 프로젝트 목표와 규모](#-프로젝트-목표와-규모)
3. [🛠️ Tech Stack](#️-tech-stack)
4. [🖥️ Service UI](#️-service-ui)
   - [User Interface (B2C)](#user-interface-b2c)
   - [Admin Interface (B2B)](#admin-interface-b2b)
   - [화면 플로우 설계](#-화면-플로우-설계)
5. [📌 핵심 기능 (Core Features)](#-핵심-기능-core-features)
   - [상담 분석 기능](#상담-분석-기능)
   - [로그 수집 기능](#로그-수집-기능)
   - [캐릭터 배치 기능](#캐릭터-배치-기능)
   - [개인별 추천 기능](#개인별-추천-기능)
   - [이탈률 계산 기능](#이탈률-계산-기능)
6. [🏗️ 백엔드 시스템 아키텍처](#️-백엔드-시스템-아키텍처)
7. [🏗️ 도메인 아키텍처](#️-도메인-아키텍처)
8. [🏗️ 인프라 아키텍처](#️-인프라-아키텍처)
9. [🗂️ ERD 설계 및 Flyway 기반 DB 형상 관리](#️-erd-설계-및-flyway-기반-db-형상-관리)
10. [⚖️ 기술 선택 근거 (Technical Decisions)](#️-기술-선택-근거-technical-decisions)
    - [Kafka 사용 이유](https://github.com/one-year-gap/.github/blob/main/profile/README.md#%EC%B9%B4%ED%94%84%EC%B9%B4-%EB%8F%84%EC%9E%85-%EC%9D%B4%EC%9C%A0--:~:text=%EC%B9%B4%ED%94%84%EC%B9%B4%20%EB%8F%84%EC%9E%85%20%EC%9D%B4%EC%9C%A0,%EC%95%88%EC%A0%95%EC%A0%81%EC%9C%BC%EB%A1%9C%20%EC%A0%81%EC%9E%AC%ED%95%98%EA%B3%A0%2C%20%EB%8F%99%EC%8B%9C%EC%97%90)
11. [🚀 추후 확장 가능성](#-추후-확장-가능성)
12. [👥 팀 역할 소개](#-팀-역할-소개)

---

# 📌 프로젝트 소개

**HOLLIVERSE**는 통신 서비스 이용 데이터를 기반으로 고객 행동을 분석하고 운영자가 고객을 더 쉽게 이해할 수 있도록 돕는 분석 플랫폼입니다.  
또한 분석에 이어서, 고객의 특성에 맞춰 개인별로 맞춤형 추천을 해 **실질적 액션과 수익으로 이어지는 서비스**를 목표로 합니다.

이 프로젝트는 다음과 같은 핵심 기능을 목표로 설계되었습니다.

- **통합 데이터 뷰**: 산재한 고객 정보를 특성별로 분류하고 조회할 수 있는 기능
- **행동 기반 분석**: 실시간 상담 로그와 사용패턴 기반의 이탈 예측과 추천
- **Actionable Insight**: 분석에 그치지 않고 추천, 알림, 쿠폰 등 실질적인 서비스 액션으로 연결

---

# 👥 팀원

<h2>Backend</h2>
<table>
  <tr>
    <td align="center" width="220">
      <img src="https://avatars.githubusercontent.com/bon0512?v=4" width="120" height="120"/><br/>
      <b>구본문</b><br/>
      <a href="https://github.com/bon0512">@bon0512</a><br/><br/>
      <sub>팀장</sub><br/>
      <sub>캐릭터배치, 로그파이브라인 적재과정 구축</sub>
    </td>
    <td align="center" width="220">
      <img src="https://avatars.githubusercontent.com/tkv00?v=4" width="120" height="120"/><br/>
      <b>김도연</b><br/>
      <a href="https://github.com/tkv00">@tkv00</a><br/><br/>
      <sub>INFRA</sub><br/>
      <sub>이탈률 설계 및 파이프라인 구축</sub>
    </td>
    <td align="center" width="220">
      <img src="https://avatars.githubusercontent.com/rettooo?v=4" width="120" height="120"/><br/>
      <b>최하영</b><br/>
      <a href="https://github.com/rettooo">@rettooo</a><br/><br/>
      <sub>로그 파이프라인 구축</sub><br/>
       <sub>추천 LLM 구축</sub>
    </td>
    <td align="center" width="220">
      <img src="https://avatars.githubusercontent.com/YeongHyeonHeo?v=4" width="120" height="120"/><br/>
      <b>허영현</b><br/>
      <a href="https://github.com/YeongHyeonHeo">@YeongHyeonHeo</a><br/><br/>
      <sub>데이터베이스 구축 및 유지보수</sub><br/>
       <sub>상담 키워드 분석 시스템 구축</sub>
    </td>
  </tr>
</table>

<h2>Frontend</h2>
<table>
  <tr>
    <td align="center" width="220">
      <img src="https://avatars.githubusercontent.com/dahlia0916?v=4" width="120" height="120"/><br/>
      <b>이수빈</b><br/>
      <a href="https://github.com/dahlia0916">@dahlia0916</a><br/><br/>
      <sub>클라이언트 로깅, 지역별 통계, 로그인 api 연동</sub>
    </td>
    <td align="center" width="220">
      <img src="https://avatars.githubusercontent.com/Zoo2-bi?v=4" width="120" height="120"/><br/>
      <b>박주이</b><br/>
      <a href="https://github.com/Zoo2-bi">@Zoo2-bi</a><br/><br/>
      <sub>상품,추천,고객특성,상담이력 api 연동</sub>
    </td>
    <td align="center" width="220">
      <img src="https://avatars.githubusercontent.com/joonhyong?v=4" width="120" height="120"/><br/>
      <b>박준형</b><br/>
      <a href="https://github.com/joonhyong">@joonhyong</a><br/><br/>
      <sub>마이,메인,캐릭터유형,이탈률,고객관리 api 연동</sub>
    </td>
  </tr>
</table>



---

# 🎯 프로젝트 목표와 규모

우리는 **일간 방문자 수 3만 명(DAU 30K)** 처리를 목표로 시스템을 설계하였습니다.

## 서비스 트래픽 산출 근거

   <img width="2816" height="1536" alt="Gemini_Generated_Image_3flk2n3flk2n3flk (1)" src="https://github.com/user-attachments/assets/e0e20263-7dd2-4559-82fc-778b15ba527a" />



- **통신사 규모:** LG U+ 모바일 가입자(약 1,100만 명) 및 5G 성장세 기반
- **실제 웹 트래픽:** 공식 채널 월 방문자 약 1,100만 명(일 평균 30만 명) 데이터 활용
- **타겟 고객 설정:** 요금제 탐색/조회 관련 사용자 비중(30%)을 고려하여 **잠재 고객 10만 명** 설정
- **최종 목표:** 잠재 고객 중 활성 사용자 비율 30%를 적용하여 **DAU 3만 명, MAU 100만 명**을 안정적으로 수용하는 아키텍처 구축

---

## 🛠️ Tech Stack

## 💻 Frontend

<p>
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white">
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white">
  <img src="https://img.shields.io/badge/TanStack_Query-FF4154?style=for-the-badge&logo=react-query&logoColor=white">
  <img src="https://img.shields.io/badge/Zustand-443E38?style=for-the-badge&logo=react&logoColor=white">
</p>

- **Next.js (SSR/CSR):** 초기 로딩/SEO와 인터랙션을 함께 고려한 렌더링 구조
- **TypeScript:** 정적 타입 기반 안정적인 UI/데이터 모델링
- **Tailwind CSS:** 빠른 UI 제작 및 일관된 디자인 시스템
- **TanStack Query:** 서버 상태 캐싱/동기화, API 호출 표준화
- **Zustand:** 전역 상태 관리(인증 상태, UI state 등)

---

## ⚙️ Backend (Java / Spring)

<p>
  <img src="https://img.shields.io/badge/Java_17-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white">
  <img src="https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">
  <img src="https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white">
  <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white">
  <img src="https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white">
</p>

- **Core:** Java 17, Spring Boot 3.x, Spring MVC (Validation 기반 요청 검증)
- **Security:** Spring Security, JWT, Spring OAuth2 Client (자체 토큰 및 소셜 로그인)
- **Data Access:** Spring Data JPA (Hibernate), **jOOQ** (통계용 타입 세이프 SQL)
- **Batch/Event:** Spring Batch (일 단위 세그먼트 산출), Spring Kafka (이벤트 기반 비동기 처리)
- **Util:** MapStruct (DTO 매핑), **TSID** (시간 정렬 가능 고유 ID 전략)

---

## 🤖 AI / LLM Engine (Python)

<p>
  <img src="https://img.shields.io/badge/Python_3.11-3776AB?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white">
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white">
  <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white">
</p>

- **Framework:** Python 3.11, FastAPI, Uvicorn (비동기 고성능 서버)
- **AI/NLP:** LangChain, OpenAI, spaCy (한글 토큰화), rapidfuzz (텍스트 매칭 최적화)
- **Streaming:** aiokafka (실시간 로그 수집), AWS MSK IAM Auth 연동

---

## 🗄️ Data / Storage

<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white">
  <img src="https://img.shields.io/badge/H2_Database-00519E?style=for-the-badge&logo=sqlite&logoColor=white">
  <img src="https://img.shields.io/badge/Flyway-CC0000?style=for-the-badge&logo=flyway&logoColor=white">
  <img src="https://img.shields.io/badge/Amazon_S3-FF9900?style=for-the-badge&logo=amazons3&logoColor=white">
</p>

- **RDBMS:** PostgreSQL (핵심 트랜잭션), pgvector (벡터 임베딩 및 유사도 검색)
- **Management:** Flyway (스키마 이력 관리), jOOQ Codegen

---

## ☁️ Infra / DevOps / Observability

<p>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white">
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white">
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white">
</p>

- **Infra:** AWS SDK v2, AWS Secrets Manager, AWS X-Ray (분산 트레이싱)
- **DevOps:** Docker (Multi-stage build), GitHub Actions (CI/CD 파이프라인)
- **Observability:** Spring Boot Actuator, Micrometer, Prometheus, Jacoco

---

## 🤝 Collaboration

> 프로젝트 협업 문서와 이슈를 아래 링크에서 바로 확인할 수 있습니다.

- **[Notion](https://oxidized-cornflower-232.notion.site/2fd8a2b69065809fb671d47a8189b846):** 문서화 및 프로젝트 지식 베이스 구축
- **[Jira](https://tkv00123.atlassian.net/jira/software/projects/HSC/boards/2/timeline?atlOrigin=eyJpIjoiMGE4ZGY1NDVkYzZlNDY1YzgzMTQ2NDA0NmQ2MGM3ZDEiLCJwIjoiaiJ9):** 애자일 스프린트 관리 및 이슈 트래킹
- **[GitHub Wiki](https://one-year-gap.github.io/docs/):** 기술 명세서 및 트러블슈팅 가이드 관리
- **[Postman API](https://documenter.getpostman.com/view/50252872/2sBXcGFLPD):** API 명세서
- **ErdCloud:** ERD 공유 문서

---

## 🖥️ Service UI

## User Interface (B2C)

Holiverse의 고객 화면은 **메인 분석, 상품 조회·비교, 캐릭터 페르소나, 마이페이지**로 구성되어 있습니다.

| 메인 / 분석 | 상품 조회 / 비교 | 캐릭터 페르소나 | 마이페이지 |
| --- | --- | --- | --- |
| <img src="https://github.com/user-attachments/assets/ebe31f67-754d-43fd-8aca-fca3ef78bc6b" width="180"/> | <img src="https://github.com/user-attachments/assets/38c5060e-1e13-4113-86fd-41b4da198257" width="180"/> | <img src="https://github.com/user-attachments/assets/fd4828d1-850c-4e30-bc52-1a62984f55fc" width="180"/> | <img src="https://github.com/user-attachments/assets/42efcc20-3e4e-4265-9b38-45ab1301f1da" width="180"/> |

- **메인 / 분석:** 데이터·통화·문자 사용량과 예상 요금을 한 화면에서 확인
- **상품 조회 / 비교:** 5G/LTE, 부가서비스 등 필터 기반 요금제 조회 및 현재 요금제와 비교
- **캐릭터 페르소나:** 사용 패턴 기반 캐릭터를 통해 자신의 이용 성향을 직관적으로 이해
- **마이페이지:** 보유 요금제/혜택, 쿠폰 보유 내역 등을 한 번에 관리

---

## Admin Interface (B2B)

운영자는 웹 기반 관리자 화면에서 고객/지역/상담/이탈 정보를 한 눈에 모니터링할 수 있습니다.

- **고객 통합 관리:** 필터·검색을 통해 고객을 조회하고, 등급별 분포와 월간 데이터 사용량 차트를 제공합니다.
- **지역별 통계:** 지도 기반으로 지역별 ARPU와 데이터 사용량을 시각화하고, 클릭/호버로 상세 지표를 확인합니다.
- **고객 특성 분석:** 고객 유형별 분포와 유형별 요금제 사용 패턴을 그래프로 확인합니다.
- **상담 이력 분석:** 상담 키워드 버블 차트와 시간·요일별 상담 트래픽을 통해 주요 이슈와 피크 타임을 파악합니다.
- **이탈 예측 대시보드:** 이탈 위험 고객 목록, 증감 추이, 실시간 이탈 신호를 모니터링하여 선제 대응이 가능합니다.

---

## 📐 화면 플로우 설계

자세한 플로우 화면은 아래 문서를 참고해주세요.

- **[Flow 차트 바로가기](https://one-year-gap.github.io/docs/2026/03/12/%ED%99%94%EB%A9%B4-%ED%94%8C%EB%A1%9C%EC%9A%B0-%EC%84%A4%EA%B3%84/)**

---
## 🏗️ 백엔드 시스템 아키텍처

> 아래와 같이 주요 기술적 고민 및 선택 과정을 아키텍처 설계 문서의 형태로 체계적으로 정리하였습니다.  
> 📖 **[아키텍처 상세 Docs 바로가기](https://one-year-gap.github.io/docs/2026/02/10/%EB%B0%B1%EC%97%94%EB%93%9C-system-architecture/)**

## ✅ 주요 고민 리스트

| # | 고민 내용 |
| --- | --- |
| 1 | **배포 단위 및 시스템 설계**<br>기능(도메인)별 서비스 분리 여부, 단일/멀티 모듈 구조 결정 |
| 2 | **DB/배포 분리 기준**<br>각 서비스의 데이터베이스 분리 또는 통합, 배포 단위 최적화 방안 |
| 3 | **비용 최적화**<br>7주 프로젝트 기간 내에 개발/스테이징/운영 환경을 60만원 예산으로 구축 |
| 4 | **DDD 적용**<br>이전 경험을 바탕으로 현실적으로 적용 가능한 도메인 중심 설계안 검토 |

## ⬇️ 아키텍처 설계 결론

최적의 시스템 성능 및 운영 효율성을 확보하기 위해, 본 프로젝트에서는 **명령(Command) 및 트랜잭션성 작업은 JPA를, 복잡한 집계·추천과 대량 처리는 jOOQ로 분리(CQRS적 접근)**하는 구조적 전략을 채택하였습니다.

> **요약**  
> 주요 트랜잭션(OLTP)은 높은 생산성을 제공하는 JPA를 활용하고, 대용량 분석/집계/추천(OLAP)은 SQL 구문 제어 및 성능 튜닝이 용이한 jOOQ를 별도로 적용함으로써, 각 기술의 장점을 극대화할 수 있도록 시스템을 설계하였습니다.

이와 같은 구조는 다음과 같은 아키텍처적 의도를 기반으로 합니다.

- 단일 ORM(JPA) 체계에서 모든 처리를 진행할 때 발생하는 성능 이슈, 트래픽 추적 한계, 복잡성 증가 등의 문제를 해소하기 위함
- 명령/조회 업무를 기술 특성에 따라 역할별로 분리하여, 코드의 유지보수성과 시스템 확장성을 높임
- 핵심 트랜잭션 관리의 일관성과 분석/추천을 위한 집계 로직의 성능 튜닝 유연성 동시 확보

즉, **CQRS(Command-Query Responsibility Segregation) 원칙을 고려하여, 비즈니스 도메인 별 역할에 적합한 기술 조합을 전략적으로 배치**한다는 점을 아키텍처 설계의 핵심 결론으로 도출할 수 있습니다.

---

## 🏗️ 도메인 아키텍처

> 상세한 설계 과정과 전체 내용은 📖 **[백엔드 Domain Architecture 문서](https://one-year-gap.github.io/docs/2026/02/12/%EB%B0%B1%EC%97%94%EB%93%9C-domain-architecture/)** 에 정리했습니다.

이 아키텍처의 핵심 목표는 **customer 트래픽 폭주로 인해 admin 기능까지 같이 다운되지 않도록, 런타임/리소스를 강하게 분리하면서도 코드베이스는 하나로 유지하는 것**입니다.

- **핵심 문제 정의:** 고객 트래픽이 몰리면 동일 런타임에 있는 admin API도 같은 스레드/커넥션 풀, DB 병목에 의해 함께 장애가 날 수 있습니다.
- **코드 하나 + 런타임 둘:** 코드베이스는 하나이지만, `customer-api-service` / `admin-api-service` 두 개의 ECS 서비스로 분리 배포하여 CPU, 메모리, 커넥션 풀을 물리적으로 분리합니다.
- **Profile 역할 정리:** `SPRING_PROFILES_ACTIVE=customer/admin` 은 “어떤 기능/설정만 켤지”를 제어하는 용도이며, **실제 장애/트래픽 분리는 인프라(ECS, 라우팅)** 가 담당합니다.
- **경계 강제(Guarding):** 코드(@Profile, Port/Adapter), 런타임(host guard/filter), CI(ArchUnit 규칙), DB(role·schema 분리) 레벨에서 cross-access를 막아 실수를 구조적으로 줄입니다.
- **확장/승격 전략:** 처음에는 단일 RDS + 스키마/권한 경계로 시작하고, 모니터링 지표(p95 latency, pool usage, DB load 등)를 보고 필요 시 read replica 분리, 배치/추천 서비스 분리 등으로 단계적으로 승격합니다.

전체 아키텍처 다이어그램은 아래와 같습니다.

<img src="/Users/haing/Ureka/최종 프로젝트/.github/profile/Billing Cycle Gate Flow-2026-02-12-013948.svg" width="1000">

---

## 🏗️ 인프라 아키텍처

이 인프라는 **고객 웹(Vercel)**, **운영·비즈니스 API(AWS ECS)**, **데이터 계층(RDS)** 를 명확히 분리하고,  
외부에 직접 노출되는 자원(ALB, DNS)과 VPC 내부에서만 동작해야 하는 워크로드를 네트워크 레벨에서 구분하는 것을 목표로 합니다.

- **도메인/트래픽 분리:**  
  루트 도메인은 Vercel(고객 웹)로, `api.<domain>` 은 Customer ALB → Customer API ECS,  
  `admin.<domain>` 은 Admin ALB → Admin Web/Admin API 로 분기하여 **고객/관리자 경계를 네트워크에서 먼저 분리**합니다.
- **VPC·서브넷 구조:**  
  하나의 VPC 안에서 **PUBLIC 서브넷(ALB)** 과 **PRIVATE 서브넷(ECS, RDS)** 로 나누어,  
  애플리케이션/DB는 인터넷에서 직접 접근할 수 없고 ALB나 내부 서비스만 통해 접근하도록 설계했습니다.
- **보안 그룹/최소 권한:**  
  Customer ALB, Customer API, Admin ALB, Admin Web, Admin API, DB에 **역할별 Security Group** 을 부여하여  
  “같은 VPC 안이라서 다 보인다”를 막고, **누가 누구에게 어떤 포트로 접근 가능한지 명시적으로 제어**합니다.
- **Admin 폐쇄성 강화:**  
  Admin ALB 인바운드는 `ADMIN_ALLOWED_CIDRS` 에 포함된 IP만 허용하고, Admin API는 외부에 직접 노출하지 않아  
  **관리자 콘솔을 제한된 네트워크에서만 사용하는 폐쇄형 운영 시스템**으로 유지합니다.
- **모니터링/운영:**  
  전용 EC2에 Grafana + Prometheus + pg_exporter를 두고 CloudWatch와 연동해  
  **애플리케이션·DB·AWS 인프라 메트릭을 한 곳에서 관측**하며, 접근은 SSM Port Forwarding으로만 허용해  
  **모니터링 시스템 자체도 내부망 + IAM/Secrets 기반**으로 안전하게 운영합니다.

> 상세한 인프라 구성과 설계 배경은 아래 문서에 정리했습니다.  
> - [AWS CDK(Java)를 선택한 이유](https://one-year-gap.github.io/docs/2026/02/10/aws-cdk-with-java%EB%A5%BC-%EC%84%A0%ED%83%9D%ED%95%9C-%EC%9D%B4%EC%9C%A0/)  
> - [Network Architecture](https://one-year-gap.github.io/docs/2026/03/17/infra-architecture-network/)  
> - [CI/CD/CT Architecture](https://one-year-gap.github.io/docs/2026/03/17/infra-architecture-ci-cd-ct/)

---

## 🗂️ ERD 설계 및 Flyway 기반 DB 형상 관리

이 프로젝트의 데이터 모델은 **member(고객)를 중심으로 상품, 상담, 캐릭터, 쿠폰, 최근 본 상품, 리프레시 토큰**까지  
핵심 도메인을 모두 포함하는 ERD를 먼저 설계한 뒤, **모든 스키마 변경을 Flyway 마이그레이션으로만 관리**하는 전략을 사용합니다.

## ERD 설계 방향

- `member`를 중심으로 `상품`, `상담 이력`, `상담 키워드`, `캐릭터 유형`, `쿠폰`, `최근 본 상품`, `리프레시 토큰` 관계를 명시적으로 정의해  
  **고객 여정(가입→이용→상담→혜택/추천)** 이 하나의 데이터 모델 위에서 추적되도록 설계했습니다.
- 온라인 트랜잭션(로그인/조회/변경)과 배치/분석용 데이터는 스키마와 테이블 단위에서 역할을 분리하여,  
  **실시간 API 성능과 배치 처리 안정성**을 동시에 확보하는 것을 목표로 합니다.

## Flyway 기반 형상 관리 전략

- `DDL` 변경은 수동 쿼리가 아니라, **`V1__init.sql`, `V2__add_coupon_table.sql`** 과 같은 Flyway 버전 마이그레이션으로만 수행합니다.
- 모든 환경(로컬/스테이징/프로덕션)은 **동일한 마이그레이션 히스토리**를 따라가도록 강제하여,  
  “환경마다 스키마가 다른” 상황을 구조적으로 방지합니다.
- 스키마 변경 시에는 **새 컬럼 추가 → 코드 반영 → 구 컬럼 제거** 순으로 점진적으로 진행하여,  
  배포 중에도 애플리케이션과 DB 간의 호환성을 유지할 수 있도록 합니다.

> ERD 설계 상세와 실제 마이그레이션 파일 구조는 📖  
> **[ERD 설계 및 Flyway 기반 DB 형상 관리](https://one-year-gap.github.io/docs/2026/03/13/erd-%EC%84%A4%EA%B3%84-%EB%B0%8F-flyway-%EA%B8%B0%EB%B0%98-db-%ED%98%95%EC%83%81-%EA%B4%80%EB%A6%AC/)** 문서에 정리되어 있습니다.

---

## 📌 핵심 기능 (Core Features)

## 상담 분석 기능

상담 데이터를 정형화하여 고객 이슈를 더 빠르게 파악하고, 운영자가 대응 우선순위를 판단할 수 있도록 돕습니다.

- [키워드 추출 라이브러리 선택 - 성능 지표 테스트](https://one-year-gap.github.io/docs/2026/02/28/%ED%82%A4%EC%9B%8C%EB%93%9C-%EC%B6%94%EC%B6%9C-%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC-%EC%84%A0%ED%83%9D-%EC%84%B1%EB%8A%A5-%EC%A7%80%ED%91%9C-%ED%85%8C%EC%8A%A4%ED%8A%B8/)
- [키워드 매핑 라이브러리 선택 - 성능 지표 테스트](https://one-year-gap.github.io/docs/2026/02/28/%ED%82%A4%EC%9B%8C%EB%93%9C-%EB%A7%A4%ED%95%91-%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC-%EC%84%A0%ED%83%9D-%EC%84%B1%EB%8A%A5-%EC%A7%80%ED%91%9C-%ED%85%8C%EC%8A%A4%ED%8A%B8/)
- [키워드 추출 & 매핑 알고리즘 설계 전략](https://one-year-gap.github.io/docs/2026/03/12/%ED%82%A4%EC%9B%8C%EB%93%9C-%EC%B6%94%EC%B6%9C-%EB%A7%A4%ED%95%91-%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-%EC%84%A4%EA%B3%84-%EC%A0%84%EB%9E%B5/)
- [감정 분석 모델 선택 - 성능 지표 테스트](https://one-year-gap.github.io/docs/2026/03/14/감정-분석-모델-선택-성능-지표-테스트/)

---

## 로그 수집 기능

사용자 행동 로그를 구조적으로 수집하고, 이후 추천·분석·최근 본 상품 기능까지 연결될 수 있도록 설계하였습니다.

- [로그 파이프라인 1 - 로그 및 템플릿 설계](https://one-year-gap.github.io/docs/2026/03/12/%EC%A0%84%EC%B2%B4-%EB%A1%9C%EA%B7%B8-%ED%8C%8C%EC%9D%B4%ED%94%84%EB%9D%BC%EC%9D%B8-1/)
- [로그 파이프라인 2 - 클라이언트 로그 적재 장소로 S3 도입 이유](https://one-year-gap.github.io/docs/2026/03/13/%ED%81%B4%EB%9D%BC%EC%9D%B4%EC%96%B8%ED%8A%B8-%EB%A1%9C%EA%B7%B8-%EC%A0%81%EC%9E%AC-%EC%9E%A5%EC%86%8C%EB%A1%9C-s3-%EB%8F%84%EC%9E%85-%EC%9D%B4%EC%9C%A0/)
- [로그 파이프라인 3 - 최근 본 상품 조회](https://one-year-gap.github.io/docs/2026/03/13/%EB%A1%9C%EA%B7%B8-%ED%8C%8C%EC%9D%B4%ED%94%84%EB%9D%BC%EC%9D%B8-3-%EC%B5%9C%EA%B7%BC-%EB%B3%B8-%EC%83%81%ED%92%88-%EC%A1%B0%ED%9A%8C/)
- [로그 파이프라인 4 - 최근 본 상품 조회 결론](https://one-year-gap.github.io/docs/2026/03/13/%EB%A1%9C%EA%B7%B8-%ED%8C%8C%EC%9D%B4%ED%94%84%EB%9D%BC%EC%9D%B8-4-%EC%B5%9C%EA%B7%BC-%EB%B3%B8-%EC%83%81%ED%92%88-%EC%A1%B0%ED%9A%8C-%EA%B2%B0%EB%A1%A0/)



---

## 캐릭터 배치 기능

고객의 실제 사용량 데이터를 분석하여 **6가지 페르소나 중 하나를 부여하고 최적의 상품을 큐레이션**합니다.
다음과 같은 지수 산출 로직으로 캐릭터를 분류하였습니다. 
> 상세한 캐릭터 배치 지수는 📖  
> **[캐릭터 페르소나 지수 산정
](https://one-year-gap.github.io/docs/2026/03/18/%EC%BA%90%EB%A6%AD%ED%84%B0-%ED%8E%98%EB%A5%B4%EC%86%8C%EB%82%98-%EC%A7%80%EC%88%98-%EC%82%B0%EC%A0%95/
)** 문서에 정리되어 있습니다.

- **Data Driven:** 요금제, 데이터 사용량, 웨어러블 사용 여부 등 다각도 분석
- **Batch Process:** 일 단위 배치를 통해 최신 고객 상태 반영 및 캐릭터 갱신

---

## 개인별 추천 기능

수집된 대량의 데이터를 AI가 분석하여 실행 가능한 전략(Action Items)을 제안합니다.

- [추천시스템 구축기 1: 추천 방식의 변화](https://one-year-gap.github.io/docs/2026/03/12/%EC%B6%94%EC%B2%9C-%EB%B0%A9%EC%8B%9D%EC%9D%98-%EB%B3%80%ED%99%94/)
- [추천 시스템 구축기 2: 상품 임베딩 및 개인별 추천 시스템 RAG](https://one-year-gap.github.io/docs/2026/03/12/%EC%83%81%ED%92%88-%EC%9E%84%EB%B2%A0%EB%94%A9-%EB%B0%8F-%EA%B0%9C%EC%9D%B8%EB%B3%84-%EC%B6%94%EC%B2%9C-%EC%8B%9C%EC%8A%A4%ED%85%9C-%EC%84%A4%EA%B3%84/)

- 상품 임베딩
- 개인별 추천 시스템 RAG 프롬프트
- **사용자 행동 로그 기반:** 사용자의 행동 로그를 수집하여 추천
- **RAG Pipeline:** 정규화된 지표 컨텍스트를 LLM에 전달하여 고품질 리포트 생성

---

## 이탈률 계산 기능

정량적 기준(Rule Config)을 바탕으로 고객군을 분류하고 맞춤형 혜택을 제공합니다.

- [이탈률 설계](https://one-year-gap.github.io/docs/2026/03/14/%EC%9D%B4%ED%83%88%EB%A5%A0-%EC%84%A4%EA%B3%84/)
- [이탈률 가중치 점수 산출](https://one-year-gap.github.io/docs/2026/03/15/%EC%9D%B4%ED%83%88%EB%A5%A0-%EA%B0%80%EC%A4%91%EC%B9%98-%EC%A0%90%EC%88%98-%EC%82%B0%EC%B6%9C/)
- [이탈률 feature 확정과 테이블 설계](https://one-year-gap.github.io/docs/2026/03/14/%EC%9D%B4%ED%83%88%EB%A5%A0-%ED%85%8C%EC%9D%B4%EB%B8%94-%EC%84%A4%EA%B3%84/)

- 이탈률 feature 설계
- 이탈률 가중치 점수 산출
- 이탈률 점수 로직 아키텍처
- **이탈 위험군 탐지:** 약정 만료 D-30, 부정 키워드 감지, 사용량 30% 급감 등 복합 조건
- **Executive Summary:** 관리자의 신속한 의사결정을 돕는 핵심 요약 및 리스크 요인 도출

---

## ⚖️ 기술 선택 근거 (Technical Decisions)

## Persistence 전략: JPA와 jOOQ의 CQRS적 접근

우리는 **명령(Command)과 조회(Query)의 책임을 분리**하여 시스템의 안정성과 성능을 극대화했습니다.

## 1) JPA (Core / Transaction)

- **역할:** 회원, 상품, 상담 기록 등 핵심 도메인의 OLTP성 CRUD 처리
- **선택 이유:** 엔티티 중심의 비즈니스 로직 표현 및 Dirty Checking을 통한 트랜잭션 무결성 보장

## 2) jOOQ (Analytics / Batch)

- **역할:** 대량 데이터 집계, 통계 산출, 추천 랭킹 조회 등 OLAP성 쿼리 처리
- **선택 이유:**
  - **성능 최적화:** 복잡한 집계 SQL의 튜닝 포인트 명확화 및 성능 예측 가능
  - **타입 안정성:** 실제 스키마 기반 코드 생성을 통해 런타임 에러 방지 및 유지보수성 향상

---

## 카프카 도입 이유  ✨
Holiverse에서는 Kafka를 **로그 수집 및 실시간 이벤트 처리의 중심 메시지 브로커**로 사용하였습니다.
결론을 말하자면, 메인 서비스 로직과 분리하여 안정적으로 적재하고, 동시에 실시간 최신 본 상품과 배치 분석용 원본 저장을 병렬로 처리하기 위함입니다. 

즉 실시간 처리용 파이프라인과 원본 적재용 파이프라인으로 동시에 분기할 수 있었습니다. 
또한 Kafka는 **LLM 추천 결과를 비동기적으로 전달하는 추천 서빙 파이프라인**에도 활용하여, Kafka는 

- 로그 수집과 **데이터 레이크 적재**를 위한 이벤트 허브
- 실시간 추천에 쓰이는 **최근 본 상품**을 위한 적제 허브
- FastAPI 기반 LLM 추천 엔진과 **Spring 서버를 느슨하게 연결하는 비동기 브로커**
역할을 동시에 수행했습니다.

<img width="1486" height="966" alt="image" src="https://github.com/user-attachments/assets/6a59e3c4-6468-4626-b73b-c8bf4298b9c4" />

> 더 상세한 카프카 도입의 이유는 📖  
> **[Kafka 도입 이유](https://one-year-gap.github.io/docs/2026/03/17/kafka-%EB%8F%84%EC%9E%85-%EC%9D%B4%EC%9C%A0/)** 문서에 정리해 두었습니다.




---

## 🚀 추후 확장 가능성

- **실시간성 강화:** Kafka Streams를 이용한 실시간 페르소나 가변 업데이트
- **인프라 고도화:** Multi-AZ 환경 구성을 통한 고가용성 인프라 구축 및 부하 분산 최적화
- **분석 모델 심화:** 사용자 행동 패턴에 대한 딥러닝 기반 예측 모델 도입


---

## 📎 참고 문서

- [GitHub Wiki](https://one-year-gap.github.io/docs/)
- [화면 플로우 설계](https://one-year-gap.github.io/docs/2026/03/12/%ED%99%94%EB%A9%B4-%ED%94%8C%EB%A1%9C%EC%9A%B0-%EC%84%A4%EA%B3%84/)
- [백엔드 시스템 아키텍처](https://one-year-gap.github.io/docs/2026/02/10/%EB%B0%B1%EC%97%94%EB%93%9C-system-architecture/)
- [도메인 아키텍처](https://one-year-gap.github.io/docs/2026/02/12/%EB%B0%B1%EC%97%94%EB%93%9C-domain-architecture/)
- [인프라 아키텍처](https://one-year-gap.github.io/docs/2026/02/24/1%EC%B0%A8-mvp-infrastructure-architecture-v1/)
- [ERD 설계 및 Flyway 기반 DB 형상 관리](https://one-year-gap.github.io/docs/2026/03/13/erd-%EC%84%A4%EA%B3%84-%EB%B0%8F-flyway-%EA%B8%B0%EB%B0%98-db-%ED%98%95%EC%83%81-%EA%B4%80%EB%A6%AC/)
- [Notion](https://oxidized-cornflower-232.notion.site/2fd8a2b69065809fb671d47a8189b846)
- [Jira](https://tkv00123.atlassian.net/jira/software/projects/HSC/boards/2/timeline?atlOrigin=eyJpIjoiMGE4ZGY1NDVkYzZlNDY1YzgzMTQ2NDA0NmQ2MGM3ZDEiLCJwIjoiaiJ9)
- [Postman API](https://documenter.getpostman.com/view/50252872/2sBXcGFLPD)
