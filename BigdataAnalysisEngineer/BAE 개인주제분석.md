# 7주차 과제 - 개인별 주제 분석

## 혼동행렬 (4과목 - 분석 모형 평가)

### 정의
- 분석 모델에서 구한 분류의 예측 번주와 데이터의 실제 분류 범주를 교차표 형태로 정리한 행렬
  
||긍정예측|부정예측|
|--|--|--|
|긍정(실제)|True Positive(TP)|False Negative(FN)|
|부정(실제)|False Positive(FP)|True Negative(TN)|

### 평가지표

- 정확도(Accuracy) = $\frac{TP+TN}{TP+TN+FP+FN}$
  - 실제 분류 범주를 정확하게 예측한 비율
  - 전체 예측에서 참 긍정(TP)과 참 부정(TN)이 차지하는 비율
- 오차 비율(Error Rate) = $\frac{FP+FN}{TP+TN+FP+FN}$
  - 실제 분류 범주를 잘못 분류한 비율
  - 오차 비율 = 1 - 정확도
- 재현율(Recall), 참 긍정률(TP Rate)  = $\frac{TP}{TP+FN}$
  - 실제로 긍정인 범주 중에서 긍정으로 올바르게 예측(TP)한 비율
  - 민감도(Sensitivity), Hit Rate로도 지칭
- 특이도(Specificity) = $\frac{TN}{TN+FP}$
  - 실제로 부정인 범주 중에서 부정으로 올바르게 예측(TN)한 비율
- 거짓 긍정률(FP Rate) = $\frac{FP}{TN+FP}$
  - 실제로 부정인 범주 중에서 긍정으로 잘못 예측(FP)한 비율
  - 거짓 긍정률 = 1 - 특이도
- 정밀도(Precision) = $\frac{TP}{TP+FP}$
  - 긍정으로 예측한 비율 중에서 실제로 긍정(TP)인 비율
- F1 지표(F1-Score) = 2$\times\frac{Precision\times Recall}{Precision + Recall}$
  - 정밀도와 민감도(재현율)를 하나로 합한 성능평가지표
  - 0~1 사이의 범위를 가짐
  - 정밀도와 민감도 양쪽이 모두 클 때 F1 지표도 큰 값을 가짐
- 카파 통계량(Kappa Statistic) = $\frac{Pr(a)-Pr(e)}{1-Pr(e)}$
  - $Pr(a)$: 예측이 일치할 확률
  - $Pr(e)$: 예측이 우연히 일치할 확률
  - 두 관찰자가 측정한 범주 값에 대한 일치도를 측정하는 지표
  - 모형의 평가 결과가 우연히 나온 결과가 아님을 설명하는 지표
  - 값이 1에 가까울수록 모델의 예측값이 실제값에 일치
  - 값이 0에 가까울수록 모델의 예측값과 실제값이 불일치
  - $0\leq \Kappa \leq 1$

## 앙상블