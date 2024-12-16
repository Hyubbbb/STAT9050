# A Comparative Study of Sub-Sampling Designs: Case-Cohort vs. Naive and Probabilistic End-Point Sampling

## 📚 프로젝트 개요  
- **과목명**: 연세대학교 일반대학원 통계데이터사이언스학과 응용통계학특수문제 (STAT9050)  
- **학기**: 2024년 2학기 (석사 3학기)  
- **프로젝트 주제**: 생존 분석에서 샘플링 디자인 비교: Case-Cohort 및 End-Point Sampling의 효율성 평가  
- **제출 기한**: 2024.12.18. 18:00 (KST)  

---

## 🗝️ 프로젝트 키워드  
- **Survival Analysis**  
- **Cox Proportional Hazards Model**  
- **Case-Cohort Sampling**  
- **End-Point Sampling** (Naive, Probabilistic)  
- **Bias and Mean Squared Error (MSE)**  

---

## 📅 프로젝트 기간  
- **2024년 9월 ~ 12월**  

---

## 📂 폴더 구조  

```
├── data/                   # 데이터 파일 및 문서
│   ├── Desc_MIMIC3.pdf     # 데이터 설명서 (MIMIC3)
│   └── mimic3_final.csv    # Real Dataset
│  
├── plot/                   # 시각화 결과  
│   ├── fig1_bias.png       # Bias 비교 그래프  
│   └── fig2_MSE.png        # MSE 비교 그래프  
│  
├── report/                 # 최종 보고서  
│   └── STAT9050_Project_Hyubkim.pdf  
│  
├── rmd/                    # 분석 및 시뮬레이션 코드 (R Markdown)  
│   ├── STAT9050_Mid_Code_Hyub_Kim.Rmd             # 시뮬레이션 코드  
│   ├── STAT9050_Mid_Code_Hyub_Kim.html            # 시뮬레이션 HTML 결과  
│   ├── STAT9050_Mid_Code_Hyub_Kim_Realdata.Rmd    # Real Data 분석 코드  
│   └── STAT9050_Mid_Code_Hyub_Kim_Realdata.html   # Real Data 분석 결과  
│  
├── README.md                   # 리드미 파일 (현재 문서)  
└── STAT9050_Project_SP24.pdf   # 교수님 제공 문서  
```  

---

## 🛠️ 사용된 도구 및 라이브러리  
- **언어**: R  
- **라이브러리**:  
  - `survival`  
  - `dplyr`  
  - `ggplot2`  

---

## 📊 연구 개요  
- 본 프로젝트는 **Survival Analysis**를 기반으로 다양한 샘플링 디자인의 efficiency를 비교하였습니다.
- 특히 **Cox 비례위험모형** 하에서 **Case-Cohort Sampling**과 **End-Point Sampling** (Naive & Probabilistic)을 중심으로 **Bias**와 **Mean Squared Error (MSE)** 를 평가하였습니다.  

### 주요 연구 내용  
1. **Simulation Analysis**  
   - Weibull 분포 기반 데이터를 생성하여 각 샘플링 방법의 효율성을 평가.  
   - Case-Cohort 및 End-Point Sampling의 성능 비교
     - 확률적 End-Point Sampling ($p(y) = \min(1, y)$ 및 $p(y) = \min(1, 0.7y^2)$)의 성능 비교.  
       - Naive End-Point Sampling과의 비교

2. **Real Data Analysis**  
   - MIMIC3 데이터를 활용하여 실제 환경에서 샘플링 방법의 성능을 검증.  
   - Case-Cohort와 End-Point Sampling의 **Bias**와 **MSE** 비교 분석.  

3. **결론**  
   - **Simulation, Real Data 모두 확률적 End-Point Sampling이 Case-Cohort 대비 우월한 성능을 보임**
     - 추가적으로, Simulation에서는 $p(y)=\min(1, y)$가 가장 효율적이었으나, Real Data에서는 $p(y)=\min(1, 0.7y^2)$가 더 나은 성능을 보임.  

---

## 📈 연구 결과  
### Simulation Results  
- **End-Point Sampling** $p(y)=\min(1, y)$ : 가장 낮은 Bias와 MSE를 달성.  
- **Case-Cohort Sampling**: 랜덤 선택 특성상 상대적으로 낮은 효율성.  

### Real Data Results  
- **End-Point Sampling** ($p(y)=\min(1, 0.7y^2)$): Real Data에서 가장 낮은 Bias와 MSE를 기록.  
- **Naive End-Point Sampling**: 높은 MSE로 인해 비효율적임을 확인.  

---

## 🔗 관련 자료  
- **깃허브 링크**: [**GitHub Repository**](https://github.com/Hyubbbb/STAT9050)  
- **최종 보고서**: [**STAT9050_Project_Hyubkim.pdf**](report/STAT9050_Project_Hyubkim.pdf)  

---

## 🧑‍💻 작성자  
- **이름**: 김협  
- **소속**: 연세대학교 일반대학원 통계데이터사이언스학과 석사과정 (3학기)  
- **이메일**: hyub@yonsei.ac.kr  

---

### 📄 참고 자료  
- Cox, D. R. (1972). Regression Models and Life-Tables. *Journal of the Royal Statistical Society*.  
- Yao, Y., Yu, W., \& Chen, K. (2017). End-Point Sampling. *Statistica Sinica*.  
- Barlow, W. E., et al. (1999). Efficient methods for weighted Cox regression. *Biometrics*.  

---