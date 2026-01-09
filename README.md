# Global Analysis: Muscle Mass & Depression Correlation
(근육량과 우울증의 상관관계에 대한 통합 분석)

## 📌 Project Overview
이 프로젝트는 인종별(White, Black, Asian, Hispanic)로 파편화된 통계 데이터를 통합하여, **"근육량(Muscle Mass)과 우울증(Depression) 사이에 보편적인 상관관계가 존재하는가?"**를 규명하기 위한 데이터 분석 시뮬레이션입니다.

개별 연구에서 제공된 요약 통계(Summary Statistics)를 바탕으로 원본 데이터를 역설계(Reverse Engineering)하고, 이를 하나의 글로벌 데이터셋으로 통합하여 통계적 유의성을 검증했습니다.

## 📊 Key Findings
총 **2,201명**의 시뮬레이션 데이터를 통합 분석한 결과는 다음과 같습니다:

* **상관계수 (Pearson r):** `-0.1440`
* **P-value:** `1.13e-11` (p < 0.05, 매우 유의미함)
* **결론:** 인종이나 인구통계학적 특성을 불문하고, **근육량이 증가할수록 우울증 수치는 유의미하게 감소하는 경향**이 확인되었습니다.

## 🛠 Methodology
이 분석은 실제 raw data가 아닌, 기존 연구의 요약 통계치를 바탕으로 수행된 **Monte Carlo Simulation**입니다.

1.  **Input Data:** 4개 주요 인종 그룹의 $N$ (표본 수), $r$ (상관계수), $Slope$ (기울기).
2.  **Data Generation:** 다변량 정규분포(Multivariate Normal Distribution)를 사용하여 각 그룹의 특성을 반영한 가상 데이터 생성.
3.  **Global Analysis:** 생성된 데이터를 통합(Merge)하여 전체 회귀 분석 및 시각화 수행.

## 📁 Repository Structure
```bash
muscle-depression-analysis/
├── main.py              # 데이터 생성, 통합 분석 및 시각화 실행 코드
├── requirements.txt     # 필요 라이브러리 목록
├── muscle_depression_analysis.png  # 결과 그래프 (Result Plot)
└── README.md            # 프로젝트 설명서

Wonil Koh, Ph.D.
contact: wkoh1231@gmail.com
