# 变量
#### 声明变量
    var test = 1;
    var test1 = 1,test2 = "a";
    与java不同，ES定义的变量不一定需要初始化(默认初始化为undefind),var test；也是有效的
    与java不同，ES定义变量可以保存不同的类型
    var t = "hi";
    alert(t);//hi
    t = 22;
    alert(t);//22
#### 命名变量
    变量名需要遵守两条简单规则：
    . 第一个字符必须是字母、下划线（_）或美元符号（$）
    . 余下的字符可以是下划线、美元符号或任何字母或数字字符
    var test;
    var $test;
    var $1;
    var _$te$t2;
    都是合法的
#### 变量的声明不是必须的
    ES的解释程序遇到未声明过的标识符时，用这个变量名创建一个全局变量，并将其初始化为指定的值。
#### 关键字
    break
    case
    catch
    continue
    default
    delete
    do
    else
    finally
    for
    function
    if
    in
    instanceof
    new
    return
    switch
    this
    throw
    try
    typeof
    var
    void
    while
    with
#### 保留字
    abstract
    boolean
    byte
    char
    class
    const
    debugger
    double
    enum
    export
    extends
    final
    float
    goto
    implements
    import
    int
    interface
    long
    native
    package
    private
    protected
    public
    short
    static
    super
    synchronized
    throws
    transient
    volatile
