```
就是gradle的版本选择会比较麻烦，安装在用户目录比如插件选7.0.0 工具选7.0.2，这个版本需要匹配，jdk和sdk api比较好理解，
而且经常自己下载安装或者用sdk manager安装，gradle没有安装过

gradle的安装直接在android studio上选择更新安装，有了这四个东西就可以编译
version 有两个 一个是插件的 一个工具的
/c/Users/Administrator/.gradle/caches/jars-8/282efb23b4268a4d244ba955399ddc87/gradle-7.0.0.jar
/c/Users/Administrator/.gradle/wrapper/dists/gradle-7.0.2-bin/857tjihv64xamwrf0h14cai3r/gradle-7.0.2/bin
```
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
![image](./android%20studio%E7%89%88%E6%9C%AC%E9%97%AE%E9%A2%98.png)
