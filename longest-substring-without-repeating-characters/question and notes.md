## question
给定一个字符串，请你找出其中不含有重复字符的 最长子串的长度。

## examples
输入: s = "abcabcbb"\
输出: 3 

输入: s = "bbbbb"\
输出: 1

输入: s = ""\
输出: 0

## notes
判断重复字符：使用C++哈希集合std::unordered_set可以降低空间复杂度
