# 《浅析URL》

##### URL是什么？

​	URL:uniform Resource Locator		统一资源定位符(网址)

#### 一、URL 包含哪几部分，每部分分别有什么作用？

​		

|       属性       |              作用               |
| :--------------: | :-----------------------------: |
|  Protocol(协议)  | 只有两种协议：http://和https:// |
|   Domin(域名)    |    表明正在请求哪个web服务器    |
|    Port(端口)    |    不同服务对应着不同的端口     |
|    Path(路径)    |     网络服务器上资源的路径      |
| Parameters(参数) |   提供给网络服务器的额外参数    |
|   Anchor(锚点)   |   帮助你快速翻到指定的那一页    |

#### 二、DNS 的作用是什么，nslookup 命令怎么用？

##### DNS是什么?

   + DNS: Domain Name System 域名系统/域名解析
   + 它作为可以将域名和IP地址相互映射的一个分布式数据库，能够使人更方便的访问互联网，而不用去记住能够被机器直接读取的IP数串。

		##### DNS作用

  + 将域名解析为IP 地址
  + 客户端向DNS服务器（DNS服务器有自己的IP地址）发送域名查询请求
  + DNS服务器告知客户机Web服务器的IP 地址
  + 客户机与Web 服务器通信

##### nslookup命令

nslookup命令用于互动式地查询域名记录

```bash
$ nslookup

> facebook.github.io
Server:     192.168.1.253
Address:    192.168.1.253#53

Non-authoritative answer:
facebook.github.io  canonical name = github.map.fastly.net.
Name:   github.map.fastly.net
Address: 103.245.222.133
>
```

#### 三、IP 的作用是什么，ping 命令怎么用？

##### IP是什么？

+ IP：Internet Protocol:因特网协议
+ 规定网络地址的协议，叫做IP协议。其本质就是提供互联网上唯一性标识，如果唯一性无法保证，互联网就彻底乱套了。
+ IP分两种：内网IP，外网IP

##### IP的作用

+ 定位一台计算机(为每一台计算机分配IP地址)
+ 封装数据报文，进行数据传输

##### ping命令

+ ping命令是用来探测本机与网络中另一主机之间是否可达的命令
+ 如果两台主机之间ping不通，则表明这两台主机不能建立起连接
+ ping是定位网络通不通的一个重要手段

#### 四、域名是什么，分别哪几类域名？

##### 什么是域名？

 + Domin Name 域名，域名是对ip的别称
 + 同一个域名可以对应不同的IP(均衡负载)
 + 同一个IP可以对应不同的域名(共享主机)

##### 域名的分类

1. 顶级域名

   + 国家顶级域名(national top-level domainnames)，例如中国是cn，美国是us，日本是jp等；

   + 国际顶级域名（international top-level domain names),
     + 表示工商企业.com
     + 表示网络提供商.net
     + 表示非盈利组织的.org
     + 其中全球注册量最大的新通用顶级域名包括.xyz、.top、.wang、.win、.club、.party等

2. 二级域名

   + 二级域名是指顶级域名之下的域名，在国际顶级域名下，它是指域名注册人的网上名称，例如 ibm，yahoo，microsoft等；
   + 在国家顶级域名下，它是表示注册企业类别的符号，例如com，edu，gov，net等。

3. 三级域名

   + 级域名用字母（ A～Z，a～z，大小写等）、数字（0～9）和连接符（－）组成，各级域名之间用实点（.）连接，三级域名的长度不能超过20个字符。

