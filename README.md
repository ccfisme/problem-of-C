之前学C语言时，总感觉定义一个数组（如int a[100000]）做题根本用不了这么大的空间，感觉是一种浪费，想用int a[n]的方式来动态定义数组，但是语法不支持，所以后来通过查找发现还有malloc这种函数来动态申请空间，用法是</br>
![截屏2021-09-29 00 07 15](https://user-images.githubusercontent.com/74129445/135126174-cd4c5596-300d-4426-a025-13abf3bf5b91.png)</br>
参考：https://mp.weixin.qq.com/s?__biz=MzAxMDQwMzU4Mg==&mid=2247484055&idx=1&sn=7b650d73481e3a2053d4ff8ba22c599f&chksm=9b51a906ac262010c29630cae99a48ead4f097ceb54c963d9477cdb88e77e0553b077f431e9e&scene=21%23wechat_redirect</br>
这里出现了free，不理解为什么出现，经过查找发现是因为内存空间小，而malloc函数的空间有可能比较大且只用一次，会造成空间不足，也就是内存泄漏，故用完malloc要记得释放之前的内存</br>
![截屏2021-09-28 23 57 50](https://user-images.githubusercontent.com/74129445/135126519-8e4619ce-c937-41bc-92fe-99f1c03aa7ca.png)</br>
![截屏2021-09-29 00 22 40](https://user-images.githubusercontent.com/74129445/135126980-10a35943-5bd1-43f9-b966-b3f65f580eeb.png)</br>
参考：https://zhuanlan.zhihu.com/p/105126066</br>

