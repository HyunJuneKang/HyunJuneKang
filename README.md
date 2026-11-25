<div align="center">

# 안녕하세요, 강현준입니다 👋

**금융 서비스와 배포 환경을 함께 만드는 개발자**

Spring Boot로 보험 수수료 지급·환수 로직을 구현하고, 팀원이 변경한 코드를 검증하고 배포할 환경을 구축했습니다.<br/>
AWS VPC와 EC2를 구성하고 GitHub Actions와 Jenkins로 개발·검증 환경에서 신한DS 교육용 서버까지 배포 과정을 연결했습니다.

[![GitHub](https://img.shields.io/badge/GitHub-HyunJuneKang-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/HyunJuneKang)
[![FGC](https://img.shields.io/badge/Featured-FGC-087F8C?style=flat-square&logo=springboot&logoColor=white)](https://github.com/feegachu/fgc)
[![BlueMarble](https://img.shields.io/badge/Project-BlueMarble-2563EB?style=flat-square)](https://github.com/HyunJuneKang/BlueMarble)

</div>

## 🚀 Featured Projects

### [FGC · 보험 수수료 업무 플랫폼](https://github.com/feegachu/fgc)

**5인 팀 · 기술 리드 · 백엔드 및 배포 환경 구축 · 2026.07–11**

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![JPA](https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white)
![QueryDSL](https://img.shields.io/badge/QueryDSL-0769AD?style=flat-square)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)

정책·지급·원장·환수를 연결하고, 산정 근거와 변경 이력을 추적하는 보험 수수료 플랫폼입니다.

- **검증한 이미지 배포** — AWS 개발 서버에 자동 배포한 이미지를 검증 서버에서 k6로 부하 테스트하고, 승인 후 같은 이미지 다이제스트로 신한DS 교육용 서버에 배포하도록 구성했습니다. [AWS 배포 파이프라인](https://github.com/feegachu/fgc/blob/develop/Jenkinsfile.fgc) · [검증 빌드의 신한DS 서버 배포](https://github.com/feegachu/fgc/blob/develop/Jenkinsfile.shinhan)
- **CI 대기 시간 개선** — 여러 작업에서 중복 실행되던 npm 의존성 취약점 검사를 한 번으로 분리했습니다. 첫 작업 시작부터 마지막 검증 완료까지 9분 34초에서 4분 4초로 줄었습니다(변경 전후 각 1회 측정). [GitHub Actions 설정](https://github.com/feegachu/fgc/blob/develop/.github/workflows/ci.yml)
- **영속성 전환** — MyBatis 잔여 구성을 제거하고 JPA·QueryDSL로 통합하며 조회 결과와 쓰기 시점을 검증했습니다. [PR #500](https://github.com/feegachu/fgc/pull/500)
- **업무 정책 구현** — 4년·7년 분급 정책의 설정·검증·조회를 구현했습니다. [PR #758](https://github.com/feegachu/fgc/pull/758)
- **계약 화면 개발** — 보험계약 목록·상세·등록·수정 화면을 React로 전환했습니다. [PR #519](https://github.com/feegachu/fgc/pull/519)
- **검증 자동화** — React 시연 E2E·커버리지 CI와 변경 범위별 필수 검사를 정리했습니다. [PR #544](https://github.com/feegachu/fgc/pull/544) · [PR #601](https://github.com/feegachu/fgc/pull/601)
- **환수 업무 연결** — 환수 통지서 PDF 생성·다운로드와 발행 이력을 구현했습니다. [PR #802](https://github.com/feegachu/fgc/pull/802)

### 공고대로 · 채용공고 판정 근거 조회

**2인 팀 · 대한민국 청년 CAREER FAIR AI 해커톤 · 2026.11**

React와 TypeScript로 AI가 판정에 사용한 문장을 원문과 대조하는 화면을 개발했습니다. 실제 공고 3건을 연결하고, GitHub Actions에서 PR마다 테스트·린트·타입 검사·빌드를 실행하도록 구성했습니다. [공고대로 서비스 열기](https://gonggo-daero.vercel.app/)

## 🧩 More Projects

| 프로젝트 | 역할 | 직접 구현한 내용 |
| :--- | :--- | :--- |
| **SAP 구매·회계 프로세스** | 1인 · 업무 분석·DB·ABAP·화면 | ECC 6.0의 Z테이블·ALV·Custom Control로 PO·GR·IV와 회계 전표 연결, 부분입고·취소 처리 |
| **[부루마블](https://github.com/HyunJuneKang/BlueMarble)** | 1인 · 게임·DB·Java 전체 설계 및 구현 | MVC와 Service·DAO 분리, DiceStrategy, Oracle JDBC 기반 회원·인벤토리·게임 기록 저장 |
| **점심메이트** | 1인 · 웹·Servlet API·DB 전체 구현 | 매칭 저장·이력·상세·조합 통계, 300개 무작위 후보 중 과거 동석 횟수 합이 가장 적은 조합 선택 |

## 🎓 Experience

| 경험 | 내용 |
| :--- | :--- |
| **숭실대학교** | 전자정보공학부 IT융합전공 · 학사 · 2020.02 - 2026.02 · GPA 4.03 / 4.5 |
| **SAP Co-op Track** | 숭실대학교 4학년 이수 · SAP ECC 6.0 · ABAP · MM/FI |
| **신한DS 금융SW아카데미** | Java·Spring·React·SQL·AWS 팀·개인 프로젝트, Python·LLM·RAG·AI Agent 실습 |

## 🛠 Tech Stack

<table>
<tr><th align="left">Backend</th><td><img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=flat-square"/> <img alt="Spring Boot" src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/> <img alt="JPA" src="https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white"/> <img alt="QueryDSL" src="https://img.shields.io/badge/QueryDSL-0769AD?style=flat-square"/> <img alt="Servlet" src="https://img.shields.io/badge/Servlet-F8DC75?style=flat-square&logo=apachetomcat&logoColor=black"/></td></tr>
<tr><th align="left">Database</th><td><img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/> <img alt="Oracle" src="https://img.shields.io/badge/Oracle-F80000?style=flat-square"/> <img alt="JDBC" src="https://img.shields.io/badge/JDBC-4479A1?style=flat-square"/></td></tr>
<tr><th align="left">Frontend</th><td><img alt="React" src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB"/> <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/> <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black"/></td></tr>
<tr><th align="left">Infra & Collaboration</th><td><img alt="AWS EC2" src="https://img.shields.io/badge/AWS_EC2-FF9900?style=flat-square"/> <img alt="Git" src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/> <img alt="GitHub Actions" src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/> <img alt="Jenkins" src="https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white"/></td></tr>
<tr><th align="left">ERP</th><td><img alt="SAP ABAP" src="https://img.shields.io/badge/SAP_ABAP-0FAAFF?style=flat-square&logo=sap&logoColor=white"/> <img alt="MM FI" src="https://img.shields.io/badge/MM_·_FI-00629B?style=flat-square"/></td></tr>
<tr><th align="left">AI Learning</th><td><img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/> <img alt="LangGraph" src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white"/> <img alt="FAISS RAG" src="https://img.shields.io/badge/FAISS_·_RAG-5B5BD6?style=flat-square"/></td></tr>
</table>

## 📜 Certification

[SAP Certified – Back-End Developer – ABAP Cloud](https://www.credly.com/badges/0af69d99-bec3-4cf3-b4b2-6dd000382e1b) · 2025.12.18 취득

## 📊 GitHub Activity

<div align="center">

![GitHub Stats](https://github-stats-extended.vercel.app/api?username=HyunJuneKang&show_icons=true&hide_title=true&hide_rank=true&hide_border=true&bg_color=171c22&text_color=e6edf3&icon_color=ad8cff&include_all_commits=true)

<a href="https://www.gitanimals.org/en-US?utm_medium=image&utm_source=HyunJuneKang&utm_content=farm">
  <img src="https://render.gitanimals.org/farms/HyunJuneKang" width="600" height="300" alt="HyunJuneKang's GitAnimals farm" />
</a>

</div>
