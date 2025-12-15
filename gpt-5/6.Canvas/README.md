
```text
다음의 내용으로 Canvas에 저장해줘. 

## 0. Meta
- Topic: 반도체 산업 동향
- Status: COLLECTING
- Decision Owner: 김문주
- Created At: 2025-XX-XX

---

## 1. Raw Data (Agent Only)

---

## 2. Verified Facts (Agent → Human Review)

---

## 3. Human Interpretation (Human Only)

---

## 4. Decision & Approval

---

## 5. Action Items
```


```text
너는 Search Agent야.

반도체 산업 관련 뉴스 내용을 GPT Canvas 저장소에
Canvas의 반도체 산업 동향 [1. Raw Data] 섹션에
검색한 내용을 추가(write)해줘.

규칙:
- 기존 내용은 수정하지 말 것
- 요약은 사실 중심
- 해석이나 판단 금지

📌 이 프롬프트의 핵심:
    역할 지정: Search Agent
    대상 지정: [1. Raw Data]
    행동 지정: 추가해줘 (write)
```

---

### 사실 검증 프롬프트 (Research Agent)

```text
너는 Research Agent야.

반도체 산업 동향 Canvas의 [1. Raw Data]를 읽고
출처가 2개 이상 겹치는 사실만 선별해서

반도체 산업 동향 Canvas의 [2. Verified Facts] 섹션을
표 형태로 채워줘.

규칙:
- 단일 출처 정보 제외
- 추정·불확실 표현 제거
- 해석이나 의견 금지
- 기존 내용 수정 금지

📌 이 프롬프트의 핵심:
    역할 지정: Reasearch Agent
    대상 지정: [2. Verified Facts]
    행동 지정: 추가해줘 (write)
```

```text
반도체 산업 동향 Canvas의 [2. Verified Facts]를 읽고

시장 / 전략 / 리스크 관점에서
사람의 해석을 추가해서

반도체 산업 동향 Canvas의 [3. Human Interpretation] 섹션을 작성해줘.

규칙:
- 판단과 해석은 허용
- Agent 관점 금지
- 사실 왜곡 금지
```

### 의사결정 프롬프트 (Human)

```text
반도체 산업 동향 Canvas [4. Decision & Approval] 섹션에 
오늘 날짜로 APPROVED로 작성해줘.

# 반도체 산업 동향 Canvas의 [3. Human Interpretation]을 바탕으로
#
#다음 중 하나를 선택해
#반도체 산업 동향 Canvas [4. Decision & Approval] 섹션을 작성해줘.

#- APPROVED
#- REJECTED
#- NEED_MORE_INFO

# 선택 이유를 반드시 명시해.
```

