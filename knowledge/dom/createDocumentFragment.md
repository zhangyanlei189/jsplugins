### createDocumentFragment
* 创建代码片段


    var oFragment = document.createDocumentFragment();
    for(var i = 0 ; i < 10; i ++) {
        var p = document.createElement("p");
        var oTxt = document.createTextNode("段落" + i);
        p.appendChild(oTxt);
        oFragment.appendChild(p);<br>
    }
    document.body.appendChild(oFragment);

> 减少操作js操作dom的次数，提高性能