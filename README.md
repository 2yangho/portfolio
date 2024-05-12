# Data Analysis portfolio
--- 

> ## 목차

1. 시계열 센서 데이터 이상탐지 [[클릭](https://github.com/2yangho/portfolio/tree/main?tab=readme-ov-file#1-%EC%8B%9C%EA%B3%84%EC%97%B4-%EC%84%BC%EC%84%9C-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EC%9D%B4%EC%83%81%ED%83%90%EC%A7%80)]
   
   `제조 도메인의 이상탐지 모델 구축 과제를 딥러닝을 이용해 수행하였습니다. `
2. 보험 관심고객군 예측 [[클릭](https://github.com/2yangho/portfolio/tree/main?tab=readme-ov-file#2-%EB%B3%B4%ED%97%98-%EA%B4%80%EC%8B%AC%EA%B3%A0%EA%B0%9D-%EC%98%88%EC%B8%A1)]
   
   `보험 도메인에서 고객 데이터를 활용한 EDA 및 Classification 머신러닝 모델 구축을 통해 보험 관심도 높은 특정 고객군을 추출하였습니다. `
3. 통신사 VOC 분석 [[클릭](https://github.com/2yangho/portfolio/tree/main?tab=readme-ov-file#3-%EC%9D%B4%EC%BB%A4%EB%A8%B8%EC%8A%A4-%EC%BD%94%ED%98%B8%ED%8A%B8-%EB%B6%84%EC%84%9D)]
   
   `통신사 도메인에서 VOC 분석을 통해 고객 불만사항들을 그룹화한 뒤 우선적으로 해결해야할 불만사항을 제시하였습니다. `
4. (팀 프로젝트 A) RFM 분석을 이용한 고객 Segmentation [[클릭](https://github.com/2yangho/portfolio/blob/main/README.md#4-rfm-%EB%B6%84%EC%84%9D%EC%9D%84-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EA%B3%A0%EA%B0%9D-segmentation-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8)]
   
   `이커머스 도메인에서 RFM 분석을 통해 고객별 등급을 만들고, 특정 등급 고객의 특징을 파악해 고객 유형별 마케팅 방향을 제시했습니다. `
5. 팀 프로젝트 B
    
   `ㅇㅇ`

## **1. 시계열 센서 데이터 이상탐지**
---

> 문제정의

```
- 장비의 고장으로 인한 생산 지연, 이로 인해 품질문제 발생 및 생산량감소
```

> 해결방안

```
- 장비 실시간 모니터링 센서 데이터로 이상탐지 모델을 구축해 장비 이상징후 조기발견
- 이상징후의 원인을 파악해 장비 고장예방 및 유지관리 전략 수립
```

> 기대효과

```
- 지속적인 생산량 및 품질 유지 가능. 고장 예방으로 장비 수리비용 절감
```

> Lesson&Learned

```
- 센서 데이터데에서 자주 발생하는 결측값 대체방법들 중 하나로 회귀예측 모델을 도입
- 프로젝트 목표 해결 위한 목표변수 재설정(Shifting)
- 데이터 불균형 문제를 해결할 대안으로서의 딥러닝 모델(AutoEncoder) 적용
```
[프로젝트 상세](https://github.com/2yangho/portfolio/tree/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8A)
## **2. 보험 관심고객 예측**
---

> 문제정의

```
- 보험사 신규 가입자수 증가율 둔화로 인한 수익 감소
```

> 해결방안

```
- 고객 데이터로부터 classification 머신러닝 모델을 구축해 보험 상품에 관심있는 특정 고객군을 예측. 해당 고객을 대상으로 마케팅 진행 제안
- 보험사의 목표 고객 응답률 또는 확보 고객수를 제안하고 이 조건에 맞는 고객 그룹 특성 추출
```

> 기대효과

```
- 신규 가입자 수 증가로 수익 증대
- 선별적 고객 대상 마케팅으로 홍보비 효율 개선
```

> Lesson&Learned

```
- classification 모델(RandomForest, lightGBM 등) 사용 경험, 모델 성능 향상을 위한 Feature Engineering
- 대상 고객의 목표 가입률 및 고객수를 만족시키는 조건을 찾기 위한 고객 데이터 드릴다운 과정 
```
[프로젝트 상세](https://github.com/2yangho/portfolio/tree/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8B)
## **3. 통신사 VOC 분석**
---

> 문제정의

```
- 고객 만족도 하락으로 인한 고객 이탈 위험 증가
```

> 해결방안

```
- VOC 분석을 통한 주요 고객 불만사항 파악
```

> 기대효과

```
- 주요 고객 불만사항 개선을 통해 서비스 만족도 증가, 고객 이탈 위험 감소
```

> Lesson&Learned

```
- 자연어 처리를 통해 텍스트로들부터 주요 토픽 추출 방법을 알게 되므로써 핵심 문제 요인 파악  
- VOC 분석으로 지역별, 날짜별, 해결상태별 핵심 문제 분포를 파악해 우선적으로 해결 요구되는 사안 확인   
```
[프로젝트 상세](https://github.com/2yangho/portfolio/tree/main/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8C)


## **4. RFM 분석을 이용한 고객 Segmentation 프로젝트**
---

> 문제정의

```
- 경기 침체로 신사업 투자가 어려운 상황에서 업계 멤버십 경쟁 심화로 신규 고객 유치 비용 상승 
- 해외 거대 기업의 국내 시장 공략으로 인한 고객 이탈 증가
```

> 해결방안

```
- 고객 소비 데이터로부터 RFM 분석을 이용해 고객 등급화 후 특정 등급의 고객에게 차별화된 혜택 제공
- 고객 세분화 분석으로 고객 특성 파악해 유형에 맞는 마케팅 전략 수립
```

> 기대효과

```
- 고객 유형에 맞는 마케팅 전략 수립으로 신규 고객 유입 및 마케팅 효율 증가
- 특정 등급 고객에게 자사만의 차별화된 혜택 제공을 통해 주요고객 이탈률 감소
```

> Lesson & Learned

```
- 분석 스토리라인 기획을 통해 RFM 분석을 비롯한 세부 분석 방향 설정하는 방법을 배움
- 기존의 변수를 조합해 새로운 분석 지표를 생성하는 RFM 분석을 이용함으로써, 고객 데이터를 해당 지표를 이용해 분류하여 새로운 특성을 도출함
```
[프로젝트 상세](https://github.com/2yangho/portfolio/tree/main/%ED%8C%80%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8A)
