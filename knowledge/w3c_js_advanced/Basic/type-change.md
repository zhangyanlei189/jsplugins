# 类型转换

#### 转换成字符串
    数字类型-->String：默认模式和基模式
    默认模式：toString(),字面表示，即十进制
    基模式：  toString(2),二进制字符串
             toString(8);八进制字符串
#### 转换成数字
    转数字：parseInt(),parseFloat();
    只有String类型调用这些方法才能正常运行。其他类型返回的都是NaN;
#### 强制类型转换
    3种强制类型转换
    Boolean：把给定的值转换成Boolean值
    Number：把给定的值转换为数字
    String：把给定的值转换成字符串
###### Boolean函数
    当要转换的值是至少有一个字符的字符串、非 0 数字或对象时，Boolean() 函数将返回 true。
    如果该值是空字符串、数字 0、undefined 或 null，它将返回 false。
###### Number函数
    Number是整体转换，不是部分转换，与parseFloat()和parseInt()不同。
    parseInt("1a");//1    Number("1a");//NaN

    Number(false)           0;
    Number(true)            1;
    Number(undefined)       NaN;
    Number(null)            0;
    Number("1.2")           1.2;
    Number("12")            12;
    Number("1.2.3")         NaN;
    Number(new Object())    NaN;
    Number(50)            50;
###### String函数
    与toString()函数的区别，String()可以转换null,undefined；
    String(null); //null
    String(undefined); //undefined
    var a = null;a.toString();  //解析错误
    













