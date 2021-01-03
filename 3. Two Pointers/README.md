# 双指针算法解释及应用场景

1. **快慢指针**：通常用于解决链表问题

2. **左右指针**：指向同一数组，遍历方向相反且不相交，搜索排好序的**数组**中满足**给定值**的可能组合

3. **固定大小的滑动窗口**：指向同一**数组或字符串**，遍历方向相同且不相交，两个指针包围的
   区域即为当前的窗口，窗口大小固定为**给定值**，区间搜索满足给定条件的substring或subarray

4. **大小不定的滑动窗口**：移动右边界直到遇到停止条件，再移动左指针。通常解决**longest或minimum**的substring或subarray

5. **HashMap或int[128]来记录字符出现的频率**

   



<br/>

<br/>

<br/>

1. Two pointers mainly use to iterate array, they point to different elements to finish the task, it can be extended as multiple arrays with multiple pointers.
2. If two pointers iterate the same array with the **same direction**, this approach also called sliding window as it uses to search in a fixed width.
3. if two pointers iterate the same array with the **opposite direction**, usually this approach can be used to search the **sorted array**.