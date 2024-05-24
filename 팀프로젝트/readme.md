## 신용카드 고객 데이터를 활용한 고객 이탈 예측

---

### 프로젝트 개요

> **배경**

```
신용카드 서비스사인 B사는 소비자 신용카드 포트폴리오에서 수집된 고객 정보를 활용하려 합니다.
목표는 고객 이탈을 예측하는 것으로, 서비스 개선 및 고객 충성도 향상에 필요한 조치를 취하고자 합니다.
이를 통해 고객의 이탈을 예측하고 이를 활용하여 포트폴리오 관리 전략을 조정하거나, 
개별 고객에게 더 맞춤화된 서비스를 제공할 방안을 모색할 예정입니다.
```

> **분석목적**

```
- 특정 고객군의 이탈 방지를 통해 이용자 수 유지
- 충성 고객 수 증가로 인한 지속적인 매출 증가
```

---

### 분석 과정

> EDA 

![](https://velog.velcdn.com/images/finemann/post/2f8d5b67-4c04-4e62-a27e-fe139bbf17a5/image.png)

- 특정 변수에서 이탈고객/비이탈고객의 분포도가 다른 것을 확인 
→ 이탈 고객 예측 모델을 만들 때 해당 변수들이 중요 변수로서 작용될 것을 예측할 수 있음

> 분류 모델 생성 

![](https://velog.velcdn.com/images/finemann/post/dde78db1-1ebf-433c-a16e-6fdd48d350fd/image.png)

- Logistic Regression, SVM 등 총 5개의 분류 알고리즘 중에서 가장 안정적 성능을 보인 Random Forest 채용
- Feature Importance 추출 결과, EDA에서 예상했던 주요 변수들이 Feature Importance의 상위에 위치함을 확인

> 차원 축소 및 클러스터링

![](https://velog.velcdn.com/images/finemann/post/25a20d62-9203-4290-8722-00609d7a00f8/image.png)

- 위에서 선정한 분류 모델을 이용해 이탈 위험도 변수 생성 후, 상위 10개 feature importance 변수들을 이용해 UMAP 알고리즘을 이용해 2차원으로 데이터를 축소
- 축소된 데이터를 Gaussian Mixture Model 클러스터링 알고리즘을 이용해 8개의 그룹으로 군집화

![](https://velog.velcdn.com/images/finemann/post/52722bfb-33e3-41eb-8b51-86c3a5e8b385/image.png)

- 클러스터별 이탈 예측점수에 따라 이탈 high / mid / low 그룹으로 분류

---

### 분석 결과

![](https://velog.velcdn.com/images/finemann/post/bef22a09-6c6e-47f1-96fb-e0dd5167ceba/image.png)

- mid1/mid2에 대한 전략
  - 위 3가지 지표에서 high1/high2 그룹과 유사한 형태를 보이므로, high 그룹과의 연결점을 제거하고 low그룹으로 이동을 유도하도록 해당 지표 관련 해결책 제시
  - 1분기 대비 4분기 이용 비율이 높으므로(연간 사용 패턴이 불규칙하므로), 이를 낮추기위해(이용 패턴을 규칙적으로 하기 위해) 1분기에 카드 사용을 촉진하도록 유도책 제안

![](https://velog.velcdn.com/images/finemann/post/a0f22598-1827-4bec-8a56-29c572888a03/image.png)

- mid3에 대한 전략
  - Card_Category, Revolving_Bal 등의 지표에서 high 그룹과 유사한 형태를 보여 관련 해결책 제시
  - mid3 그룹은 채무액이 0인 반면 low 그룹에서는 채무액이 존재하므로, 리볼빙 또는 할부 등의 채무 서비스 이용을 촉진하는 프로모션 제안
  - mid3 그룹에서 platinum 등급의 카드 소유자가 없으므로 특정 소득 구간에 해당되는 고객에게 카드 등급 승급을 제안하여 충성고객 전환 유도
  
---

### **기대효과**

![](https://velog.velcdn.com/images/finemann/post/db2575be-73ab-4744-a82f-e8017ed41cb6/image.png)

```
mid 그룹 고객을 low 그룹으로 이동을 유도함으로서 
이탈 예측 점수 약 0.17(73%) 감소 효과
```

---

### Lesson & Learned

![](https://velog.velcdn.com/images/finemann/post/e74b1b25-2f7c-427b-bae6-f7679240c483/image.png)
