# BOJ 16457번 [단풍잎 이야기](https://www.acmicpc.net/problem/16457)

## 🌈 풀이 후기
* 까먹었던 조합 문제에 대해 다시 생각해 볼 수 있어서 좋았습니다.
## 👩‍🏫 문제 풀이
* ```int[][] skillMap```에 각 퀘스트 별 수행해야 할 스킬 목록들을 저장합니다.
* 1~2*N까지 K 개를 뽑는 조합을 구합니다.
    * 각 조합을 구할 때마다 ```int[] used ``` 배열에 스킬 번호를 저장합니다.
    * 해당 스킬 번호 리스트로 몇 개의 퀘스트를 수행할 수 있는지 ```getPassQuestCnt()``` 를 통해 구합니다.
    * ```maxQuest``` 값을 갱신하며 최대 수행할 수 있는 퀘스트 개수를 갱신합니다.