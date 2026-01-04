# 0.2.2 Sets 분석

이 문서는 이산 수학의 가장 기본이 되는 구조인 **집합(Sets)**에 대해 다루는 **0.2.2 Sets** 섹션을 분석하고 설명합니다. 집합론은 현대 수학의 기초 언어이며, 컴퓨터 과학에서도 데이터를 그룹화하고 처리하는 데 필수적인 개념입니다.

## 집합의 정의 (Definition of Sets)

* **정의:** 집합(Set)은 서로 구별되는 객체(Object)들의 모임입니다.
* **원소(Element):** 집합을 구성하는 객체들을 원소 또는 멤버라고 합니다.
* **표기법:**
  * $a \in A$: $a$는 집합 $A$의 원소이다.
  * $a \notin A$: $a$는 집합 $A$의 원소가 아니다.

## 집합을 표현하는 방법

1. **원소 나열법 (Roster Method):** 중괄호 `{}` 안에 원소들을 나열하는 방법입니다.
    * 예: $V = \{a, e, i, o, u\}$
    * *주의:* 순서는 중요하지 않으며, 중복된 원소는 하나로 취급합니다. $\{1, 2, 3\} = \{3, 1, 2\} = \{1, 2, 2, 3\}$

2. **조건 제시법 (Set-Builder Notation):** 원소들이 만족해야 하는 조건을 명시하는 방법입니다.
    * 형식: $S = \{x \mid P(x)\}$ (여기서 $P(x)$는 조건)
    * 예: $O = \{x \mid x \text{ is an odd positive integer less than } 10\}$

## 중요한 수 집합 (Important Number Sets)

이산 수학에서 자주 사용되는 표준 기호들입니다.

* $\mathbb{N} = \{0, 1, 2, 3, \dots\}$: 자연수 (Natural Numbers)
* $\mathbb{Z} = \{\dots, -2, -1, 0, 1, 2, \dots\}$: 정수 (Integers)
* $\mathbb{Z}^+ = \{1, 2, 3, \dots\}$: 양의 정수 (Positive Integers)
* $\mathbb{Q} = \{p/q \mid p \in \mathbb{Z}, q \in \mathbb{Z}, q \neq 0\}$: 유리수 (Rational Numbers)
* $\mathbb{R}$: 실수 (Real Numbers)
* $\mathbb{C}$: 복소수 (Complex Numbers)

## 부분집합 (Subsets)

* **정의:** 집합 $A$의 모든 원소가 집합 $B$에 포함될 때, $A$는 $B$의 부분집합이라고 하며 $A \subseteq B$로 표기합니다.
  * $\forall x (x \in A \rightarrow x \in B)$
* **진부분집합 (Proper Subset):** $A \subseteq B$이고 $A \neq B$일 때, $A \subset B$로 표기합니다.
* **성질:**
  * 모든 집합 $S$에 대해, $\emptyset \subseteq S$ (공집합은 모든 집합의 부분집합)
  * 모든 집합 $S$에 대해, $S \subseteq S$ (자기 자신은 부분집합)

## 집합의 크기 (Cardinality)

* **정의:** 서로 다른 원소의 개수입니다. $|S|$로 표기합니다.
* **유한 집합 (Finite Set):** 원소의 개수가 유한한 집합.
  * 예: $A = \{1, 3, 5\}$이면 $|A| = 3$.
* **무한 집합 (Infinite Set):** 원소의 개수가 무한한 집합 (예: $\mathbb{Z}$).

## 멱집합 (Power Sets)

* **정의:** 집합 $S$의 모든 부분집합을 원소로 가지는 집합입니다. $\mathcal{P}(S)$로 표기합니다.
* **크기:** $|S| = n$이면, $|\mathcal{P}(S)| = 2^n$입니다.
* **예시:** $S = \{0, 1\}$일 때, $\mathcal{P}(S) = \{\emptyset, \{0\}, \{1\}, \{0, 1\}\}$.

## 곱집합 (Cartesian Products)

* **정의:** 두 집합 $A$와 $B$에 대해, 첫 번째 성분은 $A$에서, 두 번째 성분은 $B$에서 가져온 순서쌍(Ordered Pair)들의 집합입니다.
* **표기:** $A \times B = \{(a, b) \mid a \in A \land b \in B\}$
* **응용:** 데이터베이스의 테이블(Relation)은 속성들의 도메인에 대한 부분집합으로 볼 수 있습니다.

## 요약

**0.2.2 Sets**에서는 수학적 논의의 대상을 명확히 정의하는 방법을 배웁니다. 집합은 앞으로 배울 함수, 관계, 그래프, 확률 등 모든 이산 구조의 기초가 되므로, 표기법과 기본 성질(부분집합, 멱집합 등)을 숙지하는 것이 중요합니다.
