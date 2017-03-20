# 引用类型

#### Object对象
    该兑现用处不大，但是所有对象都由这个对象继承而来。
###### Object对象具有下列属性
- constructor：对创建对象函数的引用（指针）。对于Object对象，该指针指向原始的Object()函数。
- Prototype：对该对象的对象原型的引用。对于所有的对象，它默认返回Object对象的一个实例。
###### Object对象具有下列方法
- hasOwnProperty(property):判断对象是否有某个特定的属性。必须用字符串指定该属性。

    对象私有属性为true，原型共有属性为false
- IsPrototypeOf(object):判断该对象是否为另一个对象的原型。
- PropertyIsEnumerable:判断给定的对象是否可以使用for..in..枚举

    这个属性必须是实例的，不是原型的

#### Boolean对象
    尽量使用Boolean的原始值，而不使用对象值。
    var a = new Boolean(false);
    console.log(a&&true);//true
> 此处应该返回false，实际却返回了true。因为a为对象，则使用&&时返回true。
    所以，不要使用对象类型的boolean值，而是应该使用原始类型值，直接定义a = false;

#### Number对象

