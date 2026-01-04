# 5. Discrete Structures Revisited 분석

이 문서는 **5. Discrete Structures Revisited** 장의 내용을 분석하고 설명합니다. 이 장은 0장에서 간략히 소개되었던 이산 수학의 핵심 구조인 **집합(Sets)**과 **함수(Functions)**를 다시 다루며, 앞서 배운 논리와 증명 기술을 적용하여 더 깊이 있고 엄밀하게 탐구합니다.

## 1. 장의 개요 (Chapter Overview)

이산 수학의 많은 주제들은 집합과 함수라는 언어로 기술됩니다. 0장에서는 직관적인 정의를 다루었다면, 5장에서는 엄밀한 수학적 정의와 표기법을 확립하고, 집합 간의 관계나 함수의 성질을 증명하는 데 초점을 맞춥니다. 이는 추상 대수학, 해석학 등 더 높은 수준의 수학으로 나아가는 기초가 됩니다.

## 2. 집합 (Sets) - 5.1절

집합론은 현대 수학의 기초 언어입니다.

### 2.1 표기법과 정의 (Notation)

* **원소 나열법(Roster Method):** $A = \{1, 2, 3\}$
* **조건 제시법(Set-Builder Notation):** $A = \{x \in \mathbb{Z} : x > 0\}$
* **특수 집합:** $\emptyset$ (공집합), $\mathcal{P}(A)$ (멱집합 - 집합 $A$의 모든 부분집합의 집합).

### 2.2 집합 간의 관계 (Relationships)

* **부분집합(Subset):** $A \subseteq B \iff \forall x (x \in A \to x \in B)$.
* **상등(Equality):** $A = B \iff A \subseteq B \land B \subseteq A$.

### 2.3 연산 (Operations)

* **합집합(Union):** $A \cup B$
* **교집합(Intersection):** $A \cap B$
* **차집합(Difference):** $A \setminus B$
* **여집합(Complement):** $\bar{A}$
* **곱집합(Cartesian Product):** $A \times B = \{(a, b) : a \in A, b \in B\}$

### 2.4 벤 다이어그램 (Venn Diagrams)

집합 연산의 직관적인 이해와 간단한 항등식 확인을 돕는 시각적 도구입니다. 하지만 엄밀한 증명은 논리적 법칙이나 원소 포함 관계를 통해 이루어져야 합니다.

## 3. 함수 (Functions) - 5.2절

함수는 두 집합 사이의 관계를 기술하는 규칙입니다.

### 3.1 함수의 구성 요소

* **정의역(Domain):** 입력값들의 집합.
* **공역(Codomain):** 가능한 출력값들의 집합.
* **치역(Range/Image):** 실제 출력값들의 집합.
* 함수 $f: A \to B$는 정의역 $A$의 각 원소를 공역 $B$의 **유일한** 원소에 대응시킵니다.

### 3.2 함수의 성질 (Properties)

* **단사 함수(Injection, One-to-One):** 서로 다른 입력은 서로 다른 출력으로 간다. ($f(x) = f(y) \implies x = y$)
* **전사 함수(Surjection, Onto):** 공역의 모든 원소가 선택받는다. (공역 = 치역)
* **전단사 함수(Bijection):** 단사이면서 동시에 전사인 함수. 역함수가 존재하며, 두 집합의 크기(Cardinality)가 같음을 의미합니다.

### 3.3 상과 역상 (Image and Inverse Image)

* **상(Image):** 정의역의 부분집합에 대응하는 공역의 부분집합. $f(S) = \{f(x) : x \in S\}$.
* **역상(Inverse Image):** 공역의 부분집합에 대응하는 정의역의 부분집합. $f^{-1}(T) = \{x : f(x) \in T\}$. (역함수와는 다른 개념임에 주의)

## 4. 요약

**5. Discrete Structures Revisited**는 단순한 복습이 아닙니다.

* **엄밀함:** "직관"에서 "정의와 논리"로 넘어갑니다.
* **도구:** 집합의 연산과 함수의 성질(단사, 전사)은 이후 **생성 함수(Generating Functions)**나 **조합론적 증명**, **알고리즘 분석** 등에서 필수적인 도구로 사용됩니다.
