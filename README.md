WebFrameworkGrammar
===================

HBuilder的JS解析引擎能解析大多数JS框架，并直接给予提示。
但这种语法分析只能提示变量、方法的名字，无法提示类型、描述、示例、参数值域等更多内容。
更多内容的提示，有两种做法，JSDoc或SDocML语法库。

HBuilder支持开发者自助添加JS语法库框架。    
格式有2种
一种是SDocML，这是一种基于XML的通用语法描述格式，通过在HBuilder里对项目点右键-引入框架语法，来给项目导入框架语法库；
另一种是JSDoc+，基于扩展的JSDoc，可以给框架实现丰富的语法提示。使用时把带有jsdoc的js框架文件放入工程，即可实现提示。
JSDoc+的详细介绍见这里 http://ask.dcloud.net.cn/article/129
不管是SDocML还是JSDoc+，有很多共同的类型定义，比如如何提示图片列表，均参考上述JDDoc+的介绍。

DCloud Team已经完成以下框架的SDocML:
* JQuery 1.8
* JQuery 2.0
* zepto
* MUI
另外Ext框架其官方提供了一个ext-all-dev.js，里面包含有较全面的JSDoc，可以用于语法提示。我们也放在本目录下了。
注意这个JS文件体积高达6M，不要去编辑它，导入到工程里用于提示就好了，发布项目时再替换为普通的ext.js。

由于我们精力有限，而web框架多如繁星，我们自己无法制作更多框架的语法库。
我们欢迎和呼吁广大开发者行动起来，根据SDocML或JSDoc+的规范，制作更多框架语法库，并提交到这个git地址，给更多开发者造福。


===
> DCloud.io
> QQ群：326058616  
> 微博：@数字天堂网络  
> 微信公众号：DCloud   
