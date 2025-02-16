# PART 3 빅데이터 모델링

## CHAPTER 01 분석 모형 설계

### 챕터 마무리 문제

|번호|답|번호|답|번호|답|
|:--:|:--|:--:|:--|:--:|:--|
|1|<span style='color:red'>②</span> - 정답: ①|2|<span style='color:red'>②</span> - 정답: ③|3|<span style='color:red'>③</span> - 정답: ①|
|4|<span style='color:red'>①</span> - 정답: ②|5|<span style='color:red'>③</span> - 정답: ④|6|<span style='color:red'>③</span> - 정답: ②|
|7|<span style='color:skyblue'>④</span>|8|<span style='color:skyblue'>④</span>|9|<span style='color:skyblue'>③</span>|
|10|<span style='color:red'>②</span> - 정답: ①|11|<span style='color:skyblue'>①</span>|12|<span style='color:red'>②</span> - 정답: ④|
|13|<span style='color:skyblue'>②</span>|14|<span style='color:skyblue'>③</span>|15|<span style='color:red'>①</span> - 정답: ③|
|16|<span style='color:skyblue'>②</span>|17|<span style='color:skyblue'>④</span>|18|<span style='color:red'>①</span> - 정답: ③|
|19|<span style='color:skyblue'>①</span>|20|<span style='color:skyblue'>③</span>||

### 오답노트 + 관련 개념 정리

1\. 범주형 종속변수 -> 분류 분석, 선형 회귀 모형은 종속변수가 연속형인 경우 활용 가능

2\. 의사결정나무 -> 분류 및 예측 수행 (군집 분석 X)

3\. 랜덤포레스트, 인공신경망, SVM: 지도 학습 알고리즘

4\. 어떤 집단인지 구분한다 -> 분류 분석

5\. 의사결정나무, 나이브 베이즈, KNN -> 정해진 집단으로 분류하는 분석 방법

6\. 비지도 학습의 종류: 군집화, 차원축소, 연관분석, 자율학습 인공신경망

10\. 하이퍼파라미터: 모형 외부 요소, 성능에 간접적 영향, 사용자가 직접 설정
<br>파라미터: 모형 내부 요소, 성능에 직접적 영향, 모형에서 학습 결과 값으로 자동 결정

12\. 모델링 절차: 데이터 마트 구축 -> EDA -> 모델링 -> 모델 성능평가

15\. 모든 데이터를 학습에 사용 -> 과적합 현상 발생 위험 큼 -> 학습용/검증용/평가용 데이터 분할해야

18\. 검증 데이터: 학습된 모델의 성능을 검증하고 개선하기 위해 사용
<br> 테스트 데이터: 최종 모델의 성능 평가

## CHAPTER 02 분석 기법 적용

### 챕터 마무리 문제

|번호|답|번호|답|번호|답|
|:--:|:--|:--:|:--|:--:|:--|
|1|<span style='color:red'>2</span>|2|<span style='color:red'>2</span>|3|<span style='color:red'>4</span>|
|4|<span style='color:skyblue'>4</span>|5|<span style='color:skyblue'>4</span>|6|<span style='color:red'>3</span>|
|7|<span style='color:red'>1</span>|8|<span style='color:red'>2</span>|9|<span style='color:red'>2</span>|
|10|<span style='color:skyblue'>4</span>|11|<span style='color:red'>1</span>|12|<span style='color:skyblue'>3</span>|
|13|<span style='color:skyblue'>2</span>|14|<span style='color:skyblue'>2</span>|15|<span style='color:red'>1</span>|
|16|<span style='color:skyblue'>1</span>|17|<span style='color:skyblue'>2</span>|18|<span style='color:red'>3</span>|
|19|<span style='color:skyblue'>3</span>|20|<span style='color:red'>3</span>|21|<span style='color:red'>2</span>|
|22|<span style='color:skyblue'>1</span>|23|<span style='color:skyblue'>2</span>|24|<span style='color:red'>4</span>|
|25|<span style='color:skyblue'>3</span>|26|<span style='color:red'>1</span>|27|<span style='color:skyblue'>4</span>|
|28|<span style='color:skyblue'>1</span>|29|<span style='color:red'>3</span>|30|<span style='color:skyblue'>3</span>|
|31|<span style='color:skyblue'>3</span>|32|<span style='color:skyblue'>3</span>|33|<span style='color:skyblue'>3</span>|
|34|<span style='color:skyblue'>3</span>|35|<span style='color:skyblue'>4</span>|36|<span style='color:skyblue'>1</span>|
|37|<span style='color:skyblue'>1</span>|38|<span style='color:skyblue'>1</span>|39|<span style='color:red'>3</span>|
|40|<span style='color:skyblue'>3</span>|41|<span style='color:skyblue'>3</span>|42|<span style='color:red'>4</span>|
|43|<span style='color:red'>3</span>|44|<span style='color:red'>1</span>|45|<span style='color:red'>3</span>|
|46|<span style='color:skyblue'>1</span>|47|<span style='color:skyblue'>3</span>|48|<span style='color:red'>4</span>|
|49|<span style='color:red'>2</span>|50|<span style='color:skyblue'>1</span>|51|<span style='color:skyblue'>3</span>|
|52|<span style='color:red'>4</span>|53|<span style='color:red'>3</span>|54|<span style='color:red'>3</span>|
|55|<span style='color:skyblue'>4</span>|56|<span style='color:red'>3</span>|57|<span style='color:skyblue'>4</span>|
|58|<span style='color:skyblue'>3</span>|59|<span style='color:skyblue'>4</span>|60|<span style='color:red'>4</span>|
|61|<span style='color:red'>4</span>|62|<span style='color:red'>3</span>|63|<span style='color:red'>4</span>|
|64|<span style='color:red'>4</span>|65|<span style='color:red'>2</span>|66|<span style='color:skyblue'>4</span>|
|67|<span style='color:skyblue'>4</span>|68|<span style='color:red'>3</span>|69|<span style='color:skyblue'>4</span>|
|70|<span style='color:skyblue'>3</span>|71|<span style='color:skyblue'>1</span>|72|<span style='color:red'>1</span>|
|73|<span style='color:skyblue'>4</span>|74|<span style='color:red'>3</span>|75|<span style='color:red'>2</span>|
|76|<span style='color:red'>1</span>|77|<span style='color:skyblue'>1</span>|78|<span style='color:skyblue'>1</span>|
|79|<span style='color:red'>2</span>|80|<span style='color:red'>4</span>|||

### 오답노트 + 관련 개념 정리

1\. 결정계수 = 상관계수의 제곱

2\. 상관계수와 회귀계수의 관계 $\beta _1 = \gamma \frac{s_Y}{s_X}$

3\. 의사결정나무

- 분류 결과가 트리구조 -> 이해가 쉬움
- 훈련 데이터 개수와 노드 선정에 따라 모델이 달라짐
- 수치자료와 범주자료 모두 적용 가능
- 과적합의 위험 있음

6\. 데이터마이닝의 연관 분석 측정 기준: 지지도, 신뢰도, 향상도

7\. 로지스틱 회귀모형 -> 설명 변수가 한 개이고, 회귀계수의 부호가 0보다 작으면 역 S자 그래프가 그려짐

8\. 와드연결법: 군집 내의 오차 제곱 합에 기초하여 군집을 수행

9\. 중심연결법: 두 군집 사이의 거리를 두 군집의 중심 간 거리롤 계산하는 계층적 군집방법

11\. 의사결정나무 분석의 분류 기준 변수 선택 기준

- 카이제곱 통계량의 p값
- 지니 지수
- 엔트로피 지수

15\. 최소제곱법: 회귀분석에서 회귀계수를 추정할 때 사용

18\. 의사결정나무

- 전체 자료를 여러 개의 소집단으로 분류하거나 예측하는 데 사용되는 기법
- 불순도 감소량을 최대한으로 하는 분할을 선택해야 함
- 새로운 데이터를 모형에 적용하기 쉬움
- 수치형과 범주형 변수 모두에 적용 가능

20\. 의사결정나무의 단점

- 연속형 변수를 비연속값으로 범주화하기 때문에 분리 경계점에서 예측의 오류가 커짐
- 각 변수의 고유한 영향력을 해석하기 어려움
- 학습용 데이터의 과적합 위험이 큼 -> 검증용 데이터를 활용하여 교차 타당성 평가를 진행해야
- but, 대용량 데이터에서 생성이 빠르고 정확도가 높은 장점이 있음

21\. 의사결정나무의 가지치기 분리 알고리즘: CHAID, CART, C4.5
<br>SOM은 군집분석에서 사용하는 자기 조직화 지도 알고리즘

24\. 인공신경망

- 사람 두뇌의 뉴런이 전기신호를 전달하는 모습을 모방한 모델
- 입력층, 출력층, 은닉층의 세 가지 층으로 구성
- 역전파 알고리즘을 사용하여 결과값의 오차가 최소가 될 수 있도록 가중치를 계산
- 활성화 함수는 대표적으로 Sigmoid가 있음

26\. Sigmoid 함수: 곡선의 형태, 0~1 값 출력

29\. 퍼셉트론

- 단층 퍼셉트론은 AND, OR만 연산 가능 (XOR 불가)
- 다층 퍼셉트론은 단층 퍼셉트론과 달리 은닉층을 가짐
- 기울기 소실 문제는 sigmoid의 특성에 의해 발생 -> ReLU를 통해 해결 가능
- 인공 신경망 모델은 결과 해석이 어려운 것이 특징

39\. 집단으로 구분하는 것은 군집 분석

42\. 오즈비(Odds Ratio, OR) = 각 집단의 Odds 비율, 집단별로 구할 수 있는 값은 Odds

43\. 해외유입 집단의 Odds = $\frac{\frac{해외유입양성}{해외유입}}{\frac{해외유입음성}{해외유입}}$

44\. 피셔의 정확 검정

- 두 범주형 변수가 서로 독립적인지 연관성이 있는지 검정
- 표본의 수가 작거나 범주가 많아서 빈도수가 극도로 작은 경우 사용

45\. 다차원적도법(MDS)

- 개체들 사이의 관계를 상대적 위치 등 공간적 배열을 해석하는 분석 방법
- 계량적 방법과 비계량적 방법이 있음
- 스트레스 값은 부적합 정도를 나타내는 값으로 좌표를 조정해 최소화함
- 적합도가 좋을수록 스트레스 값은 0에 가까움

48\. 정상 시계열

- 평균이 일정
- 분산이 시점에 의존하지 X
- 공분산은 시차에만 의존, 시점 자체에는 의존하지 X
- 시점에 상관없이 시계열의 특성이 일정

49\. 시계열 분해

- 추세성분: 시계열의 추세가 계속 증가하거나 감소하는 등 특정한 형태를 보이는 경우
- 계절성분: 특정 주기에 따라 특징이 변하는 경우
- 순환성분: 주기가 긴 경우의 변동
- 불규칙성분: 설명할 수 없는 변동

51\. ARIMA(p, d, q) 모형

- 자기상관함수와 부분자기상관함수를 통해 적합한 차수를 식별
- 시계열이 정상성을 만족하는 경우 d가 0인 ARMA(p, q) 모형과 같음
- d는 ARIMA에서 ARMA로 정상화할 때 몇 번 차분했는지를 의미
- p와 d가 모두 0인 경우는 MA(q) 모형
- p만 0인 경우에는 차분을 포함하는 IMA(d, q) 모형

52\. MA(1) 모형: ACF가 시점 2 기준으로 절단된 형태, PACF의 절댓값이 서서히 감소

53\. 변동성 모형

- GARCH가 대표적임
- 불확실성을 설명하는 분산의 움직임에 주목
- 분산이 자기상관이 존재하는 경우 변동성이 큰 구간과 작은 구간이 구분됨
- 주로 경제학 분야에서 리스크를 축정하는 수단으로 사용

54\. $P(B|A) = \frac{P(A\cap B)}{P(A)} = \frac{P(A)\times P(B)}{P(A)}=P(B)$

56\. 나이브 베이즈

- 지도 학습 분류 모델
- 설명변수가 서로 동등하고 독립적이라고 가정
- 산출 속도가 빠름 -> 실시간 분류, 텍스트 분류에 주로 사용
- 종속변수의 각 범주에 속할 확률을 구하고 확률이 큰 범주로 분류

60\. LSTM은 RNN의 주요 모델 중 하나, 장기 의존성 문제를 해결
<br>패딩(Padding)은 CNN에서 특정 맵의 사이즈를 조절하는 방법

61\. 풀링(Pooling)은 합성곱 과정을 거친 데이터 -> 맥스 풀링(Max Pooling): 최댓값을 대푯값으로 산출

62\. 딥러닝 모델의 파라미터 학습에 경사하강법을 사용하는 경우 입력해야 하는 하이퍼파라미터

- 1 epoch는 모든 학습용 데이터가 한번씩 forward pass와 backward pass를 진행함
- 1 iteration은 한 번의 forward pass와 backward pass를 의미
- batch size는 1 iteration을 진행하는 학습용 데이터 샘플의 사이즈
- data size = batch size x iteration
- 1 epoch을 수행하는 iteration = data size / batch size
- learning rate는 파라미터의 업데이트 정도를 조절

63\. 인공신경망(ANN)

- 은닉 노드가 많을 경우 과적합 가능성이 많고 일반화가 어려움
- 레이어 수가 많으면 기울기 소실의 가능성이 높음
- 노드 수가 적으면 과소적합의 가능성이 높음

64\. CNN의 Padding: 이미지 주변에 계산과 무관한 테두리를 추가하여 출력되는 feature map의 사이즈를 조정

65\. 근접중심성: 사회연결망분석(SNA)에서 간접적으로 연결된 모든 노드 간의 거리를 합산하여 중심성을 측정하는 지표

68\. 사회연결망분석(SNA)

- 사회를 구성하는 집단의 수와 규모 알 수 있음
- 영향력 있는 고객을 파악할 수 있음
- 사회 구성원들 간의 관계를 알 수 있음

72\. 배깅: 부트스트랩 샘플링으로 추출한 여러 개의 표본에 모형을 병렬적으로 학습하고 추출된 결과를 집계하는 앙상블 기법

74\. Light GBM: Leaf-wise 방식을 사용하는 트리 기반 알고리즘

- Level-wise 방식: 균형 트리 분할 방식, 최대한 균형 잡힌 트리를 유지하면서 분할하고 이에 따라 깊이가 최소화
- Leaf-wise 방식: 최대 손실을 갖는 리프 노드를 지속 분할하여 깊고 비대칭적인 트리를 생성

75\. 앙상블 모형은 성능을 분산 -> 과적합 방지 -> 실제 데이터에 성능이 좋은 모형을 얻을 수 있음

76\. 부스팅: 이전 모형에서 잘못 분류한 데이터는 높은 가중치를 부여, 다음 모델에서 더 잘 분류하도록 유도

79\. 카이 제곱 검정 - 적합성 검정: 단일 표본에서만 검정 진행

80\. 크루스칼-왈리스 검정: 세 개 이상 집단의 분포를 비교하는 검정 방법

## 과목 마무리 문제

<span style="color:yellow">내용 정리에 없었던 내용</span>
<br><span style="color:orange">다시 확인할 내용</span>
