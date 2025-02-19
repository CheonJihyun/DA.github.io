# PART 3 기출변형 모의고사

## CHAPTER 1 기출변형 모의고사 1회

### 문제풀이

|문제|답|문제|답|문제|답|
|:--:|--|:--:|--|:--:|--|
|1|<span style='color:skyblue'>③</span>|2|<span style='color:skyblue'>②</span>|3|<span style='color:red'>②</span> - 정답: ④|
|4|<span style='color:skyblue'>①</span>|5|<span style='color:skyblue'>①</span>|6|<span style='color:red'>②</span> - 정답: ③|
|7|<span style='color:red'>③</span> - 정답: ②|8|<span style='color:red'>③</span> - 정답: ④|9|<span style='color:skyblue'>③</span>|
|10|<span style='color:red'>①</span> - 정답: ②|11|<span style='color:red'>②</span> - 정답: ①|12|<span style='color:skyblue'>④</span>
|13|<span style='color:skyblue'>③</span>|14|<span style='color:skyblue'>③</span>|15|<span style='color:red'>③</span> - 정답: ④|
|16|<span style='color:skyblue'>④</span>|17|<span style='color:skyblue'>①</span>|18|<span style='color:skyblue'>①</span>|
|19|<span style='color:red'>④</span> - 정답: ③|20|<span style='color:red'>①</span> - 정답: ②|21|<span style='color:skyblue'>①</span>
|22|<span style='color:skyblue'>③</span>|23|<span style='color:skyblue'>②</span>|24|<span style='color:skyblue'>④</span>|
|25|<span style='color:skyblue'>②</span>|26|<span style='color:red'>①</span> - 정답: ④|27|<span style='color:skyblue'>①</span>|
|28|<span style='color:skyblue'>③</span>|29|<span style='color:skyblue'>①</span>|30|<span style='color:red'>②</span> - 정답: ③|
|31|<span style='color:skyblue'>②</span>|32|<span style='color:red'>③</span> - 정답: ④|33|<span style='color:skyblue'>③</span>|
|34|<span style='color:skyblue'>①</span>|35|<span style='color:skyblue'>②</span>|36|4|
|37|<span style='color:red'>②</span> - 정답: ①|38|<span style='color:skyblue'>③</span>|39|<span style='color:skyblue'>④</span>|
|40|<span style='color:red'>③</span> - 정답: ④|41|<span style='color:skyblue'>①</span>|42|<span style='color:skyblue'>②</span>|
|43|<span style='color:skyblue'>③</span>|44|<span style='color:red'>③</span> - 정답: ④|45|<span style='color:skyblue'>①</span>|
|46|<span style='color:skyblue'>④</span>|47|<span style='color:red'>①</span> - 정답: ②|48|<span style='color:skyblue'>①</span>|
|49|<span style='color:skyblue'>③</span>|50|<span style='color:skyblue'>②</span>|||

### 오답노트 + 관련 개념 정리

1\. 데이터 모델링의 3단계: 개념적 데이터 모델링 -> 논히적 데이터 모델링 -> 물리적 데이터 모델링

3\. 데이터베이스의 3단계 구조: 외부 단계 -> 개념 단계 -> 내부 단계

6\. 제2정규화: 일반속성이 주식별자의 일부에만 종속될 때
<br>제3정규화: 기본키를 제외한 일반속성 간에 종속성이 발생할 때

8\. 주식별자의 특장: 유일성, 최소성, 붊변성, 존재성

10\. 비식별 관계: 점선으로 표현

11\. <span style="color:orange">계층형 쿼리: 부모, 자식간의 수직관계를 트리 구조 형태로 보여주는 쿼리</span>
<br>START WITH: 트리 구조의 최상위 행을 지정
<br>CONNECT BY: 부모, 자식의 관계를 지정
<br>PRIOR: CONNECT BY 절에 사용되며, PRIOR에 지정된 컬럼이 맞은편 컬럼을 찾아감
<br>CONNECT BY PRIOR 자식 컬럼 = 부모 컬럼: 부모 → 자식 순방향 전개
<br>CONNECT BY PRIOR 부모 컬럼 = 자식 컬럼: 자식 → 부모 역방향 전개
<br>ORDER SIBLINGS: 계층형 쿼리에서 정렬을 수행

15\. DDL(Data Definition Language): 데이터를 정의하는 명령어(CREATE, ALTER, DROP, RENAME, TRUNCATE 등)

18\. MINUS는 중복을 제거

19\. RATIO_TO_REPORT: 파티션 내의 비율을 반환, 0~1 사이의 값을 리턴

20\. CONNECT_BY_ISLEAF: 해당 데이터가 리프 데이터면 1, 그렇지 않으면 0을 반환

22\. DISTINCT를 사용하면 중복된 부서번호는 하나만 나옴
<br>MINUS: 중복 자동 제거
<br>EXISTS: 특정 조건을 만족하는 데이터가 존재하는지 확인하는 명령어
<br>SELECT 1, SELECT 2 → 존재여부 확인
<br>GROUP BY: 부서별로 중복 제거되어 한번 씩만 나옴

26\. CROSS JOIN: 테이블 간 생길 수 있는 모든 데이터의 조합을 반환 (M*N 건의 결과 나옴)

30\. ROUND(N, -2) -> 백의 자리까지 반환

32\. COL1 <> NULL은 항상 False, NOT IN은 조건끼리의 AND

35\. CHECK 제약조건은 입력할 수 있는 값의 범위 등을 제한

37\. NULL은 반드시 IS NULL /  IS NOT NULL로 비교되어야

40\. GROUPING SETS(A, (A, B)): A로 그룹핑 + A, B로 그룹핑

44\. COUNT(상수), COUNT(*): NULL 상관 없이 모든 행의 수 출력

47\. AND 연산자가 OR 연산자보다 우선순위가 높음

## CHAPTER 2 기출변형 모의고사 2회

### 문제풀이

|문제|답|문제|답|문제|답|
|:--:|--|:--:|--|:--:|--|
|1|<span style='color:skyblue'></span>|2|<span style='color:skyblue'></span>|3|<span style='color:skyblue'></span>|
|4|<span style='color:skyblue'></span>|5|<span style='color:skyblue'></span>|6|<span style='color:skyblue'></span>|
|7|<span style='color:skyblue'></span>|8|<span style='color:skyblue'></span>|9|<span style='color:skyblue'></span>|
|10|<span style='color:skyblue'></span>|11|<span style='color:skyblue'></span>|12|<span style='color:skyblue'></span>|
|13|<span style='color:skyblue'></span>|14|<span style='color:skyblue'></span>|15|<span style='color:skyblue'></span>|
|16|<span style='color:skyblue'></span>|17|<span style='color:skyblue'></span>|18|<span style='color:skyblue'></span>|
|19|<span style='color:skyblue'></span>|20|<span style='color:skyblue'></span>|21|<span style='color:skyblue'></span>|
|22|<span style='color:skyblue'></span>|23|<span style='color:skyblue'></span>|24|<span style='color:skyblue'></span>|
|25|<span style='color:skyblue'></span>|26|<span style='color:skyblue'></span>|27|<span style='color:skyblue'></span>|
|28|<span style='color:skyblue'></span>|29|<span style='color:skyblue'></span>|30|<span style='color:skyblue'></span>|
|31|<span style='color:skyblue'></span>|32|<span style='color:skyblue'></span>|33|<span style='color:skyblue'></span>|
|34|<span style='color:skyblue'></span>|35|<span style='color:skyblue'></span>|36|<span style='color:skyblue'></span>|
|37|<span style='color:skyblue'></span>|38|<span style='color:skyblue'></span>|39|<span style='color:skyblue'></span>|
|40|<span style='color:skyblue'></span>|41|<span style='color:skyblue'></span>|42|<span style='color:skyblue'></span>|
|43|<span style='color:skyblue'></span>|44|<span style='color:skyblue'></span>|45|<span style='color:skyblue'></span>|
|46|<span style='color:skyblue'></span>|47|<span style='color:skyblue'></span>|48|<span style='color:skyblue'></span>|
|49|<span style='color:skyblue'></span>|50|<span style='color:skyblue'></span>|||

### 오답노트 + 관련 개념 정리

## CHAPTER 3 기출변형 모의고사 3회

### 문제풀이

|문제|답|문제|답|문제|답|
|:--:|--|:--:|--|:--:|--|
|1|<span style='color:skyblue'></span>|2|<span style='color:skyblue'></span>|3|<span style='color:skyblue'></span>|
|4|<span style='color:skyblue'></span>|5|<span style='color:skyblue'></span>|6|<span style='color:skyblue'></span>|
|7|<span style='color:skyblue'></span>|8|<span style='color:skyblue'></span>|9|<span style='color:skyblue'></span>|
|10|<span style='color:skyblue'></span>|11|<span style='color:skyblue'></span>|12|<span style='color:skyblue'></span>|
|13|<span style='color:skyblue'></span>|14|<span style='color:skyblue'></span>|15|<span style='color:skyblue'></span>|
|16|<span style='color:skyblue'></span>|17|<span style='color:skyblue'></span>|18|<span style='color:skyblue'></span>|
|19|<span style='color:skyblue'></span>|20|<span style='color:skyblue'></span>|21|<span style='color:skyblue'></span>|
|22|<span style='color:skyblue'></span>|23|<span style='color:skyblue'></span>|24|<span style='color:skyblue'></span>|
|25|<span style='color:skyblue'></span>|26|<span style='color:skyblue'></span>|27|<span style='color:skyblue'></span>|
|28|<span style='color:skyblue'></span>|29|<span style='color:skyblue'></span>|30|<span style='color:skyblue'></span>|
|31|<span style='color:skyblue'></span>|32|<span style='color:skyblue'></span>|33|<span style='color:skyblue'></span>|
|34|<span style='color:skyblue'></span>|35|<span style='color:skyblue'></span>|36|<span style='color:skyblue'></span>|
|37|<span style='color:skyblue'></span>|38|<span style='color:skyblue'></span>|39|<span style='color:skyblue'></span>|
|40|<span style='color:skyblue'></span>|41|<span style='color:skyblue'></span>|42|<span style='color:skyblue'></span>|
|43|<span style='color:skyblue'></span>|44|<span style='color:skyblue'></span>|45|<span style='color:skyblue'></span>|
|46|<span style='color:skyblue'></span>|47|<span style='color:skyblue'></span>|48|<span style='color:skyblue'></span>|
|49|<span style='color:skyblue'></span>|50|<span style='color:skyblue'></span>|||

### 오답노트 + 관련 개념 정리

## CHAPTER 4 기출변형 모의고사 4회

### 문제풀이

|문제|답|문제|답|문제|답|
|:--:|--|:--:|--|:--:|--|
|1|<span style='color:skyblue'></span>|2|<span style='color:skyblue'></span>|3|<span style='color:skyblue'></span>|
|4|<span style='color:skyblue'></span>|5|<span style='color:skyblue'></span>|6|<span style='color:skyblue'></span>|
|7|<span style='color:skyblue'></span>|8|<span style='color:skyblue'></span>|9|<span style='color:skyblue'></span>|
|10|<span style='color:skyblue'></span>|11|<span style='color:skyblue'></span>|12|<span style='color:skyblue'></span>|
|13|<span style='color:skyblue'></span>|14|<span style='color:skyblue'></span>|15|<span style='color:skyblue'></span>|
|16|<span style='color:skyblue'></span>|17|<span style='color:skyblue'></span>|18|<span style='color:skyblue'></span>|
|19|<span style='color:skyblue'></span>|20|<span style='color:skyblue'></span>|21|<span style='color:skyblue'></span>|
|22|<span style='color:skyblue'></span>|23|<span style='color:skyblue'></span>|24|<span style='color:skyblue'></span>|
|25|<span style='color:skyblue'></span>|26|<span style='color:skyblue'></span>|27|<span style='color:skyblue'></span>|
|28|<span style='color:skyblue'></span>|29|<span style='color:skyblue'></span>|30|<span style='color:skyblue'></span>|
|31|<span style='color:skyblue'></span>|32|<span style='color:skyblue'></span>|33|<span style='color:skyblue'></span>|
|34|<span style='color:skyblue'></span>|35|<span style='color:skyblue'></span>|36|<span style='color:skyblue'></span>|
|37|<span style='color:skyblue'></span>|38|<span style='color:skyblue'></span>|39|<span style='color:skyblue'></span>|
|40|<span style='color:skyblue'></span>|41|<span style='color:skyblue'></span>|42|<span style='color:skyblue'></span>|
|43|<span style='color:skyblue'></span>|44|<span style='color:skyblue'></span>|45|<span style='color:skyblue'></span>|
|46|<span style='color:skyblue'></span>|47|<span style='color:skyblue'></span>|48|<span style='color:skyblue'></span>|
|49|<span style='color:skyblue'></span>|50|<span style='color:skyblue'></span>|||

### 오답노트 + 관련 개념 정리

## CHAPTER 5 기출변형 모의고사 5회

### 문제풀이

|문제|답|문제|답|문제|답|
|:--:|--|:--:|--|:--:|--|
|1|<span style='color:skyblue'></span>|2|<span style='color:skyblue'></span>|3|<span style='color:skyblue'></span>|
|4|<span style='color:skyblue'></span>|5|<span style='color:skyblue'></span>|6|<span style='color:skyblue'></span>|
|7|<span style='color:skyblue'></span>|8|<span style='color:skyblue'></span>|9|<span style='color:skyblue'></span>|
|10|<span style='color:skyblue'></span>|11|<span style='color:skyblue'></span>|12|<span style='color:skyblue'></span>|
|13|<span style='color:skyblue'></span>|14|<span style='color:skyblue'></span>|15|<span style='color:skyblue'></span>|
|16|<span style='color:skyblue'></span>|17|<span style='color:skyblue'></span>|18|<span style='color:skyblue'></span>|
|19|<span style='color:skyblue'></span>|20|<span style='color:skyblue'></span>|21|<span style='color:skyblue'></span>|
|22|<span style='color:skyblue'></span>|23|<span style='color:skyblue'></span>|24|<span style='color:skyblue'></span>|
|25|<span style='color:skyblue'></span>|26|<span style='color:skyblue'></span>|27|<span style='color:skyblue'></span>|
|28|<span style='color:skyblue'></span>|29|<span style='color:skyblue'></span>|30|<span style='color:skyblue'></span>|
|31|<span style='color:skyblue'></span>|32|<span style='color:skyblue'></span>|33|<span style='color:skyblue'></span>|
|34|<span style='color:skyblue'></span>|35|<span style='color:skyblue'></span>|36|<span style='color:skyblue'></span>|
|37|<span style='color:skyblue'></span>|38|<span style='color:skyblue'></span>|39|<span style='color:skyblue'></span>|
|40|<span style='color:skyblue'></span>|41|<span style='color:skyblue'></span>|42|<span style='color:skyblue'></span>|
|43|<span style='color:skyblue'></span>|44|<span style='color:skyblue'></span>|45|<span style='color:skyblue'></span>|
|46|<span style='color:skyblue'></span>|47|<span style='color:skyblue'></span>|48|<span style='color:skyblue'></span>|
|49|<span style='color:skyblue'></span>|50|<span style='color:skyblue'></span>|||

### 오답노트 + 관련 개념 정리