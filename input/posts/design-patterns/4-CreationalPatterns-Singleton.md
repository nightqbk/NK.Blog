Title: 创建型 - 单例 - Singleton
Published: 2019-10-14

Tags: ["Design Pattern","Creational Pattern "]
---
### 定义
保证一个类仅有一个实例，并提供一个访问它的全局访问点。

### 示例代码
GitHub: [Singleton](https://github.com/nightqbk/NK.DesignPattern/tree/master/NK.CreationalPatterns/NK.CreationalPatterns.Singleton)

### 分析

#### 1. 单例模式的两种实现方式

##### 1.1 懒汉式

##### 1.2 懒汉式 - double check locking

##### 1.3 饿汉试

#### 2. 单例模式的本质

单例模式的本质就是控制实例的数目

#### 3. 相关模式

很多模式都可以使用单例模式，只要这些模式中的某个类，需要控制实例为一个的时候，就可以很自然的用上单例模式。比如抽象工厂方法中的具体工厂类通常就是一个单例








