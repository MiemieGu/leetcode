# RMQ问题

RMQ(Range Minimum/Maximum Query)，即`区间极值问题`

## 解决方案

数据量比较小，我们可以暴力去解，数据量庞大，我们需要借助额外数据结构

我们有三种数据结构用于求解RMQ问题

- 树状数组
- ST表
- 线段树

## 应用场景

树状数组，用于区间求和问题，可以支持单点修改，区间修改，区间查询等操作

ST表，用于区间求极值问题（问题是可重复计算的）

线段树，用于区间极值，区间和等多种问题

## 复杂度

树状数组：O(NlogN)预处理，单次询问O(logN); 空间复杂度O(N)
ST表：O(NlogN)预处理，单次询问O(1); 空间复杂度O(NlogN)
线段树：O(N)预处理，单次询问O(logN); 空间复杂度O(N)