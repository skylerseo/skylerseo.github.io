---
title: 이중 연결 리스트 (Doubly Linked List)
author: Skyler Seo
date: 2020-10-15 10:12:00 +0900
categories: [dev, data-structure]
tags: [data-structure, doubly-linked-list]
---

### This is Korean translation from me, the original link is [here](https://github.com/trekhleb/javascript-algorithms/tree/master/src/data-structures/doubly-linked-list).

# 이중 연결 리스트(Doubly Linked List)

_Read this in other languages:_
[_Русский_](README.ru-RU.md),
[_简体中文_](README.zh-CN.md),
[_日本語_](README.ja-JP.md),
[_Português_](README.pt-BR.md)

컴퓨터과학에 있어서 **이중 연결 리스트**는 노드라고 불리우는 일련의 링크 레코드로 이루어진 연결 데이터 구조입니다. 각 노드는 Links라고 불리는 2개의 필드를 가지고 있는데, 이것들은 일련의 노드 안에서 이전 노드와 다음 노드를 참조하고 있습니다. 첫번째 노드 앞의 링크와 마지막 노드 다음의 링크는 어떤 의미로 끝을 나타내고 있고, 일반적으로는 더미노드나 null이 들어있어 리스트의 순회(traversal)를 쉽게 실행할 수 있게 되어있습니다. 만일 더미노드가 1개밖에 없다면 리스트는 그 1개의 노드를 통해서 순환적으로 연결(Link)됩니다. 이는 각각 역순의 연결리스트(singly linked lists)가 2개 있는 것이라고 생각할 수 있습니다.

![Doubly Linked List](https://upload.wikimedia.org/wikipedia/commons/5/5e/Doubly-linked-list.svg)

2개의 링크에 의해, 리스트를 어느 방향이든지 순회(traverse)시키는 것이 가능합니다. 이중 리스트는 노드의 추가나 삭제를 위해, 이중 연결 리스트와 비교해서 보다 많은 링크를 변경할 필요가 있습니다. 하지만 그 조작은 간단하고 보다 효율적일(최초의 노드 이외인 경우) 가능성이 있습니다. 이전 노드의 링크를 갱신할 때에 이전 노드를 보존하거나, 이전 노드를 바라보기 위해서 리스트를 순회(traverse)시킬 필요는 없습니다.

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
    n.previous ← tail
    tail.next ← n
    tail ← n
  end if
end Add
```

### 삭제

```text
Remove(head, value)
  Pre: head is the head node in the list
       value is the value to remove from the list
  Post: value is removed from the list, true; otherwise false
  if head = ø
    return false
  end if
  if value = head.value
    if head = tail
      head ← ø
      tail ← ø
    else
      head ← head.next
      head.previous ← ø
    end if
    return true
  end if
  n ← head.next
  while n = ø and value !== n.value
    n ← n.next
  end while
  if n = tail
    tail ← tail.previous
    tail.next ← ø
    return true
  else if n = ø
    n.previous.next ← n.next
    n.next.previous ← n.previous
    return true
  end if
  return false
end Remove
```

### 역순회

```text
ReverseTraversal(tail)
  Pre: tail is the node of the list to traverse
  Post: the list has been traversed in reverse order
  n ← tail
  while n = ø
    yield n.value
    n ← n.previous
  end while
end Reverse Traversal
```

## 복잡도

## 시간 복잡도

| Access | Search | Insertion | Deletion |
| :----: | :----: | :-------: | :------: |
|  O(n)  |  O(n)  |   O(1)    |   O(n)   |

### 공간 복잡도

O(n)

## 참고자료

- [Wikipedia](https://en.wikipedia.org/wiki/Doubly_linked_list)
- [YouTube](https://www.youtube.com/watch?v=JdQeNxWCguQ&t=7s&index=72&list=PLLXdhg_r2hKA7DPDsunoDZ-Z769jWn4R8)
