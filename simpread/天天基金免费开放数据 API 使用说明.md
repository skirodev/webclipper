> 本文由 [简悦 SimpRead](http://ksria.com/simpread/) 转码， 原文地址 [blog.ops-coffee.cn](https://blog.ops-coffee.cn/t/eastmoney-fund-free-open-api.html)

实时涨跌
----

```
https://fundgz.1234567.com.cn/js/007345.js?v=20200908175500
```

数字为基金代码，rt 为时间戳

```
jsonpgz({
  "fundcode": "007345",
  "name": "瀵屽浗绉戞妧鍒涙柊鐏垫椿閰嶇疆娣峰悎",
  "jzrq": "2020-09-17",
  "dwjz": "1.9441",
  "gsz": "1.9717",
  "gszzl": "1.42",
  "gztime": "2020-09-18 15:00"
});
```

基金列表
----

```
http://fund.eastmoney.com/js/fundcode_search.js
```

返回数据

```
var r = [
  [
    "000001",
    "HXCZHH",
    "华夏成长混合",
    "混合型",
    "HUAXIACHENGZHANGHUNHE"
  ],
  [
    "000002",
    "HXCZHH",
    "华夏成长混合(后端)",
    "混合型",
    "HUAXIACHENGZHANGHUNHE"
  ]
]
```

基金详情
----

```
http://fund.eastmoney.com/pingzhongdata/007345.js?v=20200908175500
```

基金公司列表
------

```
http://fund.eastmoney.com/js/jjjz_gs.js
```

返回数据

```
var gs={
  op: [
    [
      "80163340",
      "安信基金"
    ],
    [
      "80036782",
      "招商基金"
    ]
  ]
}
```

基金净值数据
------

```
http://fund.eastmoney.com/f10/F10DataApi.aspx?type=lsjz&code=007345&page=1&per=20&sdate=2020-09-01&edate=2020-09-18
```

基金增幅排名
------

```
http://fund.eastmoney.com/data/rankhandler.aspx?op=ph&dt=kf&ft=gp&rs=&gs=0&sc=zzf&st=desc&sd=2016-03-29&ed=2017-03-29&qdii=&tabSubtype=,,,,,&pi=1&pn=50&dx=1&v=0.6370068000914493
```

ft： fund type 类型 所有 - all 股票型 - gp 混合型 - hh 债券型 - zq 指数型 - zs 保本型 - bb QDII-qdii LOF-lof

* * *

能看到这里一定是真爱，关注一下吧

![](https://blz.nosdn.127.net/sre/wx.sou1.png)