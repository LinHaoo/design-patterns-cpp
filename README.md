## C++ 设计模式

掌握好设计模式是构建良好架构的基础。

### 创建型模式(Creational Patterns)

- [工厂方法模式] Factory Method, 被实例化的对象的子类
- [抽象工厂模式] Abstract Factory, 产品对象系列
- [单例模式] Singleton, 类的唯一实例
- [建造者模式] Builder, 复合对象是如何创建的
- [原型模式] Prototype, 被实例化的对象的类

### 结构型模式

- [适配器模式] Adapter, 对象的接口
- [装饰器模式] Decorator, 没有子类化的对象的责任
- [代理模式] Proxy, 如何访问对象(其位置)
- [外观模式] Facade, 子系统的接口
- [桥接模式] Bridge, 对象的实现
- [组合模式] Composite, 一个对象的结构和组成
- [享元模式] Flyweight, 对象的存储成本

### 行为型模式

- [策略模式] Strategy, 一种算法
- [模板方法模式] Template Method, 算法的步骤
- [观察者模式] Observer, 依赖对象如何保持最新
- [迭代器模式] Iterator, 如何访问聚合的元素
- [责任链模式] Chain of Responsibility, 可以满足请求的对象
- [命令模式] Command, 何时以及如何完成请求
- [备忘录模式] Memento, 什么私有信息存储在对象之外，何时存储
- [状态模式] State, 对象的状态
- [访问者模式] Visitor, 可以应用于对象而不改变其类的操作
- [中介者模式] Mediator, 对象如何以及哪些对象相互作用
- [解释器模式] Interpreter, 一种语言的语法和解释

### 六大原则

#### 1、开闭原则(Open Close Principle)

开闭原则就是说对扩展开放，对修改关闭。在程序需要进行拓展的时候，不能去修改原有的代码，实现一个热插拔的效果。所以一句话概括就是：为了使程序的扩展性好，易于维护和升级。想要达到这样的效果，我们需要使用接口和抽象类。

#### 2、里氏代换原则(Liskov Substitution Principle)

里氏代换原则(Liskov Substitution Principle LSP)面向对象设计的基本原则之一。 里氏代换原则中说，任何基类可以出现的地方，子类一定可以出现。 LSP是继承复用的基石，只有当衍生类可以替换掉基类，软件单位的功能不受到影响时，基类才能真正被复用，而衍生类也能够在基类的基础上增加新的行为。里氏代换原则是对“开-闭”原则的补充。实现“开-闭”原则的关键步骤就是抽象化。而基类与子类的继承关系就是抽象化的具体实现，所以里氏代换原则是对实现抽象化的具体步骤的规范。—— From Baidu 百科

#### 3、依赖倒置原则(Dependence Inversion Principle)

这个是开闭原则的基础，具体内容：真对接口编程，依赖于抽象而不依赖于具体。

#### 4、接口隔离原则(Interface Segregation Principle)

这个原则的意思是：使用多个隔离的接口，比使用单个接口要好。还是一个降低类之间的耦合度的意思，从这儿我们看出，其实设计模式就是一个软件的设计思想，从大型软件架构出发，为了升级和维护方便。所以上文中多次出现：降低依赖，降低耦合。

#### 5、迪米特法则(最少知道原则)(Demeter Principle)

为什么叫最少知道原则，就是说：一个实体应当尽量少的与其他实体之间发生相互作用，使得系统功能模块相对独立。

#### 6、单一职责原则(Single-Responsibility-Principle)

核心：一个类只负责一个功能领域中相应的职责，或者可以定义为：就一个类而言，应该只有一个引起它变化的原因。 

思想：如果一个类承担的职责过多，就等于把这些职责耦合在一起，一个职责的变化可能会削弱或者抑制这个类完成其他职责的能力。这种耦合会导致脆弱的设计，当变化发生时，设计会遭受到意想不到的破坏。

### 参考文献

* [Design Patterns in C++]
* [Wikipedia]

[Design Patterns in C++]: https://github.com/JakubVojvoda/design-patterns-cpp
[Wikipedia]: https://en.wikipedia.org/wiki/Software_design_pattern