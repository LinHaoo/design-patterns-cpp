## 备忘录模式

Memento在不违反封装的情况下，捕获并具体化一个对象的内部状态，以便该对象可以在以后恢复到这个状态。模式有行为目的，并应用于对象。

### 何时使用

* 必须保存对象状态的快照，以便以后可以恢复到该状态
* 获取状态的直接接口会暴露实现细节并破坏对象的封装