第六次测试
==========
## RGB街道 a
#### 题目描述
在RGB街道，从左往右右N个房子，现在你需要为每个房子涂上红、绿、蓝三种颜色之一，cost\[i\]\[1\]表示把第i个房子涂上红色的费用，cost\[i\]\[2\]表示把第i个房子涂上绿色的费用，cost\[i\]\[3\]表示把第i个房子涂上蓝色的费用。但任意相邻的两个房子的颜色都不能相同。  
你的任务是输出最小的总费用。
#### 输入格式
多组测试数据。
第一行，一个整数R(1 ≤ R ≤ 10)，表示有R组测试数据。
每组测试数据格式如下：
  * 第一行，一个整数N(1 ≤ N ≤ 20)。
  * 接下来有N行，第i行有三个正整数: cost\[i\]\[1\]、cost\[i\]\[2\]、cost\[i\]\[3\]，范围都不超过1000。

#### 输出格式
共R行。每行一个正整数，表示最小总费用。
#### 样例输入
	5
	3
	1 100 100
	100 1 100
	100 100 1
	3
	1 100 100
	100 100 100
	1 100 100
	3
	26 40 83
	49 60 57
	13 89 99
	6
	30 19 5
	64 77 64
	15 19 97
	4 71 57
	90 86 84
	93 32 91
	8
	71 39 44
	32 83 55
	51 37 63
	89 29 100
	83 58 11
	65 13 15
	47 25 29
	60 66 19
#### 样例输出
	3
	102
	96
	208
	253
## 打怪物 b
#### 题目描述
有N只怪物，第i只怪物的能量是blood[i]。你有一种攻击武器，称为“三连冲击波”，每使用一次这个攻击武器，它的杀伤力是这样的：
  1. 首先被冲击的那只怪物的能量会减少9。
  2. 其次被冲击的那只怪物的能量会减少3。（N>=2时有效）
  3. 最后被冲击的那只怪物的能量会减少1。（N=3时有效）

当某只怪物的能量为0或者低于0时，该怪物就会灭亡。你可以按照你的意愿来确定每一轮攻击中，怪物受到冲击的次序。你的任务是计算，至少要使用多少次攻击武器，才能消灭N只怪物？
#### 输入格式
第一行，一个整数R(1 ≤ R ≤ 10)，表示有R组测试数据。
每组测试数据格式如下：
  * 第一行，一个整数N(1 ≤ N ≤ 3)。  。
  * 第二行,有N个正整数: 第i个正整数是blood\[i\](1 ≤ blood[i] ≤ 60)。
  
#### 输出格式
共R行，每行一个整数。
#### 样例输入
	9
	3
	12 10 4 
	3
	54 18 6 
	3
	55 60 53 
	3
	1 1 1 
	2
	60 40 
	1
	60 
	1
	1 
	1
	60 
	1
	51 
#### 样例输出
	2
	6
	13
	1
	9
	7
	1
	7
	6
## 大会堂演奏厅 c
#### 题目描述
中国好声音歌手张某，要在大会堂演奏厅举行演唱会，他总共要唱N首歌。张某唱歌的特点是：
  1. 在唱每一首歌的过程中会保持相同的音量，即同一首歌的音量始终相等。
  2. 在唱每一首歌之前，他都会重新调整音量大小，在当前音量的基础上增加音量或者减少音量。

在演唱会开始之前，他初始化他的声线的音量大小是beginLevel。每一首歌都有一个调整值，第i首歌的调整值为change\[i\]，表示的意义是：不妨假设张某在唱第i首歌之前的音量是X，那么张某唱第i首歌的音量必须是X+change\[i\]或者是X-change\[i\]。
张某的高音极限是maxLevel，所以在演唱会过程中，所有歌曲的音量都不能超过maxLevel，当然所有歌曲的音量都不能小于0，等于0是允许的。
在满足上述条件的基础上，张某希望他在唱第N首歌过程中的音量越大越好，你的任务是输出该值。如果按照上述要求，张某根本无法唱第N首歌，那么输出-1。
#### 输入格式
多组测试数据。
第一行，一个整数R，表示有R组测试数据。 1 ≤ R ≤ 10。
每组测试数据格式如下：
  1. 第一行，三个整数：N(1 ≤ N ≤ 50),beginLevel(1 ≤ maxLevel ≤ 1000),maxLevel(0 ≤ beginLevel ≤ maxLevel)。
  2. 第二行,有N个正整数: 第i个正整数是change\[i\](1 ≤ change\[i\] ≤ maxLevel)。

#### 输出格式
共R行，每行一个整数。
#### 样例输入
	4
	3 5 10
	5 3 7 
	4 8 20
	15 2 9 10 
	14 40 243
	74 39 127 95 63 140 99 96 154 18 137 162 14 88
	8 516 668
	79 417 337 349 40 41 45 42
#### 样例输出
	10
	-1
	238
	334
