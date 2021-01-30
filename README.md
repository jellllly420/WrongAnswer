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
