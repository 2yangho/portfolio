# Data Analysis portfolio
--- 

> ## 목차

1. 시계열 센서 데이터 이상탐지 [[클릭](https://github.com/2yangho/portfolio/tree/main?tab=readme-ov-file#1-%EC%8B%9C%EA%B3%84%EC%97%B4-%EC%84%BC%EC%84%9C-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EC%9D%B4%EC%83%81%ED%83%90%EC%A7%80)]
   
   `제조 도메인의 이상탐지 모델 구축 과제를 딥러닝을 이용해 수행하였습니다. `
2. 웹툰 컨텐츠 EDA [[클릭](https://github.com/2yangho/portfolio/tree/main?tab=readme-ov-file#2-%EB%B3%B4%ED%97%98-%EA%B4%80%EC%8B%AC%EA%B3%A0%EA%B0%9D-%EC%98%88%EC%B8%A1)]
   
   `컨텐츠 도메인에서 웹툰 데이터를 활용한 EDA를 통해 사용자 행동 패턴 및 선호 컨텐츠를 파악할 수 있었습니다. `
3. 통신사 VOC 분석 [[클릭](https://github.com/2yangho/portfolio/tree/main?tab=readme-ov-file#3-%EC%9D%B4%EC%BB%A4%EB%A8%B8%EC%8A%A4-%EC%BD%94%ED%98%B8%ED%8A%B8-%EB%B6%84%EC%84%9D)]
   
   `통신사 도메인에서 VOC 분석을 통해 고객 불만사항들을 그룹화한 뒤 우선적으로 해결해야할 불만사항을 제시하였습니다. `
4. (팀 프로젝트 A) RFM 분석을 이용한 고객 Segmentation [[클릭](https://github.com/2yangho/portfolio/blob/main/README.md#4-rfm-%EB%B6%84%EC%84%9D%EC%9D%84-%EC%9D%B4%EC%9A%A9%ED%95%9C-%EA%B3%A0%EA%B0%9D-segmentation-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8)]
   
   `이커머스 도메인에서 RFM 분석을 통해 고객별 등급을 만들고, 특정 등급 고객의 특징을 파악해 고객 유형별 마케팅 방향을 제시했습니다. `
5. (팀 프로젝트 B) 신용카드 고객 데이터를 활용한 고객 이탈 예측
    
   `금융(카드) 도메인에서 Classification 모델을 이용해 이탈 고객을 예측하고, 클러스터링을 이용해 이탈 위험 고객군을 분류하여 고객 특성에 맞는 이탈 방지 전략을 제안했습니다.`

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
## **2. 웹툰 컨텐츠 EDA**
---

> 문제정의

```
- 사용자 웹툰 선호도 및 행동 패턴에 대한 정보 부족
```

> 해결방안

```
- 정규 웹툰 데이터를 통해 인기 웹툰의 장르, 업데이트 요일별 분석
- 베스트도전 웹툰 데이터를 통해 공식연재 결정 웹툰의 특징 분석
- 웹툰 사용자의 선호 패턴 분석
```

> 기대효과

```
- 사용자 행동 패턴 및 웹툰 선호도 파악을 통해 콘텐츠 맞춤 제공, 효율적인 웹툰 마케팅 전략으로 사용자 유입 증가
- 베스트 도전 웹툰 데이터 분석을 통해 합리적인 비용으로 잠재 유망 작가 유치 
```

> Lesson&Learned

```
- 심화된 EDA를 통해 연령별/인기작가별/연도별 선호 작품 장르 파악
- 베스트 도전 웹툰/ 정규 웹툰 각 데이터셋으로부터 공통된 특징을 파악해 트렌드 이해
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

## **5. 신용카드 고객 데이터를 활용한 고객 이탈 예측**
---

> 문제정의

```
- 신용카드 이용 고객 이탈로 인한 이용자 수 하락 및 매출 감소
```

> 해결방안

```
- 고객별 이탈 예측 모델을 생성 후, 클러스터링을 이용해 이탈 위험도별 고객군 분류
- 이탈 위험 고객군들의 특징에 맞는 이탈방지 솔루션 제시 및 충성고객으로 전환 방법 제안
```

> 기대효과

```
- 특정 고객군의 이탈 방지를 통해 이용자 수 유지
- 충성 고객 수 증가로 인한 지속적인 매출 증가
```

> Lesson & Learned

```
- 다양한 머신러닝 분류 모델 중에서 데이터셋의 특징에 맞는 모델을 선정하는 방법을 배움
- 여러가지 차원축소 알고리즘의 장단점을 파악하고 그 중 적절한 모델을 사용하는 방법을 알게됨
- 차원축소 알고리즘의 원본 데이터 보존 정도의 중요성을 깨닫고, 보존 정도를 평가하는 다양한 지표들을 사용하는 방법을 배움
```
[프로젝트 상세](https://github.com/2yangho/portfolio/tree/main/%ED%8C%80%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8B)
