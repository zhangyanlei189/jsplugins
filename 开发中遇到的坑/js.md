# 项目开发中遇到的坑

#### switch..case..
    判断条件为全等 ===  而不是 ==
    var a = "1";
    switch(a){
        case 1: console.log(1);break;
        case 2: console.log(2);break;
        default:console.log(3);
    }



####  arguments
    arguments是可以被修改的

[arguments](arguments.png)



