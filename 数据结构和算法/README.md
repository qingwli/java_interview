# 数据结构与算法

* 1、栈。后进先出；顺序栈、链式栈的底层实现；栈的应用：符号匹配。中缀转后缀、后缀求值。标签匹配。网页浏览器中已访问页面的历史记录。
http://blog.csdn.net/javazejian/article/details/53362993

* 2、队列。

1、HashMap和HashTable的区别，HashMap的key可以是任何对象或者数据类型吗？
* HashTable是线程安全的。HashMap是线程不安全的。
* HashTable不可以存储null值，HashMap可以存储null值。key和value都可以）
* HashTable和HashMap都能通过values()方法返回一个Collection，然后进行遍历处理。两者都可以通过entrySet()方法返回一个Set然后进行遍历处理。
* HashTable使用Enumeration，HashMap使用Iterator。
* HashTable直接使用对象的hashCode，HashMap重新计算hash值，而且用于代替求模。
* HashTable基于Dictionary类，HashMap基于AbstractMap类。

* HashMap的key可以为null但不能是可变对象，如果是可变对象的话，改变对象的属性，则对应的HashCode也进行相应的改变，否则下次无法找到已经存在Map的值。如果是可变对象的话，要保证对象成员变量改变的时候不能改变哈希值。

* HashTable是线程安全的。 是在对应的方法上添加了synchronized关键字进行修饰。执行较慢，推荐使用ConcurrectHashMap，使用的分段锁。

2、Map中有哪些类？哪些是线程安全的？如何实现的线程安全？

LinkedHashMap、HashMap、HashTable、TreeMap。

4、了解Java collection类，集合框架。

https://www.lqwang.net/595.html

5、HashMap和ConcurrectHashMap的区别？如何实现线程安全？
* HashMap是线程不安全的。ConcurrectHashMap是线程安全的。

6、HashMap的原理、Hashmap为什么大小是2的幂次。

7、二叉树的分类。

满二叉树（除最后一层无任何子节点外，每一层上的所有结点都有两个子结点二叉树）
完全二叉树（一棵二叉树至多只有最下面的一层上的结点的度数可以小于2，并且最下层上的结点都集中在该层最左边的若干位置上，则此二叉树成为完全二叉树）
平衡二叉树（它是一棵空树或它的左右两个子树的高度差的绝对值不超过1，并且左右两个子树都是一棵平衡二叉树）
二叉搜索树（它或者是一棵空树，或者是具有下列性质的二叉树： 若它的左子树不空，则左子树上所有结点的值均小于它的根结点的值； 若它的右子树不空，则右子树上所有结点的值均大于它的根结点的值；它的左、右子树也分别为二叉排序树）
红黑树（平衡二叉搜索树）
哈弗曼树（给定n个权值作为n个叶子结点，构造一棵二叉树，若带权路径长度达到最小，称这样的二叉树为最优二叉树，也称为哈夫曼树(Huffman Tree)。哈夫曼树是带权路径长度最短的树，权值较大的结点离根较近）

7、Hashmap中jdk1.8之后做了哪些优化？

8、因为别人知道源码如何思想的，故意构造相同的hash的字符串进行攻击，如何处理？jdk7如何处理？

9、常见的hash算法有哪些？

10、快排的思想、过程、复杂度。什么时候适用，什么时候不适用？

11、什么是排序的稳定性？

12、常见的排序哪些是稳定的，哪些是不稳定的？

13、各中排序的原理。

14、二分搜索的过程。

15、一万个数中如何找到重复的数字？

16、一个数组中如何找到和为k的两个数？

17、十万数中找到最小或最大的十个。

18、加密解密的算法思想。

19、Arraylist的原理，Arraylist的扩容机制，为什么扩容是1.5倍？

20、B树，B+树，红黑树。

21、平衡二叉树。

22、一千万用户并发抢购，怎么设计，如果成功的用户有10万，redis存不下怎么处理？

23、如何用HashMap实现LinkedMap。

24、队列的实现和应用。

hash负载均衡 redis设计与实现