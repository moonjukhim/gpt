# Web search

```text
당신은 Multi-Agent Orchestrator입니다.  
아래 5단계 자동화 흐름을 순서대로 수행하세요.

[분석 대상 산업]
13대 주력산업 (자동차, 조선, 일반기계, 철강, 정유, 석유화학, 섬유, 정보통신기기, 가전, 반도체, 디스플레이, 이차전지, 바이오헬스)

[기간]
최근 72시간(최신성 가중치 포함)

────────────────────────
📌 1단계 — 최신성 기반 Web Search 수행
────────────────────────
· Web Search를 사용 최근 72시간 기사, 산업 보고서, 정책 발표, 기업 동향을 검색  
· 전략 / 기술 / 시장 관점으로 분류하여 정리  
· 각 항목별 출처(URL, 일시 포함)를 반드시 명시  
· 노이즈 기사 제거  
· 신뢰도 높은 출처 우선 정렬

출력:
- Strategy Findings
- Technology Findings
- Market Findings

────────────────────────
📌 2단계 — Deep Research로 출처 기반 비교·검증
────────────────────────
수집한 데이터를 PCVS(Plan → Collect → Verify → Synthesize) 구조로 분석하라.

필수 작업:
· 서로 상충되는 정보 비교  
· 가격 전망, 공급망 이슈, 정책 변화 검증  
· 중요 출처(TrendForce, Reuters, Bloomberg, KITA 등) 강조  
· 출처별 주장 차이점 요약  
· 결론 도출

출력:
- Verified Insights (근거 기반)
- Critical Signals (핵심 시그널)
- Supporting Sources (출처 목록)

────────────────────────
📌 3단계 — Shift Detection & Impact Analysis
────────────────────────
GPT-5 Reasoning Engine을 사용해 다음을 수행하라:

1) 기존 산업 평균/트렌드 대비 "변화 감지(Shift Detection)"
2) 변화의 의미 분석  
3) 영향도를 Low / Medium / High로 분류  
4) 영향받는 부서 매핑
   - 전략팀
   - 기술팀
   - 마케팅팀
   - 영업팀

출력:
- Detected Shifts
- Impact Levels
- Department Impact Map

────────────────────────
📌 4단계 — Canvas 문서 자동 업데이트용 변경 내용 생성
────────────────────────
아래 문서에 적용할 업데이트 내용을 생성하라:

문서명: "경제ㆍ산업_전망_2025년_하반기_경제산업_결과.pdf"

룰:
· 변경된 내용만 하이라이트 표시  
· 신규 데이터 → (NEW)  
· 수정된 데이터 → (UPDATED)  
· 삭제 필요 데이터 → (REMOVED)  
· 업데이트 블록을 Markdown으로 구조화

출력:
- Canvas_Update_Block

────────────────────────
📌 5단계 — 부서별 요약 알림 메시지 생성
────────────────────────
각 부서가 바로 읽고 대응할 수 있는 Slack/Gmail 요약 메시지를 생성하라.

구성:
· 1줄 헤드라인  
· 3줄 요약  
· 행동 권고(Action Items)  
· 중요도: Low/Medium/High 표시

부서:
- 전략팀
- 기술팀
- 마케팅팀
- 영업팀

출력:
- Strategy_Alert
- Tech_Alert
- Marketing_Alert
- Sales_Alert

────────────────────────
📌 최종 출력 포맷
────────────────────────
1) Step1 Findings (Strategy / Technology / Market)
2) Step2 Deep Research 결과 (근거 기반)
3) Step3 변화 감지 & 영향 분석
4) Step4 Canvas 업데이트 블록
5) Step5 부서별 자동 알림 메시지


위의 5단계를 순차적으로 수행하고 전체 결과를 
"2025년_하반기_경제산업_검토.docx"로 종합 출력하라.
기존 Canvas 문서 "KIET_경제ㆍ산업_전망_2025년_하반기_경제산업_전망.pdf"과 비교해 
차이가 나는 부분을 경제ㆍ산업_전망_2025년_하반기_경제산업_결과2.pdf출력해줘.
```

---

##### Test 2

```text
Web Search를 사용해서 최근 72시간 동안 반도체 산업에 영향을 주는
주요 뉴스·정책 변화를 조사해줘.

1) 최신성 평가
2) 핵심 요약
3) 산업 영향 분석
4) 기존 Canvas 문서 “2026_반도체_리서치초안.docx”과 비교해 
   변경이 필요한 부분을 표시하고 자동 업데이트해줘.

마지막에 업데이트된 내용을 별도로 표시해줘.
```