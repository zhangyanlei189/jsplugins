# 原始类型
    5种原始类型，Undefined,Null,Boolean,Number和String。
#### typeof
    typeof运算符有一个参数，即要检查的变量或值
    Undefined---->"undefined"
    String  ----->"string"
    Number  ----->"number"
    Boolean ----->"boolean"
    引用类型或者null ---->"object"
> null被认为是对象的占位符。typeof用于判断未声明的变量时，结果也是"undefined".

    var a;
    alert(typeof a);//"undefined"
    alert(typeof b);//"undefined"
    alert(c == undefined);//此处报错
> 即，未声明的变量除能使用typeof外，其他运算符均报错。
#### Undefined类型
    当声明的变量未初始化时，该变量的默认值是undefined。
    var oTemp；
    alert(opemp == undefined);//true
    当函数无明确返回值时，返回值也是"undefined"，
    function fn(){
    }
    alert(fn());
#### Null类型
    undefined是从null派生来的
    alert(null == undefined);//true
#### Boolean类型
    NUll        false
    ""          false
    " "         true
    Undefined   false
    0           false
    {}          true
    []          true
    NaN         false

#### Number类型
    ES中最特殊的类型，既可以表示32位的整数，还可以表示64位浮点数。
#### 浮点数
    浮点数必须包括小数点和小数点后的至少一位数字。这被看做浮点数的字面量。如：1.0
#### 特殊的Number值
    Number.MAX_VALUE        最大值
    Number.MIN_VALUE        最小值
    isFinite()              是否是有穷数值
    NaN                     not a number 一般发生在类型转换失败时。
                            NaN不与自身相等：
                            alert(NaN == NaN) //false

    isNaN()                 alert(isNaN('blue'));//true
                            alert(isNaN('1blue'));//true
                            alert(isNaN('blue1'));//true
                            alert(isNaN(5));//false
                            alert(isNaN("5"));//false
                            alert(isNaN(""));//false
                            alert(isNaN(" "));//false
#### String类型
    String是唯一没有固定大小的原始类型。可以用字符串存储0或更多的Unicode字符(有16位整数表示)
