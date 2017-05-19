# 引用类型

#### Object对象
    该对象用处不大，但是所有对象都由这个对象继承而来。
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
###### toFixed()
    返回指定位数小数的数字的字符串。四舍五入
###### toExponential()
    返回用科学计数法表示的数字的字符串形式。
###### toPrecision()
    返回最有意义的形式来返回数字的预定形式或指数形式。以最接近给定数的形式返回。
#### String
###### concat
    连接字符串
###### indexOf()和lastIndexOf()
    获取指定字符串在原字符串中的位置
    indexOf是第一个出现的位置
    lastIndexOf是最后一个出现的位置
###### localeCompare()
    按字母顺序排序比较,如果参数排在后面，则返回正数，如果相等，则返回0，如果参数排在后边，则返回负数。
###### slice()和subString();
    两者都是用来截取字符串，但是遇到负数时有所不同。
    slice()遇到负数相当于，字符串的长度加上参数
    subString()遇到负数相当于,参数为0



