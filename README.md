# 2020 금융 빅데이터 페스티벌 
## [주제2] 보험금 청구 건 분류

https://programmers.co.kr/competitions/252/2020-miraeasset

|대회|기간|수행내용|결과|
|---|---|---------|-----|
|예선|~20.10.04|보험금 청구건 다중분류 모델 Competition| **1위** |
|본선|~20.10.30|알고리즘 포함 보고서 제출| **TOP3**   |
|결선|~20.11.27|비즈니스 활용방안 고안 및 프레젠테이션|보험금 청구분야 **최종 1위, 전체 우수상** |


## 📌Techniques
#### **Machine Learning, Business Intelligence**







## 📌사용한 주요 인사이트 

### 1) Modeling : Extra Tree + KNN 

- Randomness가 심한 Extra Tree의 특성을 보완하고 안정성을 높이고자 Ramdom state를 다르게 설정한 3가지 모델 앙상블
- 또한, 사례기반 모델인 KNN의 추가
- 본선에서는 자동지급을 먼저 분류하고, 그 다음 심사와 조사를 분류하는 Two-Stage model 고안

----------------------------------------------

### 2) Feature Engineering

- 자동지급, 심사, 조사의 분류에 청구보험금 관련 Feature들이 우수한 성능을 보였음
- 병원별, 질병별 평균 청구액과 각 개인의 청구액의 차이를 구한 Features들이 중요한 역할을 함

----------------------------------------------


### 3) Business Insight : 고객 유형화를 통한 보험 청구 적정성 평가 및 추천 서비스 제안

- 마이데이터 사업과 연계하여 고객 Segmentation 전략과, 활용 방안에 대하여 본선과 결선에서 피력
- 특히, 군집 기반 협업필터링(Collaborative Filtering) 을 활용하여 **군집 내 고객의 질병 유사도 기반 질병예측 모델 제안**

![image](https://user-images.githubusercontent.com/62705839/115139627-e04db300-a06d-11eb-899c-33dc60f9e93b.png)
![image](https://user-images.githubusercontent.com/62705839/115139649-0410f900-a06e-11eb-9d4f-7653f465a0cb.png)



## 📌 사용한 패키지와 버전
Pandas -- 0.25.1   
Numpy -- 1.16.5    
Matplotlib -- 3.1.1    
Seaborn -- 0.11.0    
Sklearn -- 0.23.1     




