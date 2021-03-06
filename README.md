# LinuxServerCodes
Linux高性能服务器编程源码

作者: 游双 

出版社: 机械工业出版社

出版年: 2013-5-1

ISBN: 9787111425199

* table of content:
《Linux高性能服务器编程》
前言
第一篇 TCP/IP协议详解
第1章 TCP/IP协议族 / 2
1.1 TCP/IP协议族体系结构以及主要协议 / 2
1.1.1 数据链路层 / 2
1.1.2 网络层 / 3
1.1.3 传输层 / 4
1.1.4 应用层 / 5
1.2 封装 / 6
1.3 分用 / 7
1.4 测试网络 / 8
1.5 ARP协议工作原理 / 9
1.5.1 以太网ARP请求/应答报文详解 / 9
1.5.2 ARP高速缓存的查看和修改 / 10
1.5.3 使用tcpdump观察ARP通信过程 / 10
1.6 DNS工作原理 / 12
1.6.1 DNS查询和应答报文详解 / 12
1.6.2 Linux下访问DNS服务 / 14
1.6.3 使用tcpdump观察DNS通信过程 / 15
1.7 socket和TCP/IP协议族的关系 / 16
第2章 IP协议详解 / 17
2.1 IP服务的特点 / 17
2.2 IPv4头部结构 / 18
2.2.1 IPv4头部结构 / 18
2.2.2 使用tcpdump观察IPv4头部结构 / 20
2.3 IP分片 / 21
2.4 IP路由 / 22
2.4.1 IP模块工作流程 / 23
2.4.2 路由机制 / 24
2.4.3 路由表更新 / 25
2.5 IP转发 / 25
2.6 重定向 / 26
2.6.1 ICMP重定向报文 / 26
2.6.2 主机重定向实例 / 27
2.7 IPv6头部结构 / 27
2.7.1 IPv6固定头部结构 / 28
2.7.2 IPv6扩展头部 / 29
第3章 TCP协议详解 / 30
3.1 TCP服务的特点 / 30
3.2 TCP头部结构 / 32
3.2.1 TCP固定头部结构 / 32
3.2.2 TCP头部选项 / 33
3.2.3 使用tcpdump观察TCP头部信息 / 35
3.3 TCP连接的建立和关闭 / 37
3.3.1 使用tcpdump观察TCP连接的建立和关闭 / 37
3.3.2 半关闭状态 / 39
3.3.3 连接超时 / 39
3.4 TCP状态转移 / 40
3.4.1 TCP状态转移总图 / 41
3.4.2 TIME_WAIT状态 / 43
3.5 复位报文段 / 44
3.5.1 访问不存在的端口 / 44
3.5.2 异常终止连接 / 45
3.5.3 处理半打开连接 / 45
3.6 TCP交互数据流 / 46
3.7 TCP成块数据流 / 48
3.8 带外数据 / 50
3.9 TCP超时重传 / 51
3.10 拥塞控制 / 53
3.10.1 拥塞控制概述 / 53
3.10.2 慢启动和拥塞避免 / 54
3.10.3 快速重传和快速恢复 / 55
第4章 TCP/IP通信案例：访问Internet上的Web服务器 / 57
4.1 实例总图 / 57
4.2 部署代理服务器 / 58
4.2.1 HTTP代理服务器的工作原理 / 58
4.2.2 部署squid代理服务器 / 59
4.3 使用tcpdump抓取传输数据包 / 60
4.4 访问DNS服务器 / 62
4.5 本地名称查询 / 63
4.6 HTTP通信 / 64
4.6.1 HTTP请求 / 65
4.6.2 HTTP应答 / 66
4.7 实例总结 / 68
第二篇 深入解析高性能服务器编程
第5章 Linux网络编程基础API / 70
5.1 socket地址API / 70
5.1.1 主机字节序和网络字节序 / 70
5.1.2 通用socket地址 / 71
5.1.3 专用socket地址 / 72
5.1.4 IP地址转换函数 / 73
5.2 创建socket / 74
5.3 命名socket / 75
5.4 监听socket / 76
5.5 接受连接 / 78
5.6 发起连接 / 80
5.7 关闭连接 / 80
5.8 数据读写 / 81
5.8.1 TCP数据读写 / 81
5.8.2 UDP数据读写 / 85
5.8.3 通用数据读写函数 / 86
5.9 带外标记 / 87
5.10 地址信息函数 / 87
5.11 socket选项 / 87
5.11.1 SO_REUSEADDR选项 / 89
5.11.2 SO_RCVBUF和SO_SNDBUF选项 / 89
5.11.3 SO_RCVLOWAT和SO_SNDLOWAT选项 / 93
5.11.4 SO_LINGER选项 / 93
5.12 网络信息API / 94
5.12.1 gethostbyname和gethostbyaddr / 94
5.12.2 getservbyname和getservbyport / 95
5.12.3 getaddrinfo / 96
5.12.4 getnameinfo / 98
第6章 高级I/O函数 / 100
6.1 pipe函数 / 100
6.2 dup函数和dup2函数 / 101
6.3 readv函数和writev函数 / 103
6.4 sendfile函数 / 106
6.5 mmap函数和munmap函数 / 107
6.6 splice函数 / 108
6.7 tee函数 / 110
6.8 fcntl函数 / 112
第7章 Linux服务器程序规范 / 114
7.1 日志 / 114
7.1.1 Linux系统日志 / 114
7.1.2 syslog函数 / 115
7.2 用户信息 / 116
7.2.1 UID、EUID、GID和EGID / 116
7.2.2 切换用户 / 117
7.3 进程间关系 / 118
7.3.1 进程组 / 118
7.3.2 会话 / 118
7.3.3 用ps命令查看进程关系 / 119
7.4 系统资源限制 / 119
7.5 改变工作目录和根目录 / 120
7.6 服务器程序后台化 / 121
第8章 高性能服务器程序框架 / 123
8.1 服务器模型 / 123
8.1.1 C/S模型 / 123
8.1.2 P2P模型 / 124
8.2 服务器编程框架 / 125
8.3 I/O模型 / 126
8.4 两种高效的事件处理模式 / 127
8.4.1 Reactor模式 / 128
8.4.2 Proactor模式 / 128
8.4.3 模拟Proactor模式 / 129
8.5 两种高效的并发模式 / 130
8.5.1 半同步/半异步模式 / 131
8.5.2 领导者/追随者模式 / 134
8.6 有限状态机 / 136
8.7 提高服务器性能的其他建议 / 144
8.7.1 池 / 144
8.7.2 数据复制 / 145
8.7.3 上下文切换和锁 / 145
第9章 I/O复用 / 146
9.1 select系统调用 / 146
9.1.1 select API / 146
9.1.2 文件描述符就绪条件 / 148
9.1.3 处理带外数据 / 148
9.2 poll系统调用 / 150
9.3 epoll系列系统调用 / 151
9.3.1 内核事件表 / 151
9.3.2 epoll_wait函数 / 152
9.3.3 LT和ET模式 / 153
9.3.4 EPOLLONESHOT事件 / 157
9.4 三组I/O复用函数的比较 / 161
9.5 I/O复用的高级应用一：非阻塞connect / 162
9.6 I/O复用的高级应用二：聊天室程序 / 165
9.6.1 客户端 / 165
9.6.2 服务器 / 167
9.7 I/O复用的高级应用三：同时处理TCP和UDP服务 / 171
9.8 超级服务xinetd / 175
9.8.1 xinetd配置文件 / 175
9.8.2 xinetd工作流程 / 176
第10章 信号 / 178
10.1 Linux信号概述 / 178
10.1.1 发送信号 / 178
10.1.2 信号处理方式 / 179
10.1.3 Linux信号 / 179
10.1.4 中断系统调用 / 181
10.2 信号函数 / 181
10.2.1 signal系统调用 / 181
10.2.2 sigaction系统调用 / 181
10.3 信号集 / 182
10.3.1 信号集函数 / 182
10.3.2 进程信号掩码 / 183
10.3.3 被挂起的信号 / 183
10.4 统一事件源 / 184
10.5 网络编程相关信号 / 188
10.5.1 SIGHUP / 188
10.5.2 SIGPIPE / 189
10.5.3 SIGURG / 190
第11章 定时器 / 193
11.1 socket选项SO_RCVTIMEO和SO_SNDTIMEO / 193
11.2 SIGALRM信号 / 195
11.2.1 基于升序链表的定时器 / 195
11.2.2 处理非活动连接 / 200
11.3 I/O复用系统调用的超时参数 / 205
11.4 高性能定时器 / 206
11.4.1 时间轮 / 206
11.4.2 时间堆 / 211
第12章 高性能I/O框架库Libevent / 218
12.1 I/O框架库概述 / 218
12.2 Libevent源码分析 / 220
12.2.1 一个实例 / 220
12.2.2 源代码组织结构 / 222
12.2.3 event结构体 / 224
12.2.4 往注册事件队列中添加事件处理器 / 226
12.2.5 往事件多路分发器中注册事件 / 230
12.2.6 eventop结构体 / 233
12.2.7 event_base结构体 / 235
12.2.8 事件循环 / 236
第13章 多进程编程 / 239
13.1 fork系统调用 / 239
13.2 exec系列系统调用 / 240
13.3 处理僵尸进程 / 240
13.4 管道 / 241
13.5 信号量 / 243
13.5.1 信号量原语 / 243
13.5.2 semget系统调用 / 244
13.5.3 semop系统调用 / 245
13.5.4 semctl系统调用 / 247
13.5.5 特殊键值IPC_PRIVATE / 249
13.6 共享内存 / 251
13.6.1 shmget系统调用 / 251
13.6.2 shmat和shmdt系统调用 / 252
13.6.3 shmctl系统调用 / 253
13.6.4 共享内存的POSIX方法 / 254
13.6.5 共享内存实例 / 254
13.7 消息队列 / 263
13.7.1 msgget系统调用 / 263
13.7.2 msgsnd系统调用 / 264
13.7.3 msgrcv系统调用 / 264
13.7.4 msgctl系统调用 / 265
13.8 IPC命令 / 266
13.9 在进程间传递文件描述符 / 267
第14章 多线程编程 / 269
14.1 Linux线程概述 / 269
14.1.1 线程模型 / 269
14.1.2 Linux线程库 / 270
14.2 创建线程和结束线程 / 271
14.3 线程属性 / 273
14.4 POSIX信号量 / 275
14.5 互斥锁 / 276
14.5.1 互斥锁基础API / 276
14.5.2 互斥锁属性 / 277
14.5.3 死锁举例 / 278
14.6 条件变量 / 279
14.7 线程同步机制包装类 / 280
14.8 多线程环境 / 282
14.8.1 可重入函数 / 282
14.8.2 线程和进程 / 283
14.8.3 线程和信号 / 284
第15章 进程池和线程池 / 287
15.1 进程池和线程池概述 / 287
15.2 处理多客户 / 288
15.3 半同步/半异步进程池实现 / 289
15.4 用进程池实现的简单CGI服务器 / 298
15.5 半同步/半反应堆线程池实现 / 301
15.6 用线程池实现的简单Web服务器 / 304
15.6.1 http_conn类 / 304
15.6.2 main函数 / 318
第三篇 高性能服务器优化与监测
第16章 服务器调制、调试和测试 / 324
16.1 最大文件描述符数 / 324
16.2 调整内核参数 / 325
16.2.1 /proc/sys/fs目录下的部分文件 / 325
16.2.2 /proc/sys/net目录下的部分文件 / 325
16.3 gdb调试 / 326
16.3.1 用gdb调试多进程程序 / 326
16.3.2 用gdb调试多线程程序 / 328
16.4 压力测试 / 329
第17章 系统监测工具 / 333
17.1 tcpdump / 333
17.2 lsof / 334
17.3 nc / 336
17.4 strace / 338
17.5 netstat / 341
17.6 vmstat / 342
17.7 ifstat / 344
17.8 mpstat / 344
参考文献 / 346 
