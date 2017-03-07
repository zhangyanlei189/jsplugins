## callee
    arguments的属性，值就是所属的函数本身
    递归时，可以用于替换当前的匿名函数，避免全局的fn变量污染
    var fn = function(){
        arguments.callee();//当前的fn函数
    }
## caller
    获取哪个对象或函数调用了当前函数