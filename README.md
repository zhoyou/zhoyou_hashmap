## 手写hashmap集合
## 知识点：
##  1. hashmap集合组成为：数组+链表+红黑树
![Image text](https://github.com/zhoyou/zhoyou-hashmap/raw/master/img/616953-20160304192851940-1880633940.png)  
HashMap原理。HashMap，就是为快而快的数据结构。。这里不得不说到最基本的线性表结构，数组和链表。。数组呢，查找啥的挺快，但是一到插入删除，就麻烦了，涉及到一波调换位置，全体前移或者后移。所以插入删除有些吃力，尤其是插入删除到前面的。。 那链表呢，，可以说是很好的解决了插入删除要全体动元素这个问题，但是随之而来的就是查找吃力，不是像数组那样一个i[n]就能很快的得知地址在哪里。。他得顺藤摸瓜慢慢捋。。有些吃力。所谓鱼与熊掌不可兼得。。但是他俩要是组合一下呢？各取所优？于是hashMap就是取各自的优点。。数组不是查找的快吗？那我就让你充当班级的角色，，链表不是添加删除无压力吗？我就让你的每个单元充当学生。。每当一个学生入校的时候，我就根据这个学生的特质，算出来它应属于哪个班级，得出来一个班级号，就是hash，，然后我就把它加到hash指定的班里面，假设hash是3，那就分到三班。。然后学生到三班报道，总得有个座位吧，，然而这些座位相当于链表的结构，，用链表的那一套给他得出来位置就行了，其实就是加个指针。  
##  2. hashcode地位https://blog.csdn.net/weixin_28774815/article/details/80640540  
##  3. hashmap与hashtable区别为  hashtable的put方法为线程安全方法，单一线程时使用hashmap多线程环境下推荐使用Correnthashmap

