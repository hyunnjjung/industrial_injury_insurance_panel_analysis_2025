# 2025년 산재보험패널 데이터 기반 산업재해 피해자의 우울증 예측: 회귀 분석과 SHAP 분석을 통한 영향 요인 탐색

<br>

## 📚 연구 개요
산업재해 피해자의 정신건강, 특히 우울증은 신체 회복 및 직업 복귀에 큰 영향을 미칩니다. 본 연구는 **2025년 산재보험패널 제3차 코호트 1차년도 데이터**를 활용하여, **우울증 자가진단 점수(PHQ-9)** 를 예측하는 회귀/분류 모델을 개발하고, **SHAP 분석**을 통해 예측에 영향을 미치는 핵심 요인을 시각화 및 해석하였습니다.



## 🎯 연구 목적
- 회귀 모델을 통해 **우울증 점수(PHQ-9 총합)** 예측
- 점수 기준(15점 이상)을 바탕으로 **우울증 여부 이진 분류**
- **SHAP 분석**을 통해 예측에 영향을 미치는 변수 도출
- SMOTE 기법으로 데이터 불균형 해소 및 모델 성능 향상



## 📊 연구 방법
- **데이터**: 산재보험패널 제3차 코호트 1차년도(V2)
- **모델**: MLP 기반 회귀 및 이진 분류 모델
- **전처리**: 결측값 처리, 범주형 인코딩, 정규화
- **불균형 처리**: SMOTE 오버샘플링 적용
- **성능 평가**: MAE, RMSE (회귀), Accuracy, F1-score, Recall, Precision (분류)
- **해석 기법**: SHAP (Shapley Additive exPlanations)



## 🧠 주요 기술 스택
- Python
- Pandas, NumPy
- Scikit-learn, imbalanced-learn (SMOTE)
- TensorFlow / Keras
- SHAP



## 📂 파일 구성
| 파일명 | 설명 |
|--------|------|
| `2025_SanJaeInsurancePanel_Analysis_Poster.ipynb` | 전체 분석 노트북 (전처리 ~ 모델링 ~ 해석) |
| `README.md` | 프로젝트 설명 |



## 👥 연구진
| 이름     | 소속                          | 역할       |
|----------|-------------------------------|------------|
| 염동근   | 성결대학교 산업경영공학과     | 주저자     |
| 이채원   | 가톨릭대학교 데이터사이언스학과 | 공동연구자 |
| 설정석   | 고려대학교 통계학과           | 공동연구자 |
| 여현정   | 덕성여자대학교 컴퓨터공학과   | 공동연구자 |
| 차서은   | 동덕여자대학교 정보통계학과   | 공동연구자 |



## 📝 참고 문헌
1. 박수경. (2014). 산업재해 환자의 개인적 특성과 우울간의 관계. *Crisisonomy, 10(2)*, 85-103.  
2. 박수경, 김동기. (2006). 산재환자의 정신건강에 영향을 미치는 요인. *재활복지, 10(3)*, 150-174.  
3. 김태훈 외 (2023). 랜덤 포레스트를 이용한 성인의 우울증 예측. *Journal of The Korean Data Analysis Society, 25(4)*, 1449-1462.  
4. 신동석. (2019). 산업재해 및 교통사고 특성 비교 연구 [한성대학교 박사학위논문].



## 💡 시사점
- 정신건강 조기 예측을 통한 **맞춤형 재활 및 복귀 프로그램** 설계 가능  
- SHAP 분석 기반 **정책 제언 및 개입 요인** 제시  
- SMOTE 기법을 통한 **우울증 고위험군 예측 정확도 향상**
