```
不喜欢用ui的工具，很多android 的应用因为图中的各种工具版本不匹配然后编译不过

gradle version
java  version
andorid sdk version

android sdk version一开始就可以识别然后android studio去下对应的SDK API
java  version这个根据内部配置的生成.idea，比如下载比较新的studio 自带的就是java 11的jdk
gradle根据上面配的去下载生成.gradle 看图中配置的是4.4


这个图的配置就会编译不过，会提示4.4的gradle不匹配jdk 11

一般的解决方法都是降jdk版本，直接下载安装再从新选路径，.idea的misc.xml会更改jdk版本

```
![image](https://github.com/Poco-Ye/m_code/blob/master/android%20studio%E7%89%88%E6%9C%AC%E9%97%AE%E9%A2%98/android%20studio%E7%89%88%E6%9C%AC%E9%97%AE%E9%A2%98.png)
