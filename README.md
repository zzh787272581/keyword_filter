# keyword_filter
敏感词过滤研究

这里面列举了三种敏感词过滤算法
nomal 这种是最普通，全敏感词遍历匹配 效率最差

daf：其实就是简化了trie树，讲敏感词生成一颗trie数

trie：将敏感词生成一颗trie树，

后面两种比较高效，主要是在查找关键字的时候只需要遍历目标字符串即可，在查找时候时间复杂度在O(n)n=目标字符串长度

nomal的时间复杂度在O(m^n)m是关键字个数，n是目标字符串长度

============================测试数据===================

待检测语句字数：184
语句中包含敏感词的个数为：6。包含：
Array
(
    [0] => 饲养基地
    [1] => 自杀
    [2] => 法轮
    [3] => 红客联盟
    [4] => 手机卡复制器
    [5] => 三级片
)
总共消耗时间为：0.95295906066895ms
============================分割线===================
待检测语句字数：184
语句中包含敏感词的个数为：6。包含：
Array
(
    [0] => 红客联盟
    [1] => 自杀
    [2] => 轮功
    [3] => 饲养基地
    [4] => 手机卡复制器
    [5] => 三级片
)
总共消耗时间为：85.231065750122ms
============================分割线===================
待检测语句字数：184
语句中包含敏感词的个数为：7。包含：
Array
(
    [0] => 饲养基地
    [1] => 自杀
    [2] => 指南怀
    [3] => 法轮
    [4] => 红客联盟
    [5] => 手机卡复制器
    [6] => 三级片
)
总共消耗时间为：0.80704689025879ms


