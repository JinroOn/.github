<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0B1F4B,100:5BA8D4&height=230&section=header&text=JinroOn&fontSize=78&fontColor=ffffff&fontAlignY=38&desc=%ED%9D%A5%EB%AF%B8%C2%B7%ED%99%9C%EB%8F%99%C2%B7%ED%95%99%EC%8A%B5%20%EC%9D%91%EB%8B%B5%EC%9C%BC%EB%A1%9C%20%EC%A0%84%EA%B3%B5%20%ED%83%90%EC%83%89%EC%9D%98%20%EA%B7%BC%EA%B1%B0%EB%A5%BC%20%EB%A7%8C%EB%93%9C%EB%8A%94%20%ED%94%8C%EB%9E%AB%ED%8F%BC&descSize=20&descAlignY=60&descColor=C8E8F8&animation=fadeIn"/>

**진로온** · 영남대학교 종합설계 2026

[![Service](https://img.shields.io/badge/서비스-jinro--on.vercel.app-5BA8D4?style=flat-square&labelColor=0B1F4B)](https://jinro-on.vercel.app)
[![Frontend](https://img.shields.io/badge/Frontend-JOFE-5BA8D4?style=flat-square&logo=react&logoColor=white&labelColor=0B1F4B)](https://github.com/JinroOn/JOFE)
[![Backend](https://img.shields.io/badge/Backend-JOBE-5BA8D4?style=flat-square&logo=springboot&logoColor=white&labelColor=0B1F4B)](https://github.com/JinroOn/JOBE)

</div>

<br/>

## 🧭 진로온은

전공을 고르기 전에 **무엇부터 알아봐야 할지** 정리해 주는 전공 탐색 웹 플랫폼입니다.

진로온은 능력이나 적성을 판정하지 않습니다. 관심 있는 분야, 해보고 싶은 활동, 배우고 싶은 내용을 묻고,
그 응답을 근거로 **먼저 탐색해볼 수 있는 전공군과 전공**을 보여 줍니다. 결과마다 어떤 응답이 근거가 됐는지,
근거가 부족한 부분은 어디인지 함께 표시하고, 전공 비교·탐색 활동·AI 상담·12주 탐색 계획으로 이어집니다.

<br/>

## 🔄 진단 흐름

```mermaid
flowchart LR
    A["1단계<br/>공통 탐색"] --> B["2단계<br/>맞춤 질문"] --> C["3단계<br/>확인할 점"] --> D["결과<br/>전공군 · 전공 · 근거"] --> E["비교 · 활동<br/>AI 상담 · 12주 계획"]
```

| 단계 | 하는 일 | 최대 문항 |
|---|---|---|
| 1단계 공통 탐색 | 관심 분야와 해본 활동을 확인하고 후보 전공군을 정합니다 | 42 |
| 2단계 맞춤 질문 | 정해진 후보군 안에서 활동·학습 방식·전공 비교 질문을 필요한 만큼만 묻습니다 | 24 |
| 3단계 확인할 점 | 탐색 전에 알아두면 좋은 부담 요소를 확인합니다 (점수에는 쓰지 않음) | 12 |
| 결과 | 최대 3개 전공군 · 7개 전공, 근거와 부족한 근거를 보여 줍니다 | — |

문항 풀은 187개지만 응답에 따라 필요한 질문만 나오므로, 결과 전까지 실제로 답하는 문항은 최대 78개입니다.

<br/>

## 🧮 추천 방식

점수에 쓰는 응답은 **관심 · 활동 · 학습** 세 가지뿐입니다.

| 축 | 묻는 것 | 구성 |
|---|---|---|
| 관심 | 어떤 분야·주제에 끌리는지 | 14개 축 (데이터, 공학, 생명, 교육, 미디어 …) |
| 활동 | 그 분야에서 어떤 방식의 일을 하고 싶은지 | 11개 축 (시스템, 설계, 탐구, 창작, 운영 …) |
| 학습 | 대학에서 무엇을 배우고 싶은지 | 12개 세트 |

1. 응답마다 0 · 25 · 50 · 75 · 100점을 주고, "모름"과 "경험 없음"은 평균에서 뺍니다.
2. **관심 점수로 후보 전공군을 먼저 정합니다.** 75점 이상인 관심 응답이 하나 이상 있어야 하고, 상위 2개 전공군에 3위가 2위와 5점 이내면 3위까지 보여 줍니다.
3. 후보 전공군 안에서 전공별 점수를 계산해 탐색 순서를 정합니다.

<div align="center">

**전공 점수 = 관심 × 0.62 + 활동 × 0.28 + 학습 × 0.10**

</div>

학습 응답이 없으면 관심 72% · 활동 28%로 계산하고, 근거가 빠진 요소는 남은 비중을 100%로 다시 맞춥니다.
전공 비교·부담 요소·진로 상태 응답은 결과 설명에만 쓰고 점수는 바꾸지 않습니다.

> **예시 — 소프트웨어학과**
> 관심 80점(데이터 87.5 × 0.7 + 공학 62.5 × 0.3) · 활동 72.5점(시스템 · 설계 · 창작) · 학습 75점
> → 80 × 0.62 + 72.5 × 0.28 + 75 × 0.10 = **77.4점**

같은 응답과 같은 규칙 버전이면 항상 같은 질문 순서와 같은 결과가 나옵니다. 현재 시각이나 랜덤값은 쓰지 않고, 동점은 전공 코드 순으로 정합니다.

<br/>

## 🤖 AI의 역할

| AI가 하는 일 | AI가 하지 않는 일 |
|---|---|
| 확정된 결과와 승인된 전공 자료로 추천 근거를 설명합니다 | 점수 · 순위 · 후보를 계산하지 않습니다 |
| 결과를 바탕으로 상담에 답하고 12주 탐색 계획을 만듭니다 | 합격 · 취업 가능성이나 능력 · 성격을 단정하지 않습니다 |
| 인용한 문장이 근거 자료 원문과 일치하는지 검증한 뒤에만 표시합니다 | 근거가 없는 연결을 억지로 만들지 않습니다 |

후보 선정은 서버 규칙이 하고, AI는 설명을 돕는 별도 서비스로 분리했습니다. AI 서비스가 꺼져 있어도 진단과 결과는 동작합니다.

<br/>

## ✨ 주요 기능

| 기능 | 설명 |
|---|---|
| 🧭 **전공 탐색 진단** | 응답에 따라 다음 질문을 서버가 정하는 3단계 진단. 중간에 나가도 이어서 진행 |
| 📊 **결과와 근거** | 전공군 · 전공 · 근거가 된 응답 · 부족한 근거 · 확인해볼 점. 전체 후보도 열람 가능 |
| ⚖️ **전공 비교** | 후보 전공 2개를 나란히 비교 |
| 🧪 **탐색 활동** | 전공별로 검토한 탐색 활동 카드와 활동 기록 |
| 💬 **AI 상담 · 전공 설명** | 결과와 승인 자료를 근거로 한 전공별 설명과 상담 |
| 🗓️ **12주 탐색 계획** | 고른 전공의 활동을 주차별 계획으로 정리 |
| 🔗 **이력 · 공유** | 진단 이력 조회, 결과 공유 링크 |
| 🛠️ **관리자** | 문항 · 전공 · 활동 카탈로그 검토 기록과 활성화 관리 |

<br/>

## 🏗️ 시스템 구성

```mermaid
flowchart TB
    FE["Frontend<br/>React · TypeScript"] -- "REST" --> BE["Backend<br/>Spring Boot"]
    BE --> DB[("MySQL<br/>카탈로그 · 세션 · 결과")]
    BE -- "근거 설명" --> AI["AI Service<br/>FastAPI · LangChain"]
    AI --> VDB[("PostgreSQL<br/>pgvector RAG")]
    AI --> LLM["LLM"]
```

<div align="center">

![React](https://img.shields.io/badge/React_19-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-443E38?style=flat-square)
<br/>
![Java](https://img.shields.io/badge/Java_17-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_4-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL_8-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white)
<br/>
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_·_pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
<br/>
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![AWS EC2](https://img.shields.io/badge/AWS_EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white)

</div>

<br/>

## 🗂️ 데이터

| 항목 | 수량 |
|---|---|
| 전공 | 94개 · 전공군 11개 |
| 문항 풀 | 187개 (선택지 1,360개) |
| 전공 비교 세트 | 32개 |
| 전공별 주의 태그 | 846행 |

문항 · 선택지 · 전공 매핑 · 추천 규칙은 버전별 카탈로그로 관리합니다. 적재할 때 SHA-256 해시 · 수량 · 버전 · 참조 관계를 검증하고, 하나라도 다르면 적재를 거부합니다. 진단을 시작하면 그 회차가 쓰는 문항과 규칙 버전을 고정하므로, 나중에 카탈로그가 바뀌어도 지난 결과는 달라지지 않습니다.

<br/>

## 📦 리포지토리

| 리포지토리 | 내용 |
|---|---|
| [**JOFE**](https://github.com/JinroOn/JOFE) | 프론트엔드 — 진단 · 결과 · 비교 · 활동 · AI 상담 · 계획 · 관리자 화면 |
| [**JOBE**](https://github.com/JinroOn/JOBE) | 백엔드 — Spring Boot API, 탐색 진단 엔진, 데이터 카탈로그, AI 서비스(`ai-service/`) |
| [JOAI](https://github.com/JinroOn/JOAI) | 초기에 만든 AI 리포지토리. 현재 AI 서비스 코드는 JOBE의 `ai-service/`에 있습니다 |

<br/>

## 👥 팀원

<div align="center">

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/rhwnsdud70">
        <img src="https://github.com/rhwnsdud70.png" width="90px" alt=""/><br/>
        <sub><b>고준영</b></sub>
      </a><br/>
      <sub>Backend · AI</sub>
    </td>
    <td align="center">
      <a href="https://github.com/vinn81">
        <img src="https://github.com/vinn81.png" width="90px" alt=""/><br/>
        <sub><b>김가빈</b></sub>
      </a><br/>
      <sub>Backend · AI</sub>
    </td>
    <td align="center">
      <a href="https://github.com/ryu2293">
        <img src="https://github.com/ryu2293.png" width="90px" alt=""/><br/>
        <sub><b>류승래</b></sub>
      </a><br/>
      <sub>Backend</sub>
    </td>
    <td align="center">
      <a href="https://github.com/FAITRUEE">
        <img src="https://github.com/FAITRUEE.png" width="90px" alt=""/><br/>
        <sub><b>이성진</b></sub>
      </a><br/>
      <sub>Frontend</sub>
    </td>
    <td align="center">
      <a href="https://github.com/dusdnd301">
        <img src="https://github.com/dusdnd301.png" width="90px" alt=""/><br/>
        <sub><b>김연웅</b></sub>
      </a><br/>
      <sub>Frontend</sub>
    </td>
    <td align="center">
      <a href="https://github.com/ryudayeong">
        <img src="https://github.com/ryudayeong.png" width="90px" alt=""/><br/>
        <sub><b>류다영</b></sub>
      </a><br/>
      <sub>Frontend</sub>
    </td>
  </tr>
</table>

</div>

<br/>

## 📌 프로젝트 상태

2026년 11월에 종합설계 프로젝트로 마무리했습니다.

- 문항 · 임계값 · 전공 매핑은 구현을 위해 정한 후보 값입니다. 실제 사용자 파일럿과 전문가 검수로 검증하는 단계는 진행하지 않았습니다.
- 탐색 진단은 데모용 개발 모드로 운영합니다. 정식 공개를 위한 승인 절차는 구현하지 않았고, 결과 공유 링크도 외부 공개 없이 검증용으로만 열려 있습니다.
- 남은 과제: AI 전공 설명의 2차 품질 평가, 운영 환경의 실행 · 공유 범위 결정
  ([JOBE #152](https://github.com/JinroOn/JOBE/issues/152), [#166](https://github.com/JinroOn/JOBE/issues/166))

<br/>

<div align="center">
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:5BA8D4,100:0B1F4B&height=130&section=footer&animation=fadeIn"/>
</div>
