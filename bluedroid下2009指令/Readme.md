```
le scan rsp 是用来回对端信息的

le这种东西，直接用nrf connect应用来解说

下拉扫描直接把所有广播都读进来，然后发scan req过去，收到对端的scan rsp之后

就可以解释出蓝牙广播名称，功率，还可以带uuid，
complete local name
tx power
uuid 
manufacturer data

所以目前设置的2009是给对端nrf connect扫描的


这个框架只是为了熟悉android bluetooth而已


```
```
第一步是2009指令的函数回溯
```
![image](https://github.com/Poco-Ye/m_code/blob/master/bluedroid%E4%B8%8B2009%E6%8C%87%E4%BB%A4/1.png)
```
第二步是通过event来选择跑哪个cmd，枚举cmd，枚举event，对应起来，然后用event调用对应的cmd
bluedroid的第一层是BTM,这部分的接口是dm action，封装第一层。通过send message的异步方式去调用接口
```
![image](https://github.com/Poco-Ye/m_code/blob/master/bluedroid%E4%B8%8B2009%E6%8C%87%E4%BB%A4/2.png)
```
第三步
```
![image](https://github.com/Poco-Ye/m_code/blob/master/bluedroid%E4%B8%8B2009%E6%8C%87%E4%BB%A4/3.png)
```
第四步
```
![image](https://github.com/Poco-Ye/m_code/blob/master/bluedroid%E4%B8%8B2009%E6%8C%87%E4%BB%A4/4.png)

