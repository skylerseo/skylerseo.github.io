---
title: Algorithm(알고리즘)이란?
author: Skyler Seo
date: 2020-09-22 12:43:00 +0900
categories: [dev, algorithm]
tags: [algorithm]
---

# 요약

알고리즘은 어떤 종류의 문제를 풀 수 있는 정확한 방법이며, 일련의 작업을 정확하게 정의해 놓은 규칙들입니다.

`B` - 입문자, `A` - 숙련자

### **주제별 알고리즘**

- **Math**
  - `B` [Bit Manipulation](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/bits) - set/get/update/clear bits, 2의 곱 / 나누기, 음수로 만들기 etc.
  - `B` [팩토리얼](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/factorial)
  - `B` [피보나치 수](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/fibonacci)
  - `B` [소수 판별](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/primality-test) (trial division 방식)
  - `B` [유클리드 호제법](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/euclidean-algorithm) - 최대공약수 (GCD)
  - `B` [최소 공배수](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/least-common-multiple) - LCM
  - `B` [에라토스테네스의 체](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/sieve-of-eratosthenes) - 특정수 이하의 모든 소수 찾기
  - `B` [2의 거듭제곱 판별법](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/is-power-of-two) - 어떤 수가 2의 거듭제곱인지 판별 (naive 와 bitwise 알고리즘)
  - `B` [파스칼 삼각형](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/pascal-triangle)
  - `A` [자연수 분할](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/integer-partition)
  - `A` [리우 후이 π 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/liu-hui) - N-각형을 기반으로 π 근사치 구하기
- **Sets**
  - `B` [카티지언 프로덕트](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/cartesian-product) - 곱집합
  - `B` [Fisher–Yates 셔플](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/fisher-yates) - 유한 시퀀스의 무작위 순열
  - `A` [멱집합](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/power-set) - 집합의 모든 부분집합
  - `A` [순열](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/permutations) (반복 유,무)
  - `A` [조합](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/combinations) (반복 유,무)
  - `A` [최장 공통 부분수열](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/longest-common-subsequence) (LCS)
  - `A` [최장 증가 수열](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/longest-increasing-subsequence)
  - `A` [Shortest Common Supersequence](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/shortest-common-supersequence) (SCS)
  - `A` [배낭 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/knapsack-problem) - "0/1" 과 "Unbound"
  - `A` [최대 구간합](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/maximum-subarray) - "브루트 포스" 과 "동적 계획법" (Kadane's) 버전
  - `A` [조합 합](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/combination-sum) - 특정 합을 구성하는 모든 조합 찾기
- **Strings**
  - `B` [해밍 거리](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/hamming-distance) - 심볼이 다른 위치의 갯수
  - `A` [편집 거리](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/levenshtein-distance) - 두 시퀀스 간위 최소 편집거리
  - `A` [커누스-모리스-프랫 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/knuth-morris-pratt) (KMP 알고리즘) - 부분 문자열 탐색 (패턴 매칭)
  - `A` [Z 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/z-algorithm) - 부분 문자열 탐색 (패턴 매칭)
  - `A` [라빈 카프 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/rabin-karp) - 부분 문자열 탐색
  - `A` [최장 공통 부분 문자열](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/longest-common-substring)
  - `A` [정규 표현식 매칭](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/regular-expression-matching)
- **Searches**
  - `B` [선형 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/search/linear-search)
  - `B` [점프 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/search/jump-search) (or Block Search) - 정렬된 배열에서 탐색
  - `B` [이진 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/search/binary-search) - 정렬된 배열에서 탐색
  - `B` [보간 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/search/interpolation-search) - 균등한 분포를 이루는 정렬된 배열에서 탐색
- **Sorting**
  - `B` [거품 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/bubble-sort)
  - `B` [선택 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/selection-sort)
  - `B` [삽입 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/insertion-sort)
  - `B` [힙 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/heap-sort)
  - `B` [병합 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/merge-sort)
  - `B` [퀵 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/quick-sort) - 제자리(in-place)와 제자리가 아닌(non-in-place) 구현
  - `B` [셸 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/shell-sort)
  - `B` [계수 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/counting-sort)
  - `B` [기수 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/radix-sort)
- **Trees**
  - `B` [깊이 우선 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/tree/depth-first-search) (DFS)
  - `B` [너비 우선 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/tree/breadth-first-search) (BFS)
- **Graphs**
  - `B` [깊이 우선 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/depth-first-search) (DFS)
  - `B` [너비 우선 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/breadth-first-search) (BFS)
  - `B` [크루스칼 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/kruskal) - 최소 신장 트리 찾기 (MST) 무방향 가중 그래프
  - `A` [다익스트라 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/dijkstra) - 한 점에서 다른 모든 점까지 최단 거리 찾기
  - `A` [벨만-포드 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/bellman-ford) - 한 점에서 다른 모든 점까지 최단 거리 찾기
  - `A` [플로이드-워셜 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/floyd-warshall) - 모든 종단 간의 최단거리 찾기
  - `A` [사이클 탐지](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/detect-cycle) - 유방향, 무방향 그래프 (DFS 와 Disjoint Set 에 기반한 버전)
  - `A` [프림 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/prim) - 무방향 가중치 그래프에서 최소 신장 트리 (MST) 찾기
  - `A` [위상 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/topological-sorting) - DFS 방식
  - `A` [단절점](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/articulation-points) - 타잔의 알고리즘 (DFS 기반)
  - `A` [단절선](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/bridges) - DFS 기반 알고리즘
  - `A` [오일러 경로 와 오일러 회로](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/eulerian-path) - Fleury의 알고리즘 - 모든 엣지를 한번만 방문
  - `A` [해밀턴 경로](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/hamiltonian-cycle) - 모든 꼭짓점을 한번만 방문
  - `A` [강결합 컴포넌트](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/strongly-connected-components) - Kosaraju의 알고리즘
  - `A` [외판원 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/travelling-salesman) - 각 도시를 다 방문하고 다시 출발점으로 돌아오는 최단 경로 찾기
- **Uncategorized**
  - `B` [하노이 탑](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/hanoi-tower)
  - `B` [정방 행렬 회전](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/square-matrix-rotation) - 제자리(in-place) 알고리즘
  - `B` [점프 게임](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/jump-game) - 백트래킹, 동적계획법 (top-down + bottom-up), 탐욕 알고리즘 예제
  - `B` [Unique 경로](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/unique-paths) - 백트래킹, 동적계획법, 파스칼 삼각형에 기반한 예제
  - `B` [빗물 담기 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/rain-terraces) - trapping rain water problem (동적계획법, 브루트포스 버전)
  - `A` [N-Queens 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/n-queens)
  - `A` [기사의 여행 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/knight-tour)

### **패러다임별 알고리즘**

알고리즘 패러다임 이란, 알고리즘이 주어진 문제를 해결하기 위해 채택한 기초가 되는 일반적인 방법 혹은 접근법입니다. 알고리즘이 해결하는 문제나 알고리즘의 동작 방식이 완전히 다르더라도,알고리즘의 동작 원칙이 같으면 같은 패러다음을 사용했다고 말할 수 있으며, 주로 알고리즘을 구분하는 기준으로 쓰인다. 알고리즘이 일반적인 컴퓨터의 프로그램에 대한 개념보다 보다 더 추상적인 개념인 것처럼 알고리즘의 패러다임은 명확히 정의된 수학적 실체가 있는 것이 아니기 때문에 그 어떤 알고리즘의 개념보다도 훨씬 추상적인 개념입니다.

- **브루트 포스(Brute Force)** - 가능한 모든 경우를 탐색한 뒤 최적을 찾아내는 방식입니다.
  - `B` [선형 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/search/linear-search)
  - `B` [빗물 담기 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/rain-terraces) - trapping rain water problem
  - `A` [최대 구간합](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/maximum-subarray)
  - `A` [외판원 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/travelling-salesman) - 각 도시를 다 방문하고 다시 출발점으로 돌아오는 최단 경로 찾기
- **탐욕 알고리즘(Greedy)** - 이후를 고려하지 않고 현재 시점에서 가장 최적인 선택을 하는 방식입니다.
  - `B` [점프 게임](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/jump-game)
  - `A` [쪼갤수 있는 배낭 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/knapsack-problem)
  - `A` [다익스트라 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/dijkstra) - 모든 점 까지의 최단거리 찾기
  - `A` [프림 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/prim) - 무방향 가중치 그래프에서 최소 신창 트리 (MST) 찾기
  - `A` [크루스칼 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/kruskal) - 무방향 가중치 그래프에서 최소 신창 트리 (MST) 찾기
- **분할 정복법(Divide and Conquer)** - 문제를 여러 작은 문제로 분할한 뒤 해결하는 방식입니다.
  - `B` [이진 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/search/binary-search)
  - `B` [하노이 탑](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/hanoi-tower)
  - `B` [파스칼 삼각형](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/pascal-triangle)
  - `B` [유클리드 호제법](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/euclidean-algorithm) - 최대공약수 계산 (GCD)
  - `B` [병합 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/merge-sort)
  - `B` [퀵 정렬](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sorting/quick-sort)
  - `B` [트리 깊이 우선 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/tree/depth-first-search) (DFS)
  - `B` [그래프 깊이 우선 탐색](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/depth-first-search) (DFS)
  - `B` [점프 게임](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/jump-game)
  - `A` [순열](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/permutations) (반복 유,무)
  - `A` [조합](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/combinations) (반복 유,무)
- **동적 계획법(Dynamic Programming)** - 이전에 찾은 결과를 이용하여 최종적으로 해결하는 방식입니다.
  - `B` [피보나치 수](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/fibonacci)
  - `B` [점프 게임](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/jump-game)
  - `B` [Unique Paths](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/unique-paths)
  - `B` [빗물 담기 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/rain-terraces) - trapping rain water problem
  - `A` [편집 거리](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/levenshtein-distance) - 두 시퀀스 간의 최소 편집 거리
  - `A` [최장 공통 부분 수열](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/longest-common-subsequence) (LCS)
  - `A` [최장 공통 부분 문자열](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/longest-common-substring)
  - `A` [최장 증가 수열](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/longest-increasing-subsequence)
  - `A` [Shortest Common Supersequence](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/shortest-common-supersequence)
  - `A` [0/1 배낭 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/knapsack-problem)
  - `A` [자연수 분할](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/math/integer-partition)
  - `A` [최대 구간합](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/maximum-subarray)
  - `A` [벨만-포드 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/bellman-ford) - 모든 점 까지의 최단 거리 찾기
  - `A` [플로이드-워셜 알고리즘](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/floyd-warshall) - 모든 종단 간의 최단거리 찾기
  - `A` [정규 표현식 매칭](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/string/regular-expression-matching)
- **백트래킹(Backtracking)** - 모든 가능한 경우를 고려한다는 점에서 브루트 포스와 유사합니다. 하지만 다음 단계로 넘어갈때 마다 모든 조건을 만족했는지 확인하고 진행합니다. 만약 조건을 만족하지 못했다면 뒤로 돌아갑니다 (백트래킹). 그리고 다른 경로를 선택합니다. 보통 상태를 유지한 DFS 탐색을 많이 사용합니다.
  - `B` [점프 게임](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/jump-game)
  - `B` [Unique Paths](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/unique-paths)
  - `A` [해밀턴 경로](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/hamiltonian-cycle) - 모든 점을 한번씩 방문
  - `A` [N-Queens 문제](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/n-queens)
  - `A` [기사의 여행](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/uncategorized/knight-tour)
  - `A` [조합 합](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/sets/combination-sum) - 특정 합을 구성하는 모든 조합 찾기
- **분기 한정법** - 백트래킹으로 찾은 각 단계의 최소 비용이 드는 해를 기억해 두고 있다가, 이 비용을 이용해서 더 낮은 최적의 해를 찾습니다. 기억해둔 최소 비용들을 이용해 더 높은 비용이 드는 해결법을 탐색 안함으로써 불필요한 시간 소모를 줄입니다. 보통 상태 공간 트리의 DFS 탐색을 이용한 BFS 탐색 방식에서 사용됩니다.

# 상세

알고리즘 (algorithm [ǽlɡərìðm])은 수학과 컴퓨터 과학, 언어학 또는 관련 분야에서 어떠한 문제를 해결하기 위해 정해진 일련의 절차나 방법을 공식화한 형태로 표현한 것, 계산을 실행하기 위한 단계적 절차를 의미한다.

알고리즘은 연산, 데이터 진행 또는 자동화된 추론을 수행한다. 산법(算法), 셈법, 계산 절차 등으로 번역되기도 한다.

# 명칭

알고리즘은 9세기 페르시아의 수학자인 무하마드 알콰리즈미(Muhammad al-Kwarizmi)의 이름을 라틴어화한 algorismus에서 따온 말이다.

# 정의

[정지 문제](https://ko.wikipedia.org/wiki/%EC%A0%95%EC%A7%80_%EB%AC%B8%EC%A0%9C)의 결과로 알고리즘이 정지하는 데 걸리는 시간을 일반적으로 측정할 수 없다.

그러므로 알고리즘에 대해 단순한 직관을 만족하는 형식적인 정의는 불가능하다.

따라서 알고리즘의 공식적인 정의는 없다.

대부분의 알고리즘은 유한한 수의 규칙에 따라 구별 가능한 기호들을 조작하여 입력 정수에서 출력 정수를 생성하기 위한 일반화된 작업을 정의한다. 다음은 좋은 알고리즘의 특징이다.

- 정밀성 : 변하지 않는 명확한 작업 단계를 가져야 한다.
- 유일성 : 각 단계마다 명확한 다음 단계를 가져야 한다.
- 타당성 : 구현할 수 있고 실용적이어야 한다.
- 입력 : 정의된 입력을 받아들일 수 있어야 한다.
- 출력 : 답으로 출력을 내보낼 수 있어야 한다.
- 유한성 : 특정 수의 작업 이후에 정지해야 한다.
- 일반성 : 정의된 입력들에 일반적으로 적용할 수 있어야 한다.

# 구현

알고리즘은 자연어, 의사코드, 순서도, 프로그래밍 언어, 인터프리터가 작업하는 제어 테이블, 유한 상태 기계의 상태도 등으로 표현할 수 있다. 다음은 알고리즘 개발의 정형적인 단계이다.

문제 정의 → 모델 고안 → 명세 작성 → 설계 → 검증 → 분석 (복잡도 등) → 구현 → 테스트 → 문서화

알고리즘을 설계하는 기술에는 운용 과학의 방법, 설계 패턴을 이용하는 방법 등이 있다. 대부분의 알고리즘은 컴퓨터 프로그램으로 구현되지만, 전기 회로나 생물학적 신경 회로를 사용하기도 한다.

# 분류

- [구현](https://ko.wikipedia.org/wiki/%EA%B5%AC%ED%98%84) : [재귀적 알고리즘](https://ko.wikipedia.org/wiki/%EC%9E%AC%EA%B7%80%ED%95%A8%EC%88%98), [연역적 알고리즘](https://ko.wikipedia.org/wiki/%EC%97%B0%EC%97%AD), [결정론적 알고리즘](https://ko.wikipedia.org/wiki/%EA%B2%B0%EC%A0%95%EB%A1%A0%EC%A0%81_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98), [근사 알고리즘](https://ko.wikipedia.org/wiki/%EA%B7%BC%EC%82%AC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98), [양자 알고리즘](https://ko.wikipedia.org/w/index.php?title=%EC%96%91%EC%9E%90_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98&action=edit&redlink=1) 등.
- 설계 : [무차별 대입 공격](https://ko.wikipedia.org/wiki/%EB%AC%B4%EC%B0%A8%EB%B3%84_%EB%8C%80%EC%9E%85_%EA%B3%B5%EA%B2%A9), [분할 정복 알고리즘](https://ko.wikipedia.org/wiki/%EB%B6%84%ED%95%A0_%EC%A0%95%EB%B3%B5_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98), [그래프 순회](https://ko.wikipedia.org/wiki/%EA%B7%B8%EB%9E%98%ED%94%84_%EC%88%9C%ED%9A%8C), [분기 한정법](https://ko.wikipedia.org/wiki/%EB%B6%84%EA%B8%B0_%ED%95%9C%EC%A0%95%EB%B2%95), [확률적 알고리즘](https://ko.wikipedia.org/wiki/%ED%99%95%EB%A5%A0%EC%A0%81_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98), [리덕션](<https://ko.wikipedia.org/wiki/%ED%99%98%EC%82%B0_(%EB%B3%B5%EC%9E%A1%EB%8F%84)>), [백트래킹](https://ko.wikipedia.org/wiki/%ED%87%B4%EA%B0%81%EA%B2%80%EC%83%89) 등.
- [최적화 문제](https://ko.wikipedia.org/wiki/%EC%B5%9C%EC%A0%81%ED%99%94_%EB%AC%B8%EC%A0%9C) : [선형 계획법](https://ko.wikipedia.org/wiki/%EC%84%A0%ED%98%95_%EA%B3%84%ED%9A%8D%EB%B2%95), [동적 계획법](https://ko.wikipedia.org/wiki/%EB%8F%99%EC%A0%81_%EA%B3%84%ED%9A%8D%EB%B2%95), [탐욕 알고리즘](https://ko.wikipedia.org/wiki/%ED%83%90%EC%9A%95_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98), [휴리스틱 함수](https://ko.wikipedia.org/wiki/%ED%9C%B4%EB%A6%AC%EC%8A%A4%ED%8B%B1_%ED%95%A8%EC%88%98) 등.
- 이론적 분야 : [검색 알고리즘](https://ko.wikipedia.org/wiki/%EB%B6%84%EB%A5%98:%EA%B2%80%EC%83%89_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98), [정렬 알고리즘](https://ko.wikipedia.org/wiki/%EC%A0%95%EB%A0%AC_%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98), [수치 알고리즘](https://ko.wikipedia.org/wiki/%EC%88%98%EC%B9%98%ED%95%B4%EC%84%9D%ED%95%99), [그래프 알고리즘](https://ko.wikipedia.org/wiki/%EA%B7%B8%EB%9E%98%ED%94%84_%EC%9D%B4%EB%A1%A0), [문자열 알고리즘](https://ko.wikipedia.org/wiki/%EB%AC%B8%EC%9E%90%EC%97%B4), [암호학적 알고리즘](https://ko.wikipedia.org/wiki/%EC%95%94%ED%98%B8%ED%95%99), [기계 학습](https://ko.wikipedia.org/wiki/%EA%B8%B0%EA%B3%84_%ED%95%99%EC%8A%B5), [데이터 압축](https://ko.wikipedia.org/wiki/%EB%8D%B0%EC%9D%B4%ED%84%B0_%EC%95%95%EC%B6%95) 등.

## Materials

### wikipedia

<https://ko.wikipedia.org/wiki/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98#:~:text=%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98(%EB%9D%BC%ED%8B%B4%EC%96%B4%2C%20%EB%8F%85%EC%9D%BC%EC%96%B4%3A%20Algorithmus,%ED%95%98%EA%B8%B0%20%EC%9C%84%ED%95%9C%20%EB%8B%A8%EA%B3%84%EC%A0%81%20%EC%A0%88%EC%B0%A8%EB%A5%BC>

### github.com/trekhleb/javascript-algorithms

<https://github.com/trekhleb/javascript-algorithms/blob/master/README.ko-KR.md>
