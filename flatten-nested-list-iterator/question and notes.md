## question
给你一个嵌套的整型列表。请你设计一个迭代器，使其能够遍历这个整型列表中的所有整数。

列表中的每一项或者为一个整数，或者是另一个列表。其中列表的元素也可能是整数或是其他列表。

## examples
输入: [[1,1],2,[1,1]]\
输出: [1,1,2,1,1]\
解释: 通过重复调用 next 直到 hasNext 返回 false，next 返回的元素的顺序应该是: [1,1,2,1,1]。

输入: [1,[4,[6]]]\
输出: [1,4,6]\
解释: 通过重复调用 next 直到 hasNext 返回 false，next 返回的元素的顺序应该是: [1,4,6]。

## notes
Java iterator:\
Iterator 是为了实现对java容器(collection)进行遍历功能的1个接口。\
Iterator最主要的方法为hasNext()和Next()，用于让各种容器去重写，实现遍历。\
Java容器具有iterator()方法，\
例子：\
    代码：\
    HashSet hs = new HashSet();\
    hs.add(new Student(1,"Jack"));\
    hs.add(new Student(2,"Bill"));\
    hs.add(new Student(3,"Alice"));\
    hs.add(new Student(4,"Cici"));\
    Student st;\
    Iterator it = hs.iterator();  \
    while (it.hasNext()){\
        st = (Student)(it.next());\
        System.out.println(st);\
    }\
    输出：\
    [java] 2:Bill\
    [java] 1:Jack\
    [java] 4:Cici\
    [java] 3:Alice\

