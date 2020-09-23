---
title: Data structure(자료구조)란?
author: Skyler Seo
date: 2020-09-22 12:40:00 +0900
categories: [dev, data-structure]
tags: [data-structure]
---

# 요약

자료 구조는 데이터를 특정 방식으로 구성하고 저장함으로써 더 효율적으로 접근하고 수정할 수 있게 해줍니다. 간단히 말해, 자료 구조는 데이터 값들, 데이터 간의 관계, 그리고 데이터를 다룰 수 있는 함수와 작업의 모임입니다.

`B` - 입문자, `A` - 숙련자

- `B` [연결 리스트](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/linked-list)
- `B` [이중 연결 리스트](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/doubly-linked-list)
- `B` [큐](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/queue)
- `B` [스택](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/stack)
- `B` [해시 테이블](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/hash-table)
- `B` [힙](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/heap)
- `B` [우선순위 큐](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/priority-queue)
- `A` [트라이](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/trie)
- `A` [트리](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/tree)
  - `A` [이진 탐색 트리](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/tree/binary-search-tree)
  - `A` [AVL 트리](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/tree/avl-tree)
  - `A` [Red-Black 트리](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/tree/red-black-tree)
  - `A` [세그먼트 트리](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/tree/segment-tree) - min/max/sum range 쿼리 예제.
  - `A` [Fenwick 트리](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/tree/fenwick-tree) (Binary Indexed Tree)
- `A` [그래프](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/graph) (유방향, 무방향)
- `A` [서로소 집합](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/disjoint-set)
- `A` [블룸 필터](https://github.com/trekhleb/javascript-algorithms/blob/master/src/data-structures/bloom-filter)

# 상세

**자료구조**(資料構造, [영어](https://ko.wikipedia.org/wiki/%EC%98%81%EC%96%B4): data structure)는 [컴퓨터 과학](https://ko.wikipedia.org/wiki/%EC%BB%B4%ED%93%A8%ED%84%B0_%EA%B3%BC%ED%95%99)에서 [효율적인](https://ko.wikipedia.org/w/index.php?title=%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98_%ED%9A%A8%EC%9C%A8%EC%84%B1&action=edit&redlink=1) 접근 및 수정을 가능케 하는 자료의 조직, 관리, 저장을 의미한다. 더 정확히 말해, 자료 구조는 데이터 값의 모임, 또 데이터 간의 관계, 그리고 데이터에 적용할 수 있는 함수나 명령을 의미한다. 신중히 선택한 자료구조는 보다 효율적인 [알고리즘](https://ko.wikipedia.org/wiki/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)을 사용할 수 있게 한다. 이러한 자료구조의 선택문제는 대개 [추상 자료형](https://ko.wikipedia.org/wiki/%EC%B6%94%EC%83%81_%EC%9E%90%EB%A3%8C%ED%98%95)의 선택으로부터 시작하는 경우가 많다. 효과적으로 설계된 자료구조는 실행시간 혹은 메모리 용량과 같은 자원을 최소한으로 사용하면서 연산을 수행하도록 해준다.

자료구조에는 여러 종류가 있으며, 이러한 각각의 자료구조는 각자의 연산 및 목적에 맞추어져 있다. 예를 들어 [B-트리](https://ko.wikipedia.org/wiki/B-%ED%8A%B8%EB%A6%AC)는 데이터베이스에 효율적이며, [라우팅 테이블](https://ko.wikipedia.org/wiki/%EB%9D%BC%EC%9A%B0%ED%8C%85_%ED%85%8C%EC%9D%B4%EB%B8%94)은 네트워크(인터넷, 인트라넷)에 일반적이다.

다양한 프로그램을 설계할 때, 어떠한 자료구조를 선택할지는 가장 우선적으로 고려되어야 한다. 이는 큰 시스템을 제작할 때 구현의 난이도나 최종 결과물의 성능이 자료구조에 크게 의존한다는 것을 많은 경험이 뒷받침하기 때문이다. 일단 자료구조가 선택되면 적용할 [알고리즘](https://ko.wikipedia.org/wiki/%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98)은 상대적으로 명확해지기 마련이다. 때로는 반대 순서로 정해지기도 하는데, 이는 목표로 하는 연산이 특정한 알고리즘을 반드시 필요로 하며, 해당 알고리즘은 특정 자료구조에서 가장 나은 성능을 발휘할 때와 같은 경우이다. 어떠한 경우든, 적절한 자료구조의 선택은 필수적이다.

이러한 관점은 알고리즘보다 자료구조가 보다 중요한 요소로 적용되는 많은 정형화된 개발론 그리고 [프로그래밍 언어](https://ko.wikipedia.org/wiki/%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D_%EC%96%B8%EC%96%B4)의 개발을 촉발시켰다. 대부분의 언어는 일정 수준의 모듈개념을 가지고 있으며, 이는 자료구조가 검증된 구현은 감춘 채 인터페이스만을 이용하여 다양한 프로그램에서 사용되는 것을 가능하게 해준다. [C++](https://ko.wikipedia.org/wiki/C%2B%2B), [자바](<https://ko.wikipedia.org/wiki/%EC%9E%90%EB%B0%94_(%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D_%EC%96%B8%EC%96%B4)>)와 같은 [객체지향](https://ko.wikipedia.org/wiki/%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5) 프로그래밍 언어는 특별히 이러한 목적으로 객체를 사용한다.

이러한 자료구조의 중요성으로 말미암아, 최근의 프로그래밍 언어 및 개발 환경은 다양한 [표준 라이브러리](https://ko.wikipedia.org/wiki/%ED%91%9C%EC%A4%80_%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC)를 제공하고 있다. 예로, C++의 [표준 템플릿 라이브러리](https://ko.wikipedia.org/wiki/%ED%91%9C%EC%A4%80_%ED%85%9C%ED%94%8C%EB%A6%BF_%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC)나 자바의 [자바 API](https://ko.wikipedia.org/wiki/%EC%9E%90%EB%B0%94_API), [마이크로소프트 .NET](https://ko.wikipedia.org/wiki/%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8_.NET)과 같은 것들을 들 수 있다.

자료구조에서 가장 기초적인 단위는 [행렬](https://ko.wikipedia.org/wiki/%ED%96%89%EB%A0%AC), [레코드](https://ko.wikipedia.org/wiki/%EB%A0%88%EC%BD%94%EB%93%9C), [유니온](https://ko.wikipedia.org/wiki/%EC%9C%A0%EB%8B%88%EC%98%A8), [참조](https://ko.wikipedia.org/wiki/%EC%B0%B8%EC%A1%B0)와 같은 것이다. 예를 들어, Nullable 참조는 참조와 유니온의 조합으로 나타낼 수 있으며, 가장 단순한 자료구조 가운데 하나인 [연결 리스트](https://ko.wikipedia.org/wiki/%EC%97%B0%EA%B2%B0_%EB%A6%AC%EC%8A%A4%ED%8A%B8)는 레코드와 Nullable 참조로 나타낼 수 있다.

## Materials

[wikipedia](https://ko.wikipedia.org/wiki/%EC%9E%90%EB%A3%8C_%EA%B5%AC%EC%A1%B0#:~:text=%EC%9E%90%EB%A3%8C%EA%B5%AC%EC%A1%B0(%E8%B3%87%E6%96%99%E6%A7%8B%E9%80%A0%2C%20%EC%98%81%EC%96%B4,%EB%82%98%20%EB%AA%85%EB%A0%B9%EC%9D%84%20%EC%9D%98%EB%AF%B8%ED%95%9C%EB%8B%A4.)

[github.com/trekhleb/javascript-algorithms](https://github.com/trekhleb/javascript-algorithms/blob/master/README.ko-KR.md)
