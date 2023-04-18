# BFS/DFS

![dfsbfs](https://user-images.githubusercontent.com/65147869/232435616-b41f78df-79b7-4707-a6c2-f0a38d003705.gif)

- O(N) 시간복잡도
- 재귀를 이용한 DFS은 수행시간이 느려질 수 있다. 재귀를 이용하지 않은 DFS나 BFS를 이용하는 테크닉이 필요할 수 있음

<br>

 **학습 동기**
- SW Expert Academy, [1244. 최대 상금](https://swexpertacademy.com/main/code/problem/problemDetail.do?problemLevel=3&contestProbId=AV15Khn6AN0CFAYD&categoryId=AV15Khn6AN0CFAYD&categoryType=CODE&problemTitle=&orderBy=RECOMMEND_COUNT&selectCodeLang=PYTHON&select-1=3&pageSize=10&pageIndex=1&&&&&&&&&&)
문제 해결법
- 알고리즘 서적 <이것이 취업을 위한 코딩 테스트다 with Python> DFS/BFS 학습 중

- [Backtracking](Backtracking.md) 알고리즘의 근간이 되는 기법



<br>


# 선행 학습
### [Stack](../DATA%20STRUCTURE/Stack.md)
후입선출(LIFO) 방식의 자료구조

### [Queue](../DATA%20STRUCTURE/Queue.md)
선입선출(FIFO) 방식의 자료구조

### [Graph](../DATA%20STRUCTURE/Graph.md)
정점(node)과 정점들을 연결하는 간선(edge)으로 구성된 자료구조

### [Recursive | 재귀](./Recursive.md)
재귀함수를 이용한 DFS를 이해하기 위한 선행 알고리즘   
**"함수 내부에서 자신을 호출하는 것"**

<br>

# DFS | Deep First Search
**Stack + Graph** 자료구조 기반의 완전탐색 알고리즘  

가장 깊은 노드까지 갔다가 돌아오며 방문하지 않은 노드들을 방문한다.  
[Backtracking](Backtracking.md) 알고리즘의 근간이 되는 기법  

<br>

# BFS | Breadth First Search
**Queue + Graph** 자료구조 기반의 완전탐색 알고리즘

Queue를 이용하여 자연스럽게 인접한 노드부터 방문할 수 있다.  
Python으로 구현시 [deque] 라이브러리를 사용하는 것이 좋다.  
일반적인 경우 DFS보다 수행시간이 좋은 편이다.  
