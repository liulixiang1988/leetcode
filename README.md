# Leetcode解题分类
---

* 算法思想
    * 二分查找
        1. No.33
        2. No.34 分别二分查找范围的start和end
        3. No.81 去掉重复的元素，然后就和No.33一样了
        4. No.153
        5. No.162 对index做二分
        6. Mo.287 n+1个数，范围为a~(n-a+1)，在a~(n-a+1)范围内做二分
        7. No.378
        8. No.522 利用二分查找来判断是否是子序列
        9. No.524 同No.522
        10. No.540
        11. No.658
        12. No.729 因为是在线算法，所以不适合使用排序
    * 贪心思想
        1. No.11 遍历容器的两条垂直边，每次移动较小的那一边
        2. No.659
    * 2-pointer
        * 滑动窗口
            1. No.3 用flag存储窗口内元素出现的次数
            2. No.11 遍历容器的两条垂直边，每次移动较小的那一边
            3. No.209
            4. No.413
            5. No.424
            6. No.467
            7. No.495
            8. No.567 滑动计数
            9. No.678 用一个cnt可以判断不含“*”的括号表达式是否合法，在含有“*”的表达式，用lo和hi表示cnt的取值范围，最后看0是否在取值范围内
            10. No.713 向前推进右边界，移动左边界去适配右边界
        * 多数求和
            1. No.15 排序，遍历最大值，其余两值用2-pointer
            2. No.16 和No.15一样
            3. No.18 排序，遍历最大值和最小值，其余两值用2-pointer
            4. No.611 同No.15
    * 排序
        * 快速排序
            1. No.179 cmp(x, y)=-1 if str(x)+str(y)>str(y)+str(x) else 1
            2. No.274
            3. No.275 同No.274
            4. No.435 按end排序
            5. No.436 同No.435
            6. No.452 同No.435
            7. No.539
            8. No.593 排序之后各点关系就确定了
        * 堆排序
            1. No.215 堆的大小为215，计算最大值用最小堆
            2. No.347
            3. No.373
            4. No.692
        * 桶排序
            1. No.220 差不大于t，则桶的大小为t，和相邻的桶内元素比较即可
        * 计数排序
            1. No.75
    * 搜索
        * BFS
            1. No.102 层次遍历
            2. No.103 同No.102
            3. No.116 层次遍历
            4. No.117 同No.116
            5. No.127 按要求通过一系列转换从一个值变为另外一个值，可以将转换关系理解为图中的相连节点。
            6. No.130
            7. No.133 利用map存储新节点与对应源节点的映射，复制点与点之间的关系
            8. No.199
            9. No.200 计算有多少连通分量
            10. No.211
            11. No.222
            12. No.310 计算最长路径。从任一点a出发，找到离a最远的点b，再从b出发，找到离b最远的点c，搜索过程中记录下路径p。结果为p最中间的一个或两个点。
            13. No.331
            14. No.399 转换为图来做，先计算一个点到其他各个点的值，即分子相同，分母不同，在用除法计算出结果。
            15. No.417
            16. No.433
            17. No.449
            18. No.513
            19. No.515
            20. No.547
            21. No.623
            22. No.655
            23. No.662 使用数组存储完全二叉树中父节点与子节点的序号关系
        * DFS
            1. No.79
            2. No.94
            3. No.114 前序遍历
            4. No.113
            5. No.199
            6. No.230
            7. No.236 LCA问题
            8. No.310 计算最长路径。从任一点a出发，找到离a最远的点b，再从b出发，找到离b最远的点c，搜索过程中记录下b到c的路径p。结果为p最中间的一个或两个点。
            9. No.331
            10. No.332
            11. No.473
            12. No.494
            13. No.508
            14. No.638
            15. No.698
        * Backtracking
            1. No.91
            2. No.93
            3. No.95 遍历当前树的根节点，分别生成左子树和右子树
            4. No.96 同No.95
            5. No.98 分别校验左右子树，然后校验左子树的最大值和右子树的最小值
            6. No.241
            7. No.386
            8. No.416
            9. No.526
            10. No.553
    * 分治
        1. No.95 遍历当前树的根节点，分别生成左子树和右子树
        2. No.96 同No.95
        3. No.98 分别校验左右子树，然后校验左子树的最大值和右子树的最小值
        4. No.105 已知前序中序构造树
        5. No.106 已知中序后序构造树
        6. No.109 每次都平分左右子树
        7. No.131
        8. No.148 归并排序
        9. No.654
    * DP
        * 图DP
            * 路径数
                1. No.62
                2. No.63
            * 路径和
                1. No.64
                2. No.120 金字塔形结构，从底向上，逐层规约
        * 最长递增子序列(子串)
            1. No.300
            2. No.646
            3. No.673
        * 最长公共子序列(子串)
            1. No.583 转换为最长公共子序列来做。
            2. No.718 最长公共子串 DP[i][j]代表s1[:i],s2[:j]以s[i-1]和s[j-1]结尾的公共子串长度，DP[i][j]=D[i-1][j-1]+1 if s[i-1]==s[j-1] else 0
        * 最近公共祖先
            1. No.236
        * 0-1背包
            1. No.416
            2. No.474 两个维度上的0-1背包
        * 完全背包
            1. No.322
            2. No.518
            3. No.638
        * 树形DP
            1. No.337
        * 字符串编辑
            1. No.583 DP[i][j]代表word1[:i]和word2[:j]的最小删除次数，DP[i][j]=DP[i - 1][j - 1] if word1[i-1]==word2[j-1] else min(1 + DP[i - 1][j], 1 + DP[i][j - 1], 2 + DP[i - 1][j - 1])
            2. No.712 类似于No.583
        * 回文子序列(子串)
	        1. No.5
	        2. No.516
        * 整数分割
        * 字符串(数组)分割
            1. No.139
        * 状态机
            1. No.309 关键是初始值
            2. No.714 类似于No.309
        * 线性DP
            1. No.343 DP[i]代表n=i时的结果
            2. No.368 DP[i]代表以nums[i]结尾的序列，DP[i]=max([(*DP[j], n) for j in range(i - 1, -1, -1) if n % nums[j] == 0], key=lambda x: len(x), default=(n,)))
            3. No.376 要做两次DP，波动方向有两种
            4. No.377
            5. No.397 用递归自顶向下比较快
            6. No.486 DP[i][j]表示一名玩家在先手情况能从nums[i:j+1]数组中取得最大分数
        * 其他
		    1. No.152
		    2. No.213
		    3. No.221 DP数组中的DP[i][j]代表了以（i，j）为右下角的square的边长。所以当matrix[i][j]==1时，DP[i][j]=min(DP[i-1][j],DP[i][j-1],DP[i-1][j-1]),因为这三者中有一个为0时，matrix[i][j]并不能使某个square扩大。而这三者大于0，只能是其中最小值所在的square扩大。
		    4. No.264 丑数
		    5. No.279 满足条件的组合
            6. No.313 泛化丑数
            7. No.322
            8. No.375 DP[i][j]表示i...j的最优结果，有DP[i][j]=min(k+max(DP[i][k-1],DP[k+1][j] for k in range(i,j+1))) if j>i else 0
            9. No.395 如果出现次数最少的字符出现次数大于k则字符串符合条件，否则递归地以该字符分割字符串去做判断
            10. No.542 二维矩阵DP，先从左上角向右下角做DP，再反向做一次
            11. No.576 同时朝各个方向做BFS，每次都刷新矩阵
            12. No.688 同No.576
    * 数学
        * 素数
        * 多数投票
            1. No.229 典型投票问题
        * 相遇问题
        * 排列组合
            1. No.17 生成组合
            2. No.22 生成排列
            3. No.31 计算排列组合中的下一个
            4. No.39 生成组合求和
            5. No.40 同No.39
            6. No.46 排列
            7. No.47 排列
            8. No.60 计算排列组合中的任意一个。以n为第一位数排列组合有(n-1)！种，且第一位越大则这个排列越大，以此类推。类似于动态进制。
            9. No.62 可以理解为变形的排列组合问题，所有Right和Down排列之后去除相对顺序错误的那些组合。
            10. No.77 组合
            11. No.78 同No.77
            12. No.90 同No.78 
            13. No.216 组合
            14. No.357 不同的数即为首位不为0的组合数
            15. No.556 同No.31
        * 其他
            1. No.29 用减法模拟除法，用快速幂的方式加快速度
            2. No.50 快速幂
            3. No.166 模拟手工除法计算
            4. No.319 开关灯问题
            5. No.365 泊松分酒
            6. No.372 快速幂
            7. No.390 每次删数只关注第一个数字的变化即可
            8. No.396 F(k) = 0 * Bk[0] + 1 * Bk[1] + ... + (n-1) * Bk[n-1]，F(k+1) = Sum(Bk) - n * Bk[n-1]
            9. No.423 解方程
            10. No.462 把所有数字都变成**中位数**
            11. No.554 对每个wall做accumulate，统计出现频数
            12. No.640 模拟解方程
            13. No.670 总高位向地位遍历，如果某一位数字的低位有比它打的数，则这一位数字需要交互位置，要与低位中最大的且最低位的数字交换即可
            14. No.672 不太懂
    * 其他算法
        * 巧用hashmap
            1. No.454
            2. No.523 若sum(0...i)%k=n，有j>i，sum(0...j)%k=n，则可知sum(i+1...j)是k的倍数。此题中需要j>i+1。
            3. No.525 类似于523，若sum(0...i)=[x1, y1] (x1是0的个数，y1是1的个数)，若有j>i，sum(0...j)=[x2, y2]，且y2-x2=y1-x2，则可知sum(i+1...j)=[x, y]，其中x=y
            4. No.560 若sum(0...i)=n，有j>i，sum(0...j)-k=n，则可知sum(i+1...j)=k。
        * Manacher算法
            1. No.5
* 数据结构
    * 字符串
        * 普通字符串操作
            1. No.8
            2. No.13
            3. No.49
            4. No.89 G(n)=['0'+G(n-1), '1'+reversed(G(n-1))]
            5. No.151
            6. No.165
            7. No187 长度固定，用hashmap找重复即可
            8. No.299
            9. No.306
            10. No.318
        * 字符串模拟大数运算
            1. No.43 按四位进行分块，加快运行速度
    * 链表
        * 快慢指针
            1. No.19
            2. No.142 一个指针一次走两步，一个一次走一步。
        * 普通链表操作
            1. No.2：链表操作模拟加法
            2. No.24
            3. No.61
            4. No.92
            5. No.138
            6. No.147 插入排序
            7. No.148 归并排序
            8. No.328
            9. No.725 计算一下平均长度即可
    * 位操作
        1. No.137 只有一个数字出现n次，其余数字均出现m次，m>n。用多个二进制位表示一个二进制位出现的次数，计算出推导式即可。
        2. No.201 除了m和n高位相同的部分，其余都为0
        3. No.260 两个数出现奇数次，其余都为偶数次。逐个异或获得m，找到m中最右的1，其余位置0，获得n。将n再次与所有数以此做与，按结果是否为0分成两组做异或，即得结果。
        4. No.338 二进制技巧
        5. No.477 每一位的总hamming距离为`1的个数 * 0的个数`
    * 栈
        1. No.71
        2. No.143
        3. No.150 逆波兰式
        4. No.173
        5. No.227
        6. No.341
        7. No.385
        8. No.388
        9. No.394
        10. No.402 最后的结果是个递增(>=)序列
        11. No.445
        12. No.456
        13. No.503 `next greater element`类型的题目，`小技巧：数组可以循环，可以循环两倍的数组长度`
        14. No.636
    * 队列
        * 优先队列
            1. No.621 排队系列
    * 数组和矩阵
        * 普通数组和矩阵操作
            1. No.6
            2. No.36 分别校验行，列和块
            3. No.48 先将每列逆置，然后沿对角线做对称
            4. No.54 
            5. No.55
            6. No.56 按start排序
            7. No.59
            8. No.73
            9. No.74 从左下角或者右上角开始，类似于BST
            10. No.80
            11. No.82
            12. No.134 关键点在于如果车从i出发最远能到达j，那么从i到j出发都最远只能到达j，因为从i出发到达i+1至j中的任意一点时油量都>=0
            13. No.228
            14. No.238
            15. No.240 同No.74
            16. No.304 对每行做累和求差计算出范围的和
            17. No.307 累和求差计算出范围的和
            18. No.324
            19. No.334
            20. No.406 先按k排个序
            21. No.419 寻找每艘船唯一的特征点，如果一个点是1，且它的上方和左边都不是1，则这是一个特征点
            22. No.442 1. 将n放到nums[n-1]，如果nums[n-1]已经等于n了，那n出现了两次。 2. 用nums[n-1]的正负记录n是否出现过。
            23. No.457
            24. No.481
            25. No.491
            26. No.498
            27. No.529
    * 树
        * Trie树
            1. No.208
            2. No.211
            3. No.421
            4. No.648
            5. No.677
        * 前中后序遍历
            1. No.114 前序遍历
            2. No.144 先序遍历
            3. No.230 中序排列
            4. No.652 要对左右子树分组
        * 摘叶算法
            1. No.310
        * 其他
            1. No.450 删除BST的节点
    * 图
        * 并查集
            1. No.200 计算有多少连通分量
            2. No.547
            3. No.684
            4. No.721 有相同的email代表两个账号属于同一个人(即两个账号节点之间有)
        * 涂色算法
        * 拓扑排序
            1. No.207 前驱问题，典型的拓扑排序类问题
            2. No.210 同No.207
