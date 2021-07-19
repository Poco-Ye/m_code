```
le scan rsp 是用来回对端信息的

le这种东西，直接用nrf connect应用来解说

下拉扫描直接把所以广播都读进来，然后发scan req过去，收到对端的scan rsp之后

就可以解释出蓝牙广播名称，功率，还可以带uuid，
complete local name
tx power
uuid 
manufacturer data

所以目前设置的2009是给对端nrf connect扫描的


这个框架只是为了熟悉android bluetooth而已


```
