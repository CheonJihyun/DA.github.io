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
|1|<span style='color:skyblue'>3</span>|2|<span style='color:skyblue'>1</span>|3|<span style='color:skyblue'>4</span>|
|4|<span style='color:red'>3</span> - 정답: 1|5|<span style='color:skyblue'>1</span>|6|<span style='color:skyblue'>2</span>|
|7|<span style='color:skyblue'>4</span>|8|<span style='color:skyblue'>3</span>|9|<span style='color:skyblue'>2</span>|
|10|<span style='color:red'>4</span> - 정답: 2|11|<span style='color:red'>2</span> - 정답: 3|12|<span style='color:skyblue'>3</span>|
|13|<span style='color:skyblue'>4</span>|14|<span style='color:skyblue'>4</span>|15|<span style='color:skyblue'>4</span>|
|16|<span style='color:red'>3</span> - 정답: 2|17|<span style='color:skyblue'>3</span>|18|<span style='color:skyblue'>2</span>|
|19|<span style='color:skyblue'>4</span>|20|<span style='color:skyblue'>1</span>|21|<span style='color:red'>2</span> - 정답: 1|
|22|<span style='color:skyblue'>3</span>|23|<span style='color:skyblue'>1</span>|24|<span style='color:skyblue'>3</span>|
|25|<span style='color:skyblue'>2</span>|26|<span style='color:skyblue'>1</span>|27|<span style='color:skyblue'>4</span>|
|28|<span style='color:red'>2</span> - 정답: 3|29|<span style='color:skyblue'>2</span>|30|<span style='color:skyblue'>1</span>|
|31|<span style='color:red'>2</span> - 정답: 3|32|<span style='color:skyblue'>4</span>|33|<span style='color:skyblue'>4</span>|
|34|<span style='color:skyblue'>3</span>|35|<span style='color:red'>4</span> - 정답: 3|36|<span style='color:red'>2</span> - 정답: 1|
|37|<span style='color:red'>1</span> - 정답: 2|38|<span style='color:skyblue'>3</span>|39|<span style='color:red'>2</span> - 정답: 1|
|40|<span style='color:skyblue'>2</span>|41|<span style='color:skyblue'>4</span>|42|<span style='color:red'>2</span> - 정답: 4|
|43|<span style='color:skyblue'>3</span>|44|<span style='color:skyblue'>1</span>|45|<span style='color:skyblue'>2</span>|
|46|<span style='color:skyblue'>1</span>|47|<span style='color:skyblue'>3</span>|48|<span style='color:red'>4</span> - 정답: 3|
|49|<span style='color:skyblue'>1</span>|50|<span style='color:red'>2</span> - 정답: 1|||

### 오답노트 + 관련 개념 정리

4\. 엔터티 유무형에 따른 분류

- 유형 엔터티: 물리적인 형태가 있고 안정적, 지속적으로 활용되는 엔터티
- 개념 엔터티: 물리적인 형태가 없이 관리해야할 개념적 정보로 구분되는 엔터티
- 사건 엔터티: 업무를 수행함에 따라 발생되는 엔터티

10\. 파생속성: 다른 속성의 속성값을 계산하거나 특정한 규칙으로 변형하여 생성한 속성

11\. GROUP BY + HAVING

16\. START WITH -> CONNECT BY -> PRIOR

21\. IN은 OR이 연결된걸로 생각해야 -> COL1=NULL은 항상 False

28\. 계산 실수

31\. GROUP BY -> COUNT(*): 그룹바이 한 것을 셈

35\. 계산 실수 (AVG 구할 때 0은 합에는 안 들어가지만 개수에는 들어간다)

36\. LEFT OUTER JOIN -> 왼쪽 테이블에 NULL이 생김

37\. (+)가 없는 쪽 테이블이 기준 테이블, 있는 쪽 테이블이 타깃 테이블

39\. CASE 결과가 출력되지 않아도 ORDER BY의 기준이 된다

42\. TCL(Transaction Control Language): COMMIT, ROLLBACK, SAVEPOINT 등

48\. 트랜잭션의 특징

- 원자성: 트랜잭션은 더 이상 분리가 불가능한 업무의 최소단위
- 일관성: 하나의 트랜잭션이 완료된 후에도 데이터베이스는 여전히 일관된 상태여야
- 격리성: 실행 중인 트랜잭션의 중간 결과에 다른 트랜잭션이 접근할 수 없음
- 영속성: 트랜잭션이 성공적으로 실행 완료되면 그 결과는 데이터베이스에 영속적으로 저장

50\. %는 문자가 없어도 됨

## CHAPTER 3 기출변형 모의고사 3회

### 문제풀이

|문제|답|문제|답|문제|답|
|:--:|--|:--:|--|:--:|--|
|1|<span style='color:red'>4</span> - 정답: 3|2|<span style='color:skyblue'>4</span>|3|<span style='color:skyblue'>1</span>|
|4|<span style='color:skyblue'>1</span>|5|<span style='color:skyblue'>3</span>|6|<span style='color:skyblue'>2</span>|
|7|<span style='color:skyblue'>2</span>|8|<span style='color:red'>2</span> - 정답: 4|9|<span style='color:red'>4</span> - 정답: 1|
|10|<span style='color:skyblue'>4</span>|11|<span style='color:red'>4</span> - 정답: 3|12|<span style='color:skyblue'>1</span>|
|13|<span style='color:skyblue'>4</span>|14|<span style='color:skyblue'>3</span>|15|<span style='color:skyblue'>2</span>|
|16|<span style='color:red'>1</span> - 정답: 4|17|<span style='color:skyblue'>1</span>|18|<span style='color:red'>4</span> - 정답: 3|
|19|<span style='color:skyblue'>3</span>|20|<span style='color:skyblue'>1</span>|21|<span style='color:skyblue'>2</span>|
|22|<span style='color:skyblue'>4</span>|23|<span style='color:skyblue'>4</span>|24|<span style='color:skyblue'>3</span>|
|25|<span style='color:skyblue'>1</span>|26|<span style='color:skyblue'>2</span>|27|<span style='color:red'>4</span> - 정답: 2|
|28|<span style='color:skyblue'>3</span>|29|<span style='color:skyblue'>1</span>|30|<span style='color:skyblue'>4</span>|
|31|<span style='color:red'>3</span> - 정답: 1|32|<span style='color:skyblue'>3</span>|33|<span style='color:skyblue'>4</span>|
|34|<span style='color:skyblue'>4</span>|35|<span style='color:skyblue'>4</span>|36|<span style='color:red'>1</span> - 정답: 2|
|37|<span style='color:red'>2</span> - 정답: 3|38|<span style='color:skyblue'>2</span>|39|<span style='color:skyblue'>3</span>|
|40|<span style='color:skyblue'>2</span>|41|<span style='color:red'>3</span> - 정답: 4|42|<span style='color:skyblue'>2</span>|
|43|<span style='color:skyblue'>2</span>|44|<span style='color:skyblue'>4</span>|45|<span style='color:red'>2</span> - 정답: 4|
|46|<span style='color:skyblue'>1</span>|47|<span style='color:skyblue'>2</span>|48|<span style='color:skyblue'>4</span>|
|49|<span style='color:skyblue'>1</span>|50|<span style='color:red'>1</span> - 정답: 3|||

### 오답노트 + 관련 개념 정리

1\. 데이터베이스 모델리의 특징: 추상화, 단순화, 명확화

8\. 컬럼 반정규화 기법: 중복 컬럼 추가, 파생 컬럼 추가, 이력테이블 컬럼 추가, PK에 의한 컬럼 추가, 응용시스템 오작동을 위한 컬럼 추가

9\. 속성은 의미상 더 분리될 수 없음
<br>속성은 특성에 따라 기본속성, 설계속성, 파생속성으로 나눌 수 있음

11\. NVL2(인수1, 인수2, 인수3): 인수1이 NULL이 아니면 인수2 반환, NULL이면 인수3 반환

16\. SQL 명령어 구분

- DDL(Data Definition Language): CREATE, ALTER, RENAME, DROP, TRUNCATE
- DML(Data Manipulation Language): SELECT, INSERT, UPDATE, DELETE
- DCL(Data Control Language): GRANT, REVOKE
- TCL(Transaction Control Language): COMMIT, ROLLBACK, SAVEPOINT

18\. CROSS JOIN은 별도의 ON 절이 없음

27\. TRUNC(): 버림

29\. <span style="color:orange">3번 보기에서 RANK 함수 마지막이 9위 2개면 10위 없을수도 있는거 아님..?</span>

31\. 문자형과 숫자형을 비교할 경우 문자형 데이터를 묵시적으로 변환하여 비교
<br>연산자 실행 순서: 괄호 -> 비교연산자 -> NOT -> AND -> OR

36\. CROSS JOIN: 집합 연산자의 PRODUCT 개념, JOIN 조건이 없는 경우 생길 수 있는 모든 데이터의 조합을 출력

37\. LTRIM(A, B): 가장 왼쪽의 문자가 B의 구성 문자 중 하나일 때 해당 문자를 지운 후 데이터를 반환
<br>LPAD(): 왼쪽부터 특정 문자로 자릿수를 채움

41\. TCL(Transaction Control Language): COMMIT, ROLLBACK, SAVEPOINT

45\. 개념스키마

- 모든 사용자 관점을 통합한 조직 전체 관점의 통합적 표현
- 모든 응용시스템이나 사용자들이 필요로 하는 데이터를 통합한 조직 전체의 DB를 기술한 것
- DB에 저장되는 데이터와 그들간의 관계를 표현하는 스키마

50\. CUME_DIST: 해당 파티션에서의 누적 백분율을 구하는 함수 (0~1)

## CHAPTER 4 기출변형 모의고사 4회

### 문제풀이

|문제|답|문제|답|문제|답|
|:--:|--|:--:|--|:--:|--|
|1|<span style='color:red'>4</span> - 정답: 2|2|<span style='color:red'>4</span> - 정답: 1|3|<span style='color:skyblue'>3</span>|
|4|<span style='color:skyblue'>3</span>|5|<span style='color:skyblue'>4</span>|6|<span style='color:skyblue'>1</span>|
|7|<span style='color:red'>2</span> - 정답: 3|8|<span style='color:skyblue'>3</span>|9|<span style='color:red'>3</span> - 정답: 2|
|10|<span style='color:red'>3</span> - 정답: 2|11|<span style='color:skyblue'>1</span>|12|<span style='color:red'>3</span> - 정답: 4|
|13|<span style='color:skyblue'>2</span>|14|<span style='color:skyblue'>3</span>|15|<span style='color:red'>3</span> - 정답: 2|
|16|<span style='color:skyblue'>1</span>|17|<span style='color:skyblue'>2</span>|18|<span style='color:skyblue'>4</span>|
|19|<span style='color:skyblue'>3</span>|20|<span style='color:red'>1</span> - 정답: 4|21|<span style='color:skyblue'>2</span>|
|22|<span style='color:skyblue'>3</span>|23|<span style='color:red'>2</span> - 정답: 1|24|<span style='color:red'>1</span> - 정답: 3|
|25|<span style='color:red'>3</span> - 정답: 1|26|<span style='color:skyblue'>2</span>|27|<span style='color:red'>3</span> - 정답: 4|
|28|<span style='color:skyblue'>3</span>|29|<span style='color:skyblue'>2</span>|30|<span style='color:skyblue'>1</span>|
|31|<span style='color:skyblue'>3</span>|32|<span style='color:red'>2</span> - 정답: 4|33|<span style='color:red'>3</span> - 정답: 2|
|34|<span style='color:skyblue'>4</span>|35|<span style='color:skyblue'>3</span>|36|<span style='color:red'>4</span> - 정답: 3|
|37|<span style='color:skyblue'>4</span>|38|<span style='color:red'>3</span> - 정답: 1|39|<span style='color:skyblue'>2</span>|
|40|<span style='color:red'>4</span> - 정답: 2|41|<span style='color:skyblue'>3</span>|42|<span style='color:skyblue'>3</span>|
|43|<span style='color:skyblue'>4</span>|44|<span style='color:skyblue'>2</span>|45|<span style='color:skyblue'>1</span>|
|46|<span style='color:red'>3</span> - 정답: 2|47|<span style='color:skyblue'>3</span>|48|<span style='color:skyblue'>2</span>|
|49|<span style='color:skyblue'>4</span>|50|<span style='color:skyblue'>1</span>|||

### 오답노트 + 관련 개념 정리

1\. 내부 스키마: DB가 물리적으로 저장된 형식, 물리적 장치에서 데이터가 실제로 저장되는 방법
<br>물리적 데이터 모델링: 실제로 데이터베이스 구축할 때 참고되는 모델

2\. 도메인: 각 속성이 가질 수 있는 값의 범위, 엔터티 내의 속성에 대한 데이터 타입, 사이즈, 제약사항 등을 지정
<br>제약조건: 데이터의 무결성을 유지하기 위해 테이블의 특정 컬럼에 설정하는 제약(PK, FK, NOT NULL 등)

7\. 기본속성: 처음부터 주어진 속성 (i.e. 할인율)
<br>파생속성: 계산되어진 속성 (i.e. 할인가)

9\. 이상현상

- 삽입이상: 데이터 삽입 시 의도했던 데이터 외에 다른 값들도 삽입됨
- 갱신이상: 속성값 변경 시 일부 레코드만 변경되어 일관성이 깨짐
- 삭제이상: 데이터 삭제 시 의도했던 데이터 외에 다른 값들도 연쇄 삭제됨

10\. 데이터 모델링의 3단계

- 개념적 데이터 모델링: 업무중심적, 포괄적인 수준의 모델링
- 논리적 데이터 모델링: 데이터 모델링의 최종 완료 상태
- 물리적 데이터 모델링: 실제로 데이터베이스에 반영할 수 있도록 물리적 성격을 고려하여 설계

12\. NVL2(인수1, 인수2, 인수3): 인수1이 NULL이 아닌 경우 인수2를 출력, NULL인 경우 인수3을 출력

15\. ORDER BY 내부의 서브쿼리는 정렬 순서에만 영향을 미칠 뿐, 출력되는 결과와는 무관

20\. RANGE BETWEEN UNBOUNDED PRECEDING AND UNBOUNDED PRECEDING은 사용 불가한 데이터의 범위

23\. SUM 함수는 계산 시 NULL 값을 제외, 사칙연산은 NULL 존재시 결과가 NULL

24\. 결과 나온 그대로 답변 고르면 됨...

25\. DISTINCT COL1, COL2는 COL1, COL2 쌍의 DISTINCT 값을 구하는 것 (각각을 보는게 아님)

27\. FROM에 테이블 두 개, WHERE에 <>이 있으면 NON-EQUI JOIN -> 같지 않은 데이터끼리 연결

32\. LAG 함수: 파티션별 윈도우에서 위로 몇 번째 행의 값을 출력
<br>LEAD 함수: 파티션별 윈도우에서 아래로 몇 번째 행의 값을 출력

33\. EXTRACT ('YEAR'|'MONTH'|'DAY' FROM X): 날짜 데이터에서 연|월|일 데이터를 출력
<br>LPAD(데이터, 총 문자 길이, 채움문자): 지정한 총 문자 길이보다 데이터가 짧을 경우 채움문자로 빈 공간을 왼쪽에 채움

36\. 트랜잭션의 특징: 원자성, 일관성, 격리성, 영속성

38\. ~ - NULL = NULL (NULL과의 연산 결과는 항상 NULL)

40\. 숫자 BETWEEN A AND B = A와 B 사이에 숫자가 있다 = A<=숫자 & B>=숫자

46\. WHERE절은 START WITH -> CONNECT BY 다음에 적용



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