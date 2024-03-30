# Computer-Fundamentals
> 记录学习计算机网络基础的知识点  
## DAY1
### 一、传输方式 <br>
#### 1.电路交换
01:建立连接(分配通信资源) >>> 02:通话(占用通信资源) >>> 03:释放连接(归还电信网) <br>
PS:计算机之间的数据传送是突发的，当使用电路交换传送计算机数据的话，线路传输的效率很低）

![image](https://github.com/zhihuishou/Computer-Fundamentals/assets/161868456/5a66b251-b342-4570-a829-19c879bdf038) <br>

#### 2.分组交换
互联网采取分组交换可以更有效的保证数据传输的效率，如下图所示。  
![image](https://github.com/zhihuishou/Computer-Fundamentals/assets/161868456/2f0e0c54-f762-4210-8180-18f19154f11c)
大致的分组交换方式：发送方（构造分组+发送分组）>>> 交换节点（缓存分组+转发分组）>>> 接收方（接收分组+还原报文）<br>

#### 3.报文交换
![image](https://github.com/zhihuishou/Computer-Fundamentals/assets/161868456/3e5bf829-e7eb-4001-bfe8-9133da0a0e3e)

### 二。计算机网络定义和分类
#### 1.定义  
计算机网络主要是有一些通用的、可编程的硬件互联而成，这些可编程硬件能够用来传送不同类型数据。  
可编程硬件（电脑、手机、CPU之类的） + 各类应用  
#### 2.分类
交换方式 >>> 使用者（公用网OR专用网）>>> 传输介质（有线+无线）>>> 覆盖范围（WAN + MAN LAN +PAN）>>> 拓扑结构（星型 + 环形 + 网状）

### 三、计算机网络性能指标
#### 1.速率
速率是指数据传送的速率（即每秒传送多少个比特），也成为数据率或者比特率。  
速率基本单位是比特/秒，也有千比特/秒，兆比特/秒等，常见的就是下载速率兆比特/秒。   
#### 2.带宽
某个信号所包含的的各种不同频率成分所占据的频率范围，用来表示网络的通信线路所能传送数据的能力，即单位时间内从网络中某个点到另一个店所能通过的最高数据率。  
单位：Hz（KHz，MHz，GHz）。  
#### 3.吞吐量
吞吐量就是下载速率和上传速率的综合，用于与实践网络的测量，以便获知多少数据量通过网络。  
#### 4.时延
也就是延迟，是指数据从网络一端到另外一端的时间，也就是为什么很多时候打游戏延迟，觉得卡，可能是发送时延和传播时延这边出现的问题。 

![image](https://github.com/zhihuishou/Computer-Fundamentals/assets/161868456/373b51a3-2411-4fe1-b910-5f4506e3a01c)
#### 5.时延带宽积

#### 6.往返时间
![image](https://github.com/zhihuishou/Computer-Fundamentals/assets/161868456/08c54d7a-f995-448c-835f-651716b314d8)

#### 7.利用率
链路利用率 + 网络利用率，当网络通信 量较少，产生的时延并不大，但在网络通信量不断增大时，分组在交换节点中排队时延就会增大，因此引发的时延就会增大。过高的网络利用率就会产生时延，因此大型的ISP会控制利用率，或者增大线路带宽。
![image](https://github.com/zhihuishou/Computer-Fundamentals/assets/161868456/a7d7e428-d0fd-42b1-a5a9-234c622a703b)

#### 8.丢包率
丢包率是指在一定时间范围内，传输过程汇总丢失的分组数量和总分组数量的比率。举个例子：当H1的主机给R1节点传输数据，但是数据中出现了数据丢包，产生了错误码，那么H2主机就检测到了丢弃误码的分组从而产生了丢包；又或者，可能某个节点的网络交换机达到了阈值，导致了数据无法进入节点。

![image](https://github.com/zhihuishou/Computer-Fundamentals/assets/161868456/a6e921c2-7af8-42f2-889f-9045cbca7282)

### 常见的三种计算机网络体系结构
#### 体系结构

TCP/IP参考模型  
![image](https://github.com/zhihuishou/Computer-Fundamentals/assets/161868456/7b7e16ee-8fbe-443c-97b8-3e5304cc9f1e)  

### 计算机网络体系结构分层思想
#### 思路：浏览器进程与WEB服务器进程基于网络的通信

![image](https://github.com/zhihuishou/Computer-Fundamentals/assets/161868456/06ffec83-0f0a-4d80-90f8-d094c829aefb)

## DAY2
### 物理层接口特性
![Uploading image.png…]()

