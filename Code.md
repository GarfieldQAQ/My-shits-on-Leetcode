# 2025.5.20 差分数组
---
[leetcode网址](https://leetcode.cn/problems/zero-array-transformation-i/description/?envType=daily-question&envId=2025-05-20)
<iframe src="https://leetcode.cn/problems/zero-array-transformation-i/description/?envType=daily-question&envId=2025-05-20" width="1000" height="600"></iframe>

## Tips:
---
```txt
最开始采取了一遍遍历 queries，一边操作 nums的方法，最终在大数据测试用例的折磨下超时力
后来看到使用差分数组的解法，使用差分数组记录前后项差值，因为本题中默认减到 0就不再操作，判断只需第一项小于零，从第二项起，与前一项的加和小于零即可
```
# 2025.5.22 差分数组，贪心，队列
---
[leetcode网址](https://leetcode.cn/problems/zero-array-transformation-iii/description/?envType=daily-question&envId=2025-05-22)

<iframe src="https://leetcode.cn/problems/zero-array-transformation-iii/description/?envType=daily-question&envId=2025-05-22" width="1000" height="600"></iframe>

## Tips:
---
```txt
完全没有思路的一集
按照题解，首先对 queries进行升序排序，对于 nums[0]，将 queries中 queries[i][0] == nums[0]的queries压入优先 queue，再根据操作数操作将需要的 queries.pop，更新 deltaArray ...
```
# 2025.6.9 字典序的第k小数字

[leetcode网址](https://leetcode.cn/problems/k-th-smallest-in-lexicographical-order/description/)

# 2025.6.14 替换一个数字后的最大差值
[leetcode网址](https://leetcode.cn/problems/maximum-difference-by-remapping-a-digit/description/?envType=daily-question&envId=2025-06-14)
<iframe src="https://leetcode.cn/problems/zero-array-transformation-iii/description/?envType=daily-question&envId=2025-06-14" width="1000" height="600"></iframe>
## Tips:
```txt
引入十进制musk 解决问题，首先想要取到最大值只需将不为9 的最高位数字替换成9 即可找到最大值，然后将最大值所有的9 替换成0 即可得到最小值。
因此首先记录最高位数字，等于最高位数字为1 否则为0 制作musk
接着记录第一位不为9 的数字。同样制作musk
然后通过两个掩码即可求解
```

# 2025.6.16 读数据结构 最大子序列和

惊为天人 O(N)
![[Pasted image 20250616202140.png]]
