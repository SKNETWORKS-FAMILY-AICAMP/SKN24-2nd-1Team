# SKN24_2nd_1Team
---
## 카드비

<!-- prettier-ignore-start -->
| 김지원 | 나혜린 | 박정은 | 진세형 | 황인규 |
| :---: | :---: | :---: | :---: | :---: |
| [![github](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/edu-ai-jiwon) | [![github](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/nngpfls) | [![github](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/brainkat) | [![github](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/gugu-eightyone) | [![github](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/hwang-in-kyu) |
<!-- prettier-ignore-end -->

---
## 1. 프로젝트 개요

프로젝트 이름: **카드사 VIP 이탈 예측 및 방지 모델 구축**

### 1-1. 개요
본 프로젝트는 국내 카드사의 VIP 회원 금융 거래 및 행태 데이터를 결합하여, 이용 금액·잔액 변화·연체 이력 등 금융 변수가 고객의 이탈(Churn)에 미치는 영향을 통계 및 머신러닝 관점에서 분석하였음. 단순히 단일 시점의 이탈 여부를 확인하는 것을 넘어, 6개월간의 시계열적 행동 패턴을 분석하여 이탈 전조 증상을 식별하고 선제적 방어 전략을 도출하는 데 목적이 있음.
방법론: 58만 명의 대규모 회원 데이터를 기반으로 회원·승인매출·잔액 등 8개 영역의 테이블을 정합하여 마스터셋을 구축함. 기본 분류 모델과 앙상블 모델을 활용하여 각 금융 지표가 이탈 확률에 기여하는 통계적 유의성을 검증함.
기대효과: 고가치 고객(VIP)의 유지율을 높이기 위한 데이터 기반의 타겟 마케팅 가이드라인 및 조기 경보 시스템 구축의 기초 인사이트를 제공함.

### 1-2. 프로젝트 배경
최근 카드업계는 가맹점 수수료 수익 비중이 30% 미만으로 하락하며 전통적인 수익 구조의 한계에 직면했다. 이는 14년 간 지속된 가맹점 수수료 인하 정책의 영향(1)으로, 2025년에도 수수료 수익 확보에 어려움을 보였다.  
이러한 환경 변화에 대응하기 위해 카드사들은 높은 연회비가 책정된 프리미엄 카드 비중을 확대하는 수익 구조 다변화 전략을 추진하고 있다. 2025년 2분기 기준 연회비 수익은 약 7% 상승하며 전체 수익 하락을 상회하는 핵심적인 역할을 수행했다.(2)  
특히 프리미엄 카드를 이용하는 VIP 고객은 높은 소비 여력을 바탕으로 백화점 등 대형 가맹점에서의 결제 비중이 높아 카드사 수익성에 기여하는 바가 크다(3)(4)(5). 또한 이들은 카드대출 상품 이용 시에도 상대적으로 낮은 연체율을 유지하여 자산 건전성 확보에도 긍정적인 영향을 미친다.  
본 프로젝트는 이와 같은 업계의 구조적 변화를 바탕으로, 카드사의 핵심 수익원인 VIP 고객의 이탈 예측을 목표로 한다.

---
## 2. 기술 스택

## 🛠 Tech Stack
| Category | Stack |
|----------|-------|
| 💻 Language | ![Python](https://img.shields.io/badge/PYTHON-3776AB?style=for-the-badge&logo=python&logoColor=white) |
| 📊 Data Processing | ![Pandas](https://img.shields.io/badge/PANDAS-150458?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NUMPY-013243?style=for-the-badge&logo=numpy&logoColor=white) |
| 🤖 Machine Learning | ![Scikit-Learn](https://img.shields.io/badge/SCIKIT--LEARN-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white) ![XGBoost](https://img.shields.io/badge/XGBOOST-228B22?style=for-the-badge&logo=xgboost&logoColor=white) ![LightGBM](https://img.shields.io/badge/LIGHTGBM-9ACD32?style=for-the-badge) ![RandomForest](https://img.shields.io/badge/RANDOM_FOREST-228B22?style=for-the-badge) ![DecisionTree](https://img.shields.io/badge/DECISION_TREE-8B4513?style=for-the-badge) ![Optuna](https://img.shields.io/badge/OPTUNA-3C3C3C?style=for-the-badge) |
| 📈 Visualization | ![Matplotlib](https://img.shields.io/badge/MATPLOTLIB-11557C?style=for-the-badge&logo=python&logoColor=white) ![Seaborn](https://img.shields.io/badge/SEABORN-4C72B0?style=for-the-badge) |

---

## 3. WBS
<img width="1596" height="976" alt="image" src="https://github.com/user-attachments/assets/707d26bd-5161-4242-a0f2-8bb7b577b983" />

---
## 4. 데이터 수집
### 4-1. 금융 합성 데이터
<img width="1286" height="725" alt="image" src="https://github.com/user-attachments/assets/869bc5d0-5f22-4133-96d8-7cbb2a32a32a" />
<img width="1258" height="1280" alt="image" src="https://github.com/user-attachments/assets/a2206356-b6e1-4b5a-9be5-7d19922baae8" />
<img width="1310" height="560" alt="image" src="https://github.com/user-attachments/assets/6030a090-eabb-48fb-9109-34ec81dc8705" />

- 수집 방식: 2018년 7월 ~ 12월(6개월) 데이터 수집 및 정리

- 수집 항목 (총 8개 table)
    1. 회원 정보 (18/79)
    <img width="1039" height="657" alt="image" src="https://github.com/user-attachments/assets/d3026775-9ca6-4503-aafd-dff543d8f4cb" />
    2. 신용 정보 (7/42)
    <img width="981" height="167" alt="image" src="https://github.com/user-attachments/assets/3353293a-87e3-4327-b324-22e8f979e13d" />
    3. 승인매출 정보 (23/430)
    <img width="1018" height="554" alt="image" src="https://github.com/user-attachments/assets/467ede0a-ff63-4480-88ff-d71290311b24" />
    4. 청구입금 정보 (4/58)
    <img width="1158" height="75" alt="image" src="https://github.com/user-attachments/assets/f5efd9ac-0a91-40e1-9c87-dd43516da94c" />
    5. 잔액 정보 (7/83)
    <img width="1095" height="142" alt="image" src="https://github.com/user-attachments/assets/11ddbf6a-3866-4744-89dd-483eb915efb1" />
    6. 채널 정보 (4/105)
    <img width="1018" height="79" alt="image" src="https://github.com/user-attachments/assets/ccacbf52-826f-4b47-9a1c-f0b3b306d3f6" />
    7. 마케팅 정보 (8/64)
    <img width="1021" height="160" alt="image" src="https://github.com/user-attachments/assets/6e74edaa-2ed7-458b-9d18-a60d26cade9a" />
    8. 성과 정보 (7/49)
    <img width="1017" height="137" alt="image" src="https://github.com/user-attachments/assets/fa1576b3-3ec8-4b89-9a1a-c553be63fc83" />

---
## 5. 데이터 통합 & 전처리

### 5-1. 데이터 통합

#### 5-1-1. 각 테이블의 7~12월 파일 통합
<img width="976" height="551" alt="image" src="https://github.com/user-attachments/assets/947bbf23-ccdd-4338-8e2c-23d16f219e16" />
<img width="920" height="297" alt="image" src="https://github.com/user-attachments/assets/9c429e06-3fb8-4226-a611-eda540f33fde" />

#### 5-1-2. 테이블끼리의 통합
<img width="1001" height="424" alt="image" src="https://github.com/user-attachments/assets/e6883354-5a5a-4dc3-9476-55343d3467cf" />

### 5-2. 전처리

#### 5-2-1. 자료형 변환
<img width="1055" height="170" alt="image" src="https://github.com/user-attachments/assets/e660850b-3bfd-4e5b-bf68-761a16b535f1" />

#### 5-2-2. 이상치, 결측치 제거
<img width="1273" height="423" alt="image" src="https://github.com/user-attachments/assets/3bcb0441-3dea-4178-99e4-6821c83d6360" />
<img width="1046" height="317" alt="image" src="https://github.com/user-attachments/assets/f52b7bde-272e-471e-8574-9ff709510526" />
<img width="1011" height="291" alt="image" src="https://github.com/user-attachments/assets/b22e7da8-2fef-4fdd-988d-323c19a66888" />
<img width="311" height="685" alt="image" src="https://github.com/user-attachments/assets/18948f31-e1fe-402a-92c3-4363144b08e0" /> <img width="338" height="714" alt="image" src="https://github.com/user-attachments/assets/0b3a358b-240d-4b4f-96fa-d2d76bfba248" /> <img width="428" height="194" alt="image" src="https://github.com/user-attachments/assets/0edd3b74-a8b3-40bc-9f37-c639faed757f" />

#### 5-2-3. 불필요 컬럼 제거
<img width="1020" height="481" alt="image" src="https://github.com/user-attachments/assets/bf0ffe14-84c1-4b36-9799-cf50eb14676a" />

---
## 6. 파생 변수

### 6-1. X 데이터
‘양육자녀_유무’
<img width="786" height="836" alt="image" src="https://github.com/user-attachments/assets/8f2c6239-8ca5-4171-8987-4f46d778d9a0" />

### 6-2. y 데이터
<img width="1249" height="101" alt="image" src="https://github.com/user-attachments/assets/75bb203f-cb5e-4dce-90e3-de9c19c00341" />
<img width="773" height="256" alt="image" src="https://github.com/user-attachments/assets/f61a9201-0377-4baa-b3c8-75034145f5fe" />

---

### 7. 모델(XGBoost, Decision Tree, RandomForest, LightGBM)

### 7-1. XGBoost
<img width="762" height="48" alt="image" src="https://github.com/user-attachments/assets/ced5a775-731f-46e9-b790-103a1410a646" />  
<img width="452" height="211" alt="image" src="https://github.com/user-attachments/assets/50fa5c7d-7183-4529-a68c-8d3ff3d58963" />  

Precision 0.66 → 떠날 것 같다고 예측한 사람 중 66%가 실제로 이탈  
Recall 0.42 → 실제 이탈자의 42%만 탐지 (58%는 놓침)  
F1-Score 0.51 → Precision과 Recall을 종합한 점수로, 이탈 탐지 성능은 보통 수준  

<img width="690" height="590" alt="image" src="https://github.com/user-attachments/assets/60096bb2-74ce-4385-931e-48968413cdc4" />  

ROC-AUC 0.9944 → 모델이 이탈자(1)와 비이탈자(0)를 점수 기준으로 구분하는 능력이 매우 뛰어남  

### 7-2. Decision Tree
<img width="392" height="237" alt="image" src="https://github.com/user-attachments/assets/b9d4d87e-8072-4c06-b434-731f8db7b30b" />  

max_depth=4, class_weight={0:1, 1:5}로 모델을 단순화하고 이탈자 가중치 부여  

<img width="395" height="145" alt="image" src="https://github.com/user-attachments/assets/f1bcbe10-4eb2-4504-8498-81bcc2420b54" />  

Precision → 초기 결과 0.06 -> 개선 결과: 0.35 (약 6배 상승한 것으로 봄)  
Recall → 초기 결과 0.92 -> 개선 결과 0.74 ( 실제 이탈자의 74% 확인시켜줌)  
F1-Score → 초기 결과 0.11 -> 개선 결과 0.48 (의존도 어느 정도 방지되어 성능 향상 된 것으로 봄)  

<img width="1957" height="974" alt="image" src="https://github.com/user-attachments/assets/7efbdaca-57bd-4041-ab8e-e7af7ba6c9f0" />  

트리 분류 시각화

### 7-3. RandomForest
<img width="519" height="33" alt="image" src="https://github.com/user-attachments/assets/36cd9cda-a066-46d6-8bfd-951ea76c0b06" />  

test_size → 전체 데이터의 25%를 테스트 데이터 설정  
stratify → 이유 : 테스트셋에 1이 거의 없을 수 있음  

<img width="440" height="23" alt="image" src="https://github.com/user-attachments/assets/1c15c5b5-7bff-4540-81c7-68ccf33f2de2" />  

max_depth=5로 트리 깊이 설정  
random_state로 난수 고정  

<img width="427" height="301" alt="image" src="https://github.com/user-attachments/assets/f06f9b3e-6523-43fe-b7b0-aa6d4fd9d9fd" />

Precision → 0.58  
Recall → 1.00  
F1-Score → 0.74  

### 7-4. LightGBM  
1️⃣시계열 (time split) 기반의 고객 이탈 예측 LightGBM 모델  

time split 기준으로 분리한 데이터 사용 (사용자 기반 그룹 분할방법 작업한 상태로 적용)  
시계열 (time split) 핵심: 과거 데이터로 학습하고, 미래 데이터로 시험 보는 것  
과적합 방지 목적으로 하이퍼파라미터 설정  

<img width="301" height="100" alt="image" src="https://github.com/user-attachments/assets/4b71b871-784e-47a6-a960-0eee08b148fa" />  

결과:  
Time-based split  
기간 split 기준: 11월  
훈련 이탈율: 0.75%  
테스트 이탈율: 1.11%  

<img width="1155" height="490" alt="image" src="https://github.com/user-attachments/assets/8455a9c2-ef6f-4238-90ae-85242246abd6" />  

ROC - 점선 (대각선) 동전 던지기 수준 (찍는 것과 같음)  
AUC- 파란 실선  모델  점수 1.00  
실제 이탈자는 몇 명이나 예측했는지 + 이탈 안한 고개을 얼마나 잘못 이탈 예측했는지 

2️⃣사용자 기반 그룹 분할된 고객 이탈 예측 LightGBM 모델  
GroupShuffleSplit 80:20 비율로 데이터를 발급회원번호로 분리한 모델  
- 데이터를 그룹 단위로 분리하여 학습/테스트 인덱스를 무작위로 생성합니다. 여기서 그룹이란 샘플을 특정 기준(예: 사용자 ID, 지역 등)으로 묶은 것을 정수로 표현한 것입니다.  

Precision 0.91 →  "이 사람 떠날 것 같다"고 한 사람 중 91%가 실제로 이탈  
Recall 1.00 → 실제 이탈자를 거의 한 명도 빠짐없이 탐지  
F1-Score 0.95 → Precision과 Recall을 합친 종합 점수, 매우 우수 

3️⃣LightGBM Optuna 활용  
optuna.create_study 함수: 모델이 최적의 하이퍼파라미터 찾기 위해 수행하는 반복하는 실험 과정  
과적합  방지 목표로 optuna 하이퍼파라미터 설정값 정의  

결과:  
최적 파라미터 출력  
최적 파라미터로 학습했을 때 F1 점수가 0.963  

Precision 0.91 →  "이 사람 떠날 것 같다"고 한 사람 중 91%가 실제로 이탈  
Recall 1.00 → 실제 이탈자를 거의 한 명도 빠짐없이 탐지  
F1-Score 0.95 → Precision과 Recall 두 가지를 합친 종합 점수 95점 
