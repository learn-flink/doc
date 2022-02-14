状态信息保存在TaskManager的最内存中，checkpoint的时候回将状态保存到指定的文件中（HDFS等文件系统）

* 缺点：   
状态大小受TaskManager内存限制（默认5M）

* 优点：
状态访问速度很宽，信息不会丢失。 
