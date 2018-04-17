# 多线程

1、Java实现多线程的方式及三种方式的区别。

2、什么是多线程，什么是线程安全？

3、多线程如何进行交互？wait、notify、notifyAll有什么区别？

4、多线程共用一个数据变量需要注意什么？

5、什么是线程池？如何设计一个线程池？

java.util.concurrent.Executosr是线程池的静态工厂，我们通常使用它方便地生产各种类型的线程池，主要的方法有三种：
1、newSingleThreadExecutor()——创建一个单线程的线程池
2、newFixedThreadPool(int n)——创建一个固定大小的线程池
3、newCachedThreadPool()——创建一个可缓存的线程池

6、线程池的使用时的注意事项。

7、concurrect包下面，都有用什么？

8、volatile关键字如何保证内存可见性？

9、sleep和wait方法分别是什么类的方法，有什么区别？
	* Thread.sleep和Object.wait
	* sleep()睡眠时，保持对象锁，仍然占有该锁；而wait()睡眠时，释放对象锁。

10、synchronized和lock的区别，使用场景。

11、synchronized底层如何实现？用在代码块和方法上有什么区别？

12、Synchronize关键字为什么jdk1.5后效率提高了？

13、现在有一个进程挂起了，如何用工具查出原因？

14、怎么解决缓存和主存的一致性问题。

15、什么是锁，什么是乐观锁、悲观锁。

16、CAS的原理。

17、线程状态转移图。