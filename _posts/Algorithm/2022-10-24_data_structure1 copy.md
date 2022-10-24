---
layout: single
title:  "자료구조 맛보기 - BFS"
categories: Algorithm
tag: [BFS, DFS]
toc: true
toc_sticky: true
author_profile: true
sidebar:
  nav: "docs"
---

1. BFS

그래프 탐색 : 어떤것들이 연속해서 이어질때, 모두 확인하는방법

- Graph : Vertex(어떤것) + Edge(이어지는것)

그래프 탐색 종류



- BFS : Breadth-first-search(너비 우선 탐색) : 자식 탐색 → 자식 탐색(첫 노드에서 손자)
- DFS: Depth-first search(깊이 우선 탐색)

2. BFS의 코드 구현
- 시작점에 연결된 Vertex 찾기
- 찾은 Vertext를 Queue에 저장
- Queue의 가장 먼저 것 뽑아서 반복

시간복잡도

- 알고리즘이 얼마나 오래걸리는지
- BFS : O(V+E)



## 📑 출처
 - [개발자 장고](https://www.youtube.com/watch?v=ansd5B27uJM)
