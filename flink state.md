flink state:
* key state
* operator state

* 托管状态： 由flink框架管理的状态
* 原始状态： 由用户自行管理的数据结构，框架在做checkpoint的时候，使用byte[] 来读写框架内容，对其内部数据结构一无所知。通常在DataStream上的状态推荐使用托管的状态，当实现一个自定义的operator时，会使用原始状态。其他时候一般不常用。
