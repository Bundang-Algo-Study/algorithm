# BOJ 15681번 [트리와 쿼리](https://www.acmicpc.net/problem/15681)

## 🌈 풀이 후기
* 트리의 부모찾기 방법으로 풀 방법을 찾다가 시간초과 될 것 같아서 해답을 찾아봤습니다.
* 인접리스트와 dfs로 공간복잡도를 넘기지 않고 간단하게 풀 수 있었습니다.
## 👩‍🏫 문제 풀이
* 2차원 인접리스트를 만들어서 간선의 정보를 2중으로 저장합니다.
* dfs를 돌면서 자식노드의 개수를 업데이트합니다.
    * visit 배열을 확인하면서 순환구조에 빠지지 않게 합니다.
    * dp 배열은 자식노드의 개수를 저장하는 배열로, 자신의 개수 1개도 포함합니다.
* Q를 받으면서 답을 출력합니다.