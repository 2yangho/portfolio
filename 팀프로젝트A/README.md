## RFM 분석을 이용한 이커머스 고객 Segmentation 프로젝트

---

### **프로젝트 개요**

> 배경

```
이커머스 기업 A는 현재 경기 침체로 인한 신사업 투자 위험 증가, 업계 멤버십 경쟁의 심화 등 다양한 문제에 직면하고 있습니다.
이에 대응하기 위해 고객을 유치하기 위한 마케팅 전략을 수립하려고 합니다.
따라서 데이터 분석을 통해 타겟 고객층을 식별하고, 개인화된 마케팅 캠페인을 진행할 계획입니다. 
```

> 분석목적

```
- 고객 유형에 맞는 마케팅 전략 수립으로 신규 고객 유입 증가
- 특정 등급의 고객에게 자사만의 차별화된 혜택 제공을 통해 주요고객 이탈률 감소
```

---

### **분석과정**

> 데이터 EDA

![](https://velog.velcdn.com/images/finemann/post/62435bf0-397b-4067-acb8-051b896fc49a/image.png)

- 워싱턴D.C 지역은 전반적으로 낮은 고객수, 거래량, 구매금액을 보였지만, 개인당 구매금액이 높은 지역으로 나타났다. 

- 워싱턴 지역 고객들의 최근 구매 시기, 구매 빈도, 구매패턴을 파악하기 위해 RFM 분석을 도입하여 고객 특성에 맞는 마케팅 전략을 수립할 계획이다.

> RFM Score 변수 생성

- 고객 별 Recency, Frequency, Monetary 변수를 할당한 뒤, 세 변수를 더해 RFM Score 변수 생성

![](https://velog.velcdn.com/images/finemann/post/012f95ec-ff59-45c3-bdf1-d3375a5c34e6/image.png)

- score 변수의 분포에 따라 고객 등급을 A~F까지 5단계 등급으로 분할

---

### **분석결과**

![](https://velog.velcdn.com/images/finemann/post/6b7d06cd-a333-4eb4-aac5-29d9fd58b267/image.png)

- 다른 지역보다 Chicago, Washington DC 지역에서 B등급 이상 고객 비율이 높았다.

![](https://velog.velcdn.com/images/finemann/post/dfebd0b9-a7c4-49ba-90d3-24ba7c146e83/image.png)

- Washingtond DC 지역이 다른 지역보다 높은 등급에서 Nest, Nest-USA 구매 비중이 높다.

---

### 해결책 및 기대효과

```
- Washington DC 지역의 A~C등급의 고객들이 선호하는 제품에 대한 추가 할인쿠폰을 제공
  → 충성 고객의 이탈 방지, 구매력 상승 
- Washington DC 지역은 높은 등급 고객의 비율이 높은 지역 
  → 신규 고객을 더 늘린다면 다른 지역보다 수익률이 높을 것으로 예상
  → 오프라인 마케팅을 이 지역에 집중 제안
```

---

### Lesson & Learned

![](https://velog.velcdn.com/images/finemann/post/87c1eb4b-c234-42b8-abf1-dc9ae8bec142/image.png)
