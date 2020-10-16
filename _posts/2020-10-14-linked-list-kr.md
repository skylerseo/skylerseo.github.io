---
title: 연결 리스트 (Linked List)
author: Skyler Seo
date: 2020-10-14 22:16:00 +0900
categories: [dev, data-structure]
tags: [data-structure, linked-list]
---

### This is Korean translation from me, the original post is [here](https://github.com/trekhleb/javascript-algorithms/tree/master/src/data-structures/linked-list).

# 연결 리스트(Linked List)

_Read this in other languages:_
[_简体中文_](README.zh-CN.md),
[_Русский_](README.ru-RU.md),
[_日本語_](README.ja-JP.md),
[_Português_](README.pt-BR.md)

컴퓨터 과학에서 **연결 리스트**는 데이터 요소의 선형 콜렉션입니다. 요소의 순번은 메모리 안의 물리적인 배치에 의해 정해지는 것은 아닙니다. 대신 각 요소가 다음 요소를 가리키고 있습니다. 연결 리스트는 노드의 그룹으로 이루어진 데이터 구조입니다. 가장 단순한 형식으로는, 각 노드는 데이터와 시퀀스 내에서 다음 노드에 대한 참조(즉, Link)로 구성되어 있습니다. 이 구조는 이터레이션에서 임의의 위치에 요소를 효율적으로 삽입, 삭제를 가능하게 합니다. 더욱 복잡한 연결 리스트에서는 링크를 더 많이 추가하여 임의의 요소의 참조로부터 요소를 효율적으로 삽입, 삭제가 가능하게 하고 있습니다. 연결 리스트의 단점은 액세스타임이 선형(그리고 파이프라인 처리가 어려움)인 것입니다. 랜덤 액세스와 같은 고속 액세스는 실현 불가능합니다. 배열이 연결 리스트와 비교해서 캐쉬의 지역성이 더 뛰어납니다.

![Linked List](https://upload.wikimedia.org/wikipedia/commons/6/6d/Singly-linked-list.svg)

## 기본 조작을 위한 의사코드(Pseudocode)

### 삽입

```text
Add(value)
  Pre: value is the value to add to the list
  Post: value has been placed at the tail of the list
  n ← node(value)
  if head = ø
    head ← n
    tail ← n
  else
    tail.next ← n
    tail ← n
  end if
end Add
```

```text
Prepend(value)
 Pre: value is the value to add to the list
 Post: value has been placed at the head of the list
 n ← node(value)
 n.next ← head
 head ← n
 if tail = ø
   tail ← n
 end
end Prepend
```

### 검색

```text
Contains(head, value)
  Pre: head is the head node in the list
       value is the value to search for
  Post: the item is either in the linked list, true; otherwise false
  n ← head
  while n != ø and n.value != value
    n ← n.next
  end while
  if n = ø
    return false
  end if
  return true
end Contains
```

### 삭제

```text
Remove(head, value)
  Pre: head is the head node in the list
       value is the value to remove from the list
  Post: value is removed from the list, true, otherwise false
  if head = ø
    return false
  end if
  n ← head
  if n.value = value
    if head = tail
      head ← ø
      tail ← ø
    else
      head ← head.next
    end if
    return true
  end if
  while n.next != ø and n.next.value != value
    n ← n.next
  end while
  if n.next != ø
    if n.next = tail
      tail ← n
    end if
    n.next ← n.next.next
    return true
  end if
  return false
end Remove
```

### 순회(Traverse)

```text
Traverse(head)
  Pre: head is the head node in the list
  Post: the items in the list have been traversed
  n ← head
  while n != ø
    yield n.value
    n ← n.next
  end while
end Traverse
```

### 역순회(Traverse in Reverse)

```text
ReverseTraversal(head, tail)
  Pre: head and tail belong to the same list
  Post: the items in the list have been traversed in reverse order
  if tail != ø
    curr ← tail
    while curr != head
      prev ← head
      while prev.next != curr
        prev ← prev.next
      end while
      yield curr.value
      curr ← prev
    end while
   yield curr.value
  end if
end ReverseTraversal
```

## 복잡도

### 시간 복잡도

| Access | Search | Insertion | Deletion |
| :----: | :----: | :-------: | :------: |
|  O(n)  |  O(n)  |   O(1)    |   O(n)   |

### 공간 복잡도

O(n)

## 참고자료

- [Wikipedia](https://en.wikipedia.org/wiki/Linked_list)
- [YouTube](https://www.youtube.com/watch?v=njTh_OwMljA&index=2&t=1s&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)
