## 💳 ML-Based Financial Risk Analysis & Personalized Credit Evaluation System  
📅 Sep. 2024 – Dec. 2024  
🎯 *Predicting personal financial risk and designing tailored credit strategies using machine learning*

---

### 🧩 Overview  
- 신용 점수, 재정 상태, 인구통계 정보 기반으로 **개인 금융 리스크 예측 및 맞춤형 신용 평가 시스템** 구축  
- 기존 신용 평가 모델의 한계를 보완하고, **고객 및 금융기관 모두에게 실질적인 인사이트**를 제공하는 솔루션 설계  
- Streamlit 기반 **웹 예측 앱 구현**으로 사용자 실용성 확보  

---

### 📊 Data Summary

- **Data Type**: Credit score, financial attributes, demographic info  
- **Source**: [Kaggle - financial_risk_assessment](https://www.kaggle.com/)  
- **Volume**: 150,000 entries × 30 features  
- **Label**: Default status (Yes/No)

---

### 📌 Key Insights

#### 🔄 1) Feature Correlation Analysis  
- 주요 수치형 변수 간 상관관계 분석 → 다중 공선성 문제 없음  
- PCA를 통해 모델링에 유의미한 변수 3~4개로 축소

#### ⚖️ 2) Default Status Distribution  
- 전체 고객 중 **파산 고객 비율이 낮아 데이터 불균형 존재**  
- 모델 학습 시 Stratified Sampling 및 가중치 조정 필요

---

### 🧠 Modeling Workflow

#### 🚩 Step 1: 파산 여부 분류  
- PCA로 주요 피처 4개로 차원 축소  
- DNN으로 파산 여부 예측  
- 파산 고객 클러스터링 (5개 그룹) → 파산 원인 세분화

#### 📉 Step 2: 신용 점수 상/하위 그룹 추출  
- Credit Score 영향 피처 3개 추출  
- 하위 10% 고객을 위한 **개선 피드백 시스템 설계**

#### 📊 Step 3: 신용 등급 분류 + 파산 예측  
- `K-means`로 신용 점수 **Low / Medium / High** 3단계로 분류  
- 각 그룹별로 **Random Forest** 모델 학습 → 파산 여부 예측  
- 전체 정확도: **88~89%**, 주요 피처: `LTV`, `property_value`, `dtir1`

---

### 💻 Deployment: Streamlit App  
- 고객 정보 입력 시 파산 여부 예측 제공  
- 📍 실시간 신용 등급 분류 + 위험도 진단  
- 사용자 중심 금융 의사결정 도우미

---

### 🧰 Tech Stack

- **Data Analysis**: `Python`, `Pandas`, `NumPy`, `Scikit-learn`  
- **ML Models**: `K-means`, `PCA`, `Random Forest`, `DNN`  
- **Visualization**: `Matplotlib`, `Seaborn`  
- **Web App**: `Streamlit`  

---

### 🎯 Achievements

- ✅ 고도화된 신용 등급 분류 및 파산 예측 모델링  
- ✅ 데이터 기반 맞춤형 신용 개선 전략 제안  
- ✅ Streamlit 웹 앱 구축으로 서비스 실용성 강화  
- ✅ 고객 중심 AI 금융 서비스 설계 경험 확보  

---
