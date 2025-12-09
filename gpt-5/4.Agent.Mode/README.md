# GPT-5 Agent mode
# https://github.com/moonjukhim/gpt

```text
총 4개의 에이전트(Data-Agent, Analysis-Agent, Report-Agent, QA-Agent)를 생성해
월간 KPI 보고서를 자동으로 생성하고 Canvas 업데이트까지 수행해야 한다.

각 에이전트의 역할은 다음과 같다:

1) Data-Agent  
- 업로드된 KPI.xlsx 또는 CSV 파일을 로드  
- 매출, 성장률, 신규 고객, 재방문 고객 등 핵심 KPI 정제  
- 분석 가능한 형태로 구조화된 데이터 반환  

2) Analysis-Agent  
- Data-Agent가 정제한 데이터를 기반으로 KPI 분석  
- 전월 대비 증감, YoY 성장률, 이상치 감지  
- 시각화용 차트 데이터 생성  
- 핵심 인사이트 3~5개 반환  

3) Report-Agent  
- Canvas에 "월간_KPI_보고서" 문서를 신규 생성 또는 업데이트  
- Executive Summary → KPI Table → Charts → Insight 순으로 자동 구성  
- 문서 부족 시 필요한 데이터를 Data-Agent에 재요청 가능  

4) QA-Agent  
- 생성된 보고서 품질을 검증  
- 계산 오류·해석 오류·문장 품질 감지  
- 필요한 부분 자동 수정  

5) 최종 단계
- 최종 PDF를 Canvas에 저장 그리고 다운로드 가능한 링크 출력("월간_KPI_보고서.pdf")

──────────────────────────────
<<실행 규칙>>
- 반드시 “Plan → Act → Check” 루프를 각 에이전트에서 수행할 것  
- 필요한 경우 다른 에이전트에게 정보를 요청하면서 협업해야 함  
- 사용자 개입 없이 자동으로 최종 문서까지 생성할 것  
- 모든 단계에서 reasoning 과정을 간단히 표시
- 결과는 한글로 출력
```