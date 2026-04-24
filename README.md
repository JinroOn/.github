<div align="center">

<!-- 헤더 배너 -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,12,20,24&height=230&section=header&text=JinroOn&fontSize=78&fontColor=ffffff&fontAlignY=38&desc=AI%20기반%20전공%20추천%20플랫폼&descSize=21&descAlignY=60&descColor=C8E8F8&animation=fadeIn"/>

<br/>

<!-- 뱃지 -->
&nbsp;
![GitHub stars](https://img.shields.io/github/stars/JinroOn?style=flat-square&color=5BA8D4&labelColor=0B1F4B)
&nbsp;
![Made with Love](https://img.shields.io/badge/Made%20with-❤️-A8D8EA?style=flat-square&labelColor=0B1F4B)

</div>

<br/>

---

## 👥 팀원 소개

<br/>

<div align="center">

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/github_id_1">
        <img src="https://github.com/github_id_1.png" width="90px" style="border-radius:50%; border: 3px solid #5BA8D4;" alt=""/><br/>
        <sub><b>github_id_1</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/github_id_2">
        <img src="https://github.com/github_id_2.png" width="90px" style="border-radius:50%; border: 3px solid #5BA8D4;" alt=""/><br/>
        <sub><b>github_id_2</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/github_id_3">
        <img src="https://github.com/github_id_3.png" width="90px" style="border-radius:50%; border: 3px solid #5BA8D4;" alt=""/><br/>
        <sub><b>github_id_3</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/github_id_4">
        <img src="https://github.com/github_id_4.png" width="90px" style="border-radius:50%; border: 3px solid #5BA8D4;" alt=""/><br/>
        <sub><b>github_id_4</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/github_id_5">
        <img src="https://github.com/github_id_5.png" width="90px" style="border-radius:50%; border: 3px solid #5BA8D4;" alt=""/><br/>
        <sub><b>github_id_5</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/github_id_6">
        <img src="https://github.com/github_id_6.png" width="90px" style="border-radius:50%; border: 3px solid #5BA8D4;" alt=""/><br/>
        <sub><b>github_id_6</b></sub>
      </a>
    </td>
  </tr>
</table>

</div>

<br/>

---

## 🎯 프로젝트 소개

<div align="center">
<br/>

> **JinroOn**은 학생들이 자신의 학습 성향, 기초 역량, 관심사를 기반으로  
> **가장 적합한 전공을 AI가 분석·추천해주는 플랫폼**입니다.

<br/>

기존 진로 플랫폼이 단순 흥미·적성 매칭에 그친다면,  
JinroOn은 **7개 차원의 역량 벡터**와 **코사인 유사도 알고리즘**, **LLM 기반 AI 피드백**으로  
한 차원 높은 전공 탐색 경험을 제공합니다.

<br/>

</div>

---

## ✨ 주요 기능

<br/>

<div align="center">

| 기능 | 설명 |
|:---:|:---|
| 🧠 **AI 전공 적합도 분석** | 사용자 역량 벡터와 전공별 요구 역량 벡터의 코사인 유사도를 계산하여 상위 추천 전공 제시 |
| 📝 **학습 성향 진단** | 서술형 답변 AI 분석, 기초 역량 평가, 학습 방식을 종합한 성향 프로파일 생성 |
| 📊 **결과 시각화** | 레이더 차트 · 막대그래프 · 도넛 차트로 역량 및 전공 적합도를 직관적으로 시각화 |
| 🔁 **What-if 시뮬레이션** | 역량 변수를 직접 조정해 전공 적합도 변화를 실시간 예측 |
| 💬 **AI 상담 챗봇** | 진단 결과 기반 맞춤형 전공 상담 및 의사결정 지원 |
| 📚 **취약 역량 보완 플랜** | 4~12주 주차별 학습 계획 자동 생성 + 유튜브 영상 추천 |
| 📄 **결과 리포트 내보내기** | PDF 다운로드 · 이미지 저장 · 공유 링크 생성 |

</div>

<br/>

---

## 🔍 핵심 알고리즘

<br/>

**역량 벡터 기반 전공 추천**

사용자의 답변을 **7개 차원(논리 · 창의 · 언어 · 수리 · 사회 · 과학 · 예술)** 의 역량 벡터로 변환하고,  
전공별 요구 벡터와의 **코사인 유사도**를 계산해 최적 전공을 순위화합니다.

$$\text{similarity}(A, B) = \frac{A \cdot B}{\|A\| \cdot \|B\|}$$

- **서술형 분석**: LLM이 자유 응답에서 역량 성향을 자동 추출  
- **What-if 예측**: 역량값 조정 시 추천 순위가 실시간으로 재계산  
- **취약점 감지**: 상위 추천 전공과의 역량 갭을 분석해 보완 플랜 자동 생성

<br/>

---

## 🚀 로컬 실행

<br/>

```bash
# 1. 레포 클론
git clone https://github.com/JinroOn/JinroOn.git

# 2. 프론트엔드
cd frontend && npm install && npm run dev

# 3. 백엔드 (Java 17+, Gradle)
cd backend && ./gradlew bootRun

# 4. AI 서버
cd ai-server && pip install -r requirements.txt && python main.py
```

> `.env` 파일에 `CLAUDE_API_KEY` / `OPENAI_API_KEY` / `DB_URL` 설정 필요

<br/>

---

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,12,20,24&height=130&section=footer&animation=fadeIn"/>

</div>
