##修改 input type=file 的样式
更改按钮输入框等样式都比较容易，

简单的CSS就可以完成

input上传file更改样式稍微复杂点

目前把默认的按钮不透明度设置opacity:0

下面放一个button按钮设置样式

我们看到的虽然是美化的button样式

实际上按下去的却是丑的一批的上传文件

## 纯CSS写的伪下拉菜单

先默认设置隐藏菜单

鼠标经过时显示伪菜单

##### 总结：还有几点没完成，没搞好，回头搞明白了再补上。

可输入的下拉框

三角形的下拉选择

复选框 单选框按钮的美化

 /*单选按钮*/

        [type="radio"] {
            display: none;
        }
            [type="radio"] + label {
                width: 20px;
                height: 20px;
                line-height: 20px;
                display: inline-block;
                text-align: center;
                vertical-align: bottom;
                border: 1px solid gray;
                border-radius: 50%;
            }

                [type="radio"] + label:hover {
                    border: 1px solid #2783FB;
                    cursor: pointer;
                }

            [type="radio"]:checked + label {
                background: #2783FB;
                border: 1px solid #2783FB;
            }

                [type="radio"]:checked + label:after {
                    content: "\2022";
                    font-size: 35px;
                    color: white;
                }