##.gwt.xml
是GWT的配置文件,是开发中必不可少的文件，功能类似Hibernate 的*.hbm.xml。
+ inherits 元素指定文件中有多个继承;
+ entry-point 元素指定有且只有一个入口,内容是EntryPoint实现类的全名;
+ source 元素指定多个资源。

##.java
实现前台的业务逻辑，将来它会编译成 JS 文件，该文件还是一个入口文件，在页面上引用的 JS 文件就是它编译的，这有点类似 java 中的 main 方法。

##web.xml
web.xml文件是用来初始化配置信息,定制初始化参数。

##index.html
运行项目首先加载的页面，从这个页面再加载其它文件

###问题
+ 操作了一整天还是不太了解整个项目是怎样运行的？
+ 在GwtTest项目中我实际操作了下删除index.html中的"<script type="text/javascript" language="javascript" src="test/test.nocache.js"></script>"，但是还是出现了"hello word"？
+ GwtTest项目中的test文件夹是怎么生成的？我尝试新建Maven项目但是没有test文件夹
