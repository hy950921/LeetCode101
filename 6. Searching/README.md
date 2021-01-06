# 优先搜索算法

## 1. DFS

深度优先搜索类型的题可以分为主函数和辅函数，主函数用于遍历所有的搜索位置，判断是否可以开始搜索，如果
可以即在辅函数进行搜索。辅函数则负责深度优先搜索的递归调用。在辅函数里确定返回值是什么，一个一定要注意的点是辅函数内递归搜索时，在第一行进行边界条件的判定。

```java
main(int[][] grid) {
	for (0, i, grid.length) {
		for (0, j, grid[0].length) {
			if current position(grid[i][j]) == target {
				dfs();
			}
		}
	}
}

dfs(int[][] grid) {
	border cases to end the dfs
	dfs in four directions
}
```

