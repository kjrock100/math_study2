# 0.2.4 Sequences 분석

이 문서는 이산 구조에서 데이터를 순서대로 나열하는 **수열(Sequences)**에 대해 다루는 **0.2.4 Sequences** 섹션을 분석하고 설명합니다. 수열은 알고리즘의 반복 과정이나 데이터 스트림을 모델링하는 데 필수적인 개념입니다.

## 수열의 정의 (Definition of Sequences)

* **정의:** 수열은 순서가 있는 객체들의 목록입니다. 수학적으로는 정수 집합(주로 $\mathbb{N}$ 또는 $\mathbb{Z}^+$)의 부분집합에서 집합 $S$로의 **함수**로 정의됩니다.
* **표기:** 수열 $\{a_n\}$은 $a_1, a_2, a_3, \dots$ 와 같이 각 항(term)을 나열하여 표현합니다.
* **항(Term):** $a_n$은 수열의 $n$번째 항을 의미합니다.

## 주요 수열의 종류 (Types of Sequences)

### 1. 등비수열 (Geometric Progression)

* **정의:** 각 항이 바로 앞의 항에 일정한 수(공비)를 곱하여 얻어지는 수열입니다.
* **형태:** $a, ar, ar^2, \dots, ar^n, \dots$
  * $a$: 첫째항 (Initial term)
  * $r$: 공비 (Common ratio)
* **예시:** $a=2, r=3$ 일 때, $2, 6, 18, 54, \dots$

### 2. 등차수열 (Arithmetic Progression)

* **정의:** 각 항이 바로 앞의 항에 일정한 수(공차)를 더하여 얻어지는 수열입니다.
* **형태:** $a, a+d, a+2d, \dots, a+nd, \dots$
  * $a$: 첫째항 (Initial term)
  * $d$: 공차 (Common difference)
* **예시:** $a=-1, d=4$ 일 때, $-1, 3, 7, 11, \dots$

## 점화식 (Recurrence Relations)

* **정의:** 수열의 $n$번째 항 $a_n$을 그 이전의 항들($a_{n-1}, a_{n-2}, \dots$)에 대한 식으로 표현하는 방법입니다.
* **초기 조건 (Initial Conditions):** 점화식만으로는 수열이 유일하게 결정되지 않으므로, 수열의 시작 값들이 필요합니다.
* **예시 (피보나치 수열):**
  * 점화식: $f_n = f_{n-1} + f_{n-2}$
  * 초기 조건: $f_0 = 0, f_1 = 1$
  * 수열: $0, 1, 1, 2, 3, 5, 8, \dots$

## 합 (Summations)

수열의 항들을 더하는 것을 간결하게 표현하기 위해 시그마($\sum$) 표기법을 사용합니다.

* **표기:** $\sum_{i=m}^{n} a_i = a_m + a_{m+1} + \dots + a_n$
  * $i$: 인덱스 변수 (Index of summation)
  * $m$: 하한 (Lower limit)
  * $n$: 상한 (Upper limit)

### 유용한 합 공식 (Useful Summation Formulae)

1. **등비수열의 합:** $\sum_{j=0}^{n} ar^j = \begin{cases} \frac{a(r^{n+1}-1)}{r-1} & \text{if } r \neq 1 \\ (n+1)a & \text{if } r = 1 \end{cases}$
2. **자연수의 합:** $\sum_{i=1}^{n} i = \frac{n(n+1)}{2}$

## 컴퓨터 과학에서의 응용

1. **배열과 리스트:** 수열은 컴퓨터 메모리에 저장되는 배열(Array)이나 리스트(List) 자료구조의 수학적 모델입니다.
2. **알고리즘 분석:** 반복문(Loop)의 실행 횟수나 알고리즘의 시간 복잡도를 계산할 때 수열의 합 공식을 사용합니다.
3. **재귀 함수:** 점화식은 프로그래밍의 재귀 함수(Recursive Function)와 직접적으로 대응됩니다.

## 요약

**0.2.4 Sequences**에서는 데이터를 순서대로 나열하는 규칙과 이를 수학적으로 표현하는 방법을 배웁니다. 특히 등비수열과 등차수열은 알고리즘의 효율성을 분석하는 기초가 되며, 점화식은 동적 계획법(Dynamic Programming)과 같은 고급 알고리즘 설계의 핵심 원리입니다.
