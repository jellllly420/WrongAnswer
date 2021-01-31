# 2021Winter
ShitHappens[doge]
# 集合求和
· 在所有子集中每个数出现总次数为2^(n-1)次  
· 数据长度需要采用long long int型
# 回文质数
· 偶数位的回文质数只有11  
· 偶数必不为质数  
· 生成回文数方法  
· 筛法（埃氏筛/线性筛）
# 玩具谜题
· 移动num[i]时可以整体移动num[i]后判断边界，不必移动num[i]次+判断num[i]次（or TLE）  
· 引用代码运用异或运算
# A + B Problem
· 为进位方便建议将字符数组存至数字数组中（内附代码）  
· 高精度
# A * B Problem & 阶乘之和
· 乘法进位细节  
> e.p. 3 * 123  
int arr[4]={0};  
for (int i = 0; i < 3(length of 123); i++) {  
    arr[i]+=3 * a[i];  
    arr[i+1]+=(arr[i]/10);  
    arr[i]%=10;  
}
# 两只塔姆沃斯牛 The Tamworth Two
· 内附代码对于判断是否相遇的问题采用了偷懒判断法（x
>这题没有什么坑点，主要问题是判断他们是否能够相遇。一种做法是在移动次数达到一定值时判定为无法相遇，但还有另一种思路：给每个状态设定一个值，如果这个值之前已经出现过，说明他们陷入了循环，不能相遇。每个状态都要保存农夫和牛的x、y坐标（各10种可能）和方向（各4种可能），其中为了避免重复，可以将特征值设为  
farmer.x + farmer.y * 10 + cow.x * 100 + cow.y * 1000 + farmer.facing * 10000 + cow.facing * 40000  
可以用bool数组来实现以O(1)的复杂度来查询该值是否已经出现。  
——beacon_cwk from www.luogu.com.cn/problem/solution/P1518
