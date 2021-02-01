# Input Size vs. Time Complexity

CPU：10^6 ~ 10^7 ops/secs

| input size  | time complexity |                algorithm                |
| :---------: | :-------------: | :-------------------------------------: |
|   1 ~ 10    |      O(n!)      |            permutation (DFS)            |
|   15 ~ 20   |     O(2^n)      |            combination (DFS)            |
|   10 ~ 50   |     O(n^4)      |          four nested for loops          |
|  100 ~ 200  |     O(n^3)      |         three nested for loops          |
| 100 ~ 2000  |     O(n^2)      |          two nested for loops           |
|   <= 10^6   |    O(nlogn)     | greedy, sort + for loop, priority queue |
|   <= 10^7   |      O(n)       |          graph, tree traversal          |
| <= 2^31 - 1 |     O(logn)     |              binary search              |

