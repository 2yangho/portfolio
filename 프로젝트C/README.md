## 통신사 VOC 분석

---

### **프로젝트 개요**

> 배경

```
통신사 A는 고객들로부터 다양한 의견을 VOC(고객의 목소리)를 통해 수신하고 있다. 
그럼에도 불구하고 고객 만족도는 떨어져 있고, 몇몇 서비스 부문에서 불만이 높다. 
이러한 고객의 VOC를 분석하여 주요 불만사항을 파악하고, 서비스를 개선하고자 한다. 
VOC 데이터를 깊게 파고들어 고객의 진짜 불만, 해결방법을 찾아내는 것이 목표이다.
```

> 분석목적

```
주요 고객 불만사항 개선을 통해 서비스 만족도 증가, 고객 이탈 위험 감소
```

---

### **분석 과정**

> 자연어 처리를 이용한 키워드 추출, LDA를 이용한 토픽 분류

![](https://velog.velcdn.com/images/finemann/post/36fd34cd-e5ab-4cd7-b288-996d4d665741/image.png)

- text library를 이용해 고객 불만사항 텍스트 데이터에서 키워드를 추출한 뒤, 키워드별 빈도수를 나타냄
- 해당 토픽 0 ~ 토픽 5 주제들을 변수로서 원본 각 데이터에 추가

---

### **분석 결과**

> 지역별 / 문의상태별 문의 유형(토픽) 분석 결과

![](https://velog.velcdn.com/images/finemann/post/c0bd416b-f247-4b6d-ae96-84da9b6d2548/image.png)

- Billing Issue 관련하여 Florida, Georgia 주가 유독 눈에띄게 많다.
- Georgia주의 Data Cap 관련 문의수가 다른 주에 비해 독보적으로 많다.
- Tennessee주는 다른 유형에서 문의수에 이상은 없지만 유독 Data Cap 관련 문의수가 많다.
- 대부분의 문의유형의 경우 Closed / Solved 상태의 비율이 80%를 차지하지만, "Data Cap"유형일때는 해당 비율이 60%대까지 낮아진다

> 정리

```
connection 관련 문제가 많았던 Florida 주 문제 부분,
Data Capacity 유형에서 closed/solved상태 비율이 낮은 부분
두 부분에서 해당 통신사에서 우선적으로 해결해야할 과제로 판단된다. 
```
---

### **Lesson & Learned**

![](https://velog.velcdn.com/images/finemann/post/8938b978-3267-4fa1-acc3-94b4e870da33/image.png)


