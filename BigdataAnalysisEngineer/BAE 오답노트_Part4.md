# PART 4 빅데이터 결과 해석

## CHAPTER 01 분석 모형 평가 및 개선

### 챕터 마무리 문제

|번호|답|번호|답|번호|답|
|:--:|:--|:--:|:--|:--:|:--|
|1|<span style='color:red'>2</span> - 정답: 3|2|<span style='color:skyblue'>2</span>|3|<span style='color:skyblue'>2</span>|
|4|<span style='color:red'>4</span> - 정답: 1|5|<span style='color:red'>1</span> - 정답: 4|6|<span style='color:red'>3</span> - 정답: 2|
|7|<span style='color:skyblue'>2</span>|8|<span style='color:red'>3</span> - 정답: 1|9|<span style='color:skyblue'>2</span>|
|10|<span style='color:red'>3</span> - 정답: 2|11|<span style='color:skyblue'>2</span>|12|<span style='color:skyblue'>4</span>|
|13|<span style='color:red'>3</span> - 정답: 1|14|<span style='color:red'>4</span> - 정답: 1|15|<span style='color:red'>4</span> - 정답: 3|
|16|<span style='color:red'>1</span> - 정답: 3|17|<span style='color:skyblue'>1</span>|18|<span style='color:red'>2</span> - 정답: 4|
|19|<span style='color:red'>3</span> - 정답: 2|20|<span style='color:skyblue'>1</span>|||

### 오답노트 + 관련 개념 정리

1\. 회귀 모형 평가 지표

- MAE(평균절대오차, Mean Absolute Error): 오차에 절댓값을 취해 평균한 값
- MSE(평균제곱오차, Mean Squared Error): 오차를 제곱하여 평균한 값
- RMSE(평균제곱근오차, Root Mean Squared Error): MSE에 제곱근을 씌운 값
- MAPE(평균절대백분율오차, Mean Absolute Percentage Error): MAE를 퍼센트로 변환한 값

4\. 결정계수($R^2$) = $\frac{SSR}{SST}$ = $\frac{SST-SSE}{SST}$ = $1-\frac{SSE}{SST}$

- SST(Total Sum of Squares): 전체제곱합
- SSR(Regression Sum of Squares): 회귀제곱합
- SSE(Error Sum of Squares): 오차제곱합

5\. 혼동행렬 정확도: 전체 데이터 중 예측을 정확하게 한 데이터의 비율

6\. 혼동행렬 정밀도: Positive로 예측한 데이터 중 실제 Positive인 데이터의 비율

8\. 교차 검증 방법

- K-fold 교차 검증: k개의 fold로 나누어 (k-1)개는 학습에, 나머지 한 개는 검증에 사용
- 홀드아웃 교차 검증: 무작위로 7:3 또는 8:2의 비율로 학습 데이터와 검증 데이터로 나누는 방법
- 리브-p-아웃 교차 검증: p개의 관측치만 검증 데이터로 사용하고 나머지는 학습 데이터로 사용하는 방법

10\. 모수 검정: 모집단의 분포를 가정하고 표본평균, 표준편차 등을 이용하여 집단 간 차이를 검정
<br>비모수 검정: 모집단의 분포를 가정하지 않고, 순위나 부호를 검정통계량으로 사용

13\. 모집단에 대한 유의성 검정

- Z-검정: 추출된 표본이 모집단에 속하는지 검증
- t-검정: 평균값 검증(1-way), 두 집단의 평균 비교(2-way)
- ANOVA: 두 개 이상 집단의 평균 비교
- 카이제곱 검정: 분산을 알고 있을 때 두 집단의 동질성 검정
- F-검정: 두 모집단 분산 차이가 유의한지 검증

적합도 검정

- Q-Q plot: 관측치의 분포가 정규분포에 얼마나 가까운지 시각적으로 표현
- 카이제곱 검정: 어떤 그룹이 서로 독립인지 아닌지 확인하는 방법
- 샤피로-윌크 검정: 데이터의 정규성을 검증하는 방법
- 콜모고로프 스미르노프 검정: 데이터가 예상되는 분포에 얼마나 잘 맞는지를 검증하는 방법

14\. L1 규제: 모형의 모든 가중치의 절댓값을 손실함수에 추가
<br>L2 규제: 모형의 모든 가중치들의 제곱의 합을 손실함수에 추가

15\. 편향(Bias): 학습 알고리즘에서 잘못된 가정을 했을 때 발생하는 오차
<br>분산(Variance): 학습 데이터에 내재된 변동 때문에 발생하는 오차
<br>편향-분산 트레이드오프: 편향과 분산의 관계 (일반적으로 분석 모형이 복잡할수록 편향은 낮아지고, 분산은 높아짐)

16\. 매개변수 최적화 방법

- 경사하강법: 손실함수의 전역 최솟값을 찾아 가는 방법
- 확률적 경사하강법: 배치의 크기가 1인 배치 경사하강법
- 미니 배치 확률적 경사하강법: 배치 크기가 10~1,000인 배치 경사하강법
- AdaGrad:

17\. 경사하강법 알고리즘은 현재 지점에서 다음 지점으로 이동할 때, 기울기에 학습률(보폭)을 곱하여 다음 지점을 결정

18\. 부트스트랩(Bootstrap)

- 부트스트랩을 활용한 앙상블 기법은 배깅
- 배깅은 중복을 허용하지만 페이스팅(Pasting)은 중복을 허용하지 않음

19\. 앙상블 기법

- 소프트 보팅(soft voting): 분류 모형 여러 개가 예측한 레이블의 호가률을 평균 내어 가장 확률이 높은 레이블을 최종 결과 값을 채택하는 방법
- 하드 보팅(hard voting): 분류 모형 여러 개가 예측한 결과 중 가장 많이 나온 결과를 최종 결과로 사용하는 것
- 배깅 -> 과대적합을 줄이고 모형의 분산을 줄이는 데 도움이 됨

## CHAPTER 02 분석 결과 해석 및 활용

### 챕터 마무리 문제

|번호|답|번호|답|번호|답|
|:--:|:--|:--:|:--|:--:|:--|
|1|<span style='color:skyblue'>4</span>|2|<span style='color:red'>4</span> - 정답: 3|3|<span style='color:red'>1</span> - 정답: 3|
|4|<span style='color:red'>3</span> - 정답: 4|5|<span style='color:red'>1</span> - 정답: 2|6|<span style='color:skyblue'>1</span>|
|7|<span style='color:skyblue'>1</span>|8|<span style='color:skyblue'>1</span>|9|<span style='color:skyblue'>4</span>|
|10|<span style='color:skyblue'>3</span>|11|<span style='color:skyblue'>4</span>|12|<span style='color:skyblue'>3</span>|
|13|<span style='color:skyblue'>2</span>|14|<span style='color:red'>1</span> - 정답: 4|15|<span style='color:skyblue'>1</span>|
|16|<span style='color:skyblue'>2</span>|17|<span style='color:skyblue'>2</span>|18|<span style='color:skyblue'>1</span>|
|19|<span style='color:skyblue'>3</span>|20|<span style='color:skyblue'>4</span>|||

### 오답노트 + 관련 개념 정리

1\. DNN(Deep Neural Network): 대표적인 블랙박스 모형

2\. 랜덤 포레스트 모형의 변수 중요도

- 회귀 문제: 각 변수가 예측 오차와 노드 순수도 증가에 얼마나 기여하는지 각각 %IncMSEdhk IncNodePurity를 이용하여 계산
- 분류 문제: 각 변수가 정확도와 노드 불순도 개선에 얼마나 기여하는지 각각 MeanDecreaseAccuracy와 MeanDecreaseGini를 이용하여 계산

3\. 부분 의존도 plot: 1~2개의 독립변수와 종속변수 간의 전반적인 관계를 파악하기 위한 전역적인 방법 (분석 모형 전체에 대한 변수 관계를 나타냄)
<br>Shap 모델: 개별 관측치 각각에 대한 해석이 필요한 경우

4\. 총 소유 비용(TCO, Total Cost of Ownership): 자산을 획득할 때 드는 비용뿐 아니라 교육학습, 유지보수 등의 제반비용을 고려하여 산출되는 총 비용

5\. 순현재가치(NPV, Net Present Value): 투자 시작 시점부터 사업이 끝나는 시기까지 연도별로 편익과 비용을 현재 가치로 환산한 값

14\. 도트 플롯맵: 위도, 경도 값을 가지고 있는 데이터의 경우, 각 지리적 좌표 위에 점을 찍어서 데이터를 나타내는 방법
<br>버블 플롯맵: 도트 플롯 맵과 달리 점이 아니라 데이터 값의 크기에 따라 점의 크기를 다르게 나타내는 방법

## 과목 마무리 문제

1\. Throughput: 시뮬레이션에서 사용하는 평가기준, 단위 시간당 처리량