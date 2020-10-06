# 브루트 포스(brute force)
- brute: 무식한, force: 힘   무식한 힘으로 해석할 수 있다.

완전탐색 알고리즘. 즉, 가능한 모든 경우의 수를 모두 탐색하면서 요구조건에 충족되는 결과만을 가져온다.

이 알고리즘의 강력한 점은 예외 없이 100%의 확률로 정답만을 출력한다.

- 일반적인 방법으로 문제를 해결하기 위해서는 모든 자료를 탐색해야 하기 때문에 특정한 구조를 전체적으로 탐색할 수 있는 방법을 필요로 한다.

- 알고리즘 설계의 가장 기본적인 접근 방법은 해가 존재할 것으로 예상되는 모든 영역을 전체 탐색하는 방법이다.

- **선형 구조**를 전체적으로 탐색하는 `순차 탐색`, **비선형 구조**를 전체적으로 탐색하는 `깊이 우선 탐색(DFS, Depth First
 Search)`과 `너비 우선 탐색(BFS, breadth first search)`이 가장 기본적인 도구이다.

- `너비 우선 탐색`은 `브루트 포스`와 관련이 깊고, `깊이 우선 탐색`은 다음에 작성될 `백트래킹`과 관련이 깊다.

### 문제해결 방법  
1. 문제를 선형 구조로 구조화한다.

2. 구조화된 문제공간을 적절한 방법으로 해를 구성할 때까지 탐색한다.

3. 구성된 해를 정리한다.
 
 
 
### 너비 우선 탐색(BFS, Breadth-first search)
- 그래프에서 완전탐색 방법 중 하나

- 탐색트리의 루트노드부터 목표노드를 만날 때까지 단계별로 횡방향으로 탐색을 진행해 나가는 방식

#### 장점
- 출발노드에서 목표노드까지의 최단 길이 경로를 보장한다.

#### 단점
- 경로가 매우 길 경우에는 탐색 가지가 급격히 증가함에 따라 보다 많은 기억 공간을 필요로 한다.

- 해가 존재하지 않는다면 유한(finite) 그래프의 경우에는 모든 그래프를 탐색한 후에 실패로 끝난다.

- 무한(infinite) 그래프의 경우에는 결코 해를 찾지도 못하고, 끝내지도 못한다.

즉, **'해가 하나 이상 존재한다'** 라는 가정을 세우고 모든 영역을 탐색한다.