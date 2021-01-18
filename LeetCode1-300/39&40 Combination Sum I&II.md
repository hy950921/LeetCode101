# 39/40. Combination Sum I/II

```java

void backtrack(可选择列表，指针，目标值，当前路径，result) {
	if (目标值 == 0) {
		result.add(当前路径);
		return;
	}
	for (i = 指针; 可选择列表.length; i++) {
         选项 = 可选择列表[i];
         当前路径.add(选项);
		backtrack();
		当前路径.removeLastOne();
	}
}
```

情况一：同一个元素可以反复使用`dfs(i)` 从头开始搜索，如果只能用一次则`dfs(i+1)`略过前一个元素

情况二：数组中有重复数，结果不能有重复的组合，`[i] = [i-1] && i > index continue` 不是这个循环的第一个元素并且该元素和前一个相等则可以去重