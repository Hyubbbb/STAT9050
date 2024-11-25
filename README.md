# STAT9050: Advanced Topics in Applied Statistics

## 📚 프로젝트 개요
- **과목명**: 연세대학교 일반대학원 통계데이터사이언스학과 응용통계학특수문제 (STAT9050)
- **학기**: 2024년 2학기 (석사 3학기)
- **프로젝트 주제**: Survival Analysis를 활용한 다양한 샘플링 기법 비교 및 개선 (개인 프로젝트)
- **제출 기한**: 2024.12.18. 18:00 (KST)

---

## 🗝️ 프로젝트 키워드
- Survival Analysis
- Case-cohort design
- Nested case-cohort design
- End-Point Sampling

---

## 📅 프로젝트 기간
- 2024년 9월 ~ 12월

---

## 📂 폴더 구조
```
├── data/               # 데이터 파일 (제공된 데이터셋 포함)
├── report/             # 최종 보고서 (LaTeX, PDF 형식)
├── results/            # 결과 보고서 및 시각화 자료
├── rmd/                # 분석 및 시뮬레이션 스크립트 (Python, R)
└── README.md           # 리드미 파일 (현재 문서)
```

---

## 🛠️ 사용된 도구 및 라이브러리
- **언어**: R
- **라이브러리**:
  - R: `survival`, `dplyr`, `ggplot2`

---

## 📊 분석 개요
본 프로젝트에서는 생존 분석 기법을 사용하여 다양한 샘플링 방법(Case-cohort, Nested Case-control)을 비교하고, 효율적인 추정 방법을 탐색합니다. 특히, 각 샘플링 방법의 추정 효율성을 개선하기 위해 추가적인 샘플링 스킴(End-Point Sampling)과 Missing data imputation 기법을 적용할 예정입니다.

### 주요 연구 문제
1. **Cox 비례위험모형**을 사용한 변수 추정 및 표준오차 계산.
2. **Likelihood 기반 추정**을 통해 서브샘플링(cohort) 디자인 비교.
3. **샘플링 효율성 개선**을 위한 대안 기법 제안 및 검증.

---

## 📈 분석 방법
1. **Generate survival data**: 시뮬레이션을 통해 Weibull 분포를 따르는 생존시간 데이터 생성.
2. **Apply sampling techniques**: Case-cohort 및 Nested Case-control 샘플링 기법 적용.
3. **Improve efficiency**: 기존 추정 방법과 개선된 방법 비교 분석.

---

## 📝 참고 자료
- [Statistical Writing Guide](https://statds.github.io/stat-writing/index.html)
- 강의 자료 및 수업 노트

---

## 📄 보고서 제출
최종 보고서는 [report](report/) 폴더 내에 LaTeX 및 PDF 형식으로 포함되어 있으며, 분석 과정 및 결과를 요약합니다. 

- **제출 파일**: `STAT9050_Project_Hyubkim.pdf`
  - [**깃허브 링크**](https://github.com/Hyubbbb/STAT9050)

---

## 🧑‍💻 작성자
- 김협(연세대학교 일반대학원 통계데이터사이언스학과 석사과정 3학기)

--- 

### 🔗 링크
- [**GitHub Repository**](https://github.com/Hyubbbb/STAT9050)

---
