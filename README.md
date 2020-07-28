# socket_p2p_connection

1. socket可以将应用层与运输层的TCP与UDP相连，与更底层的ICMP，IP与IGMP相连

  
    ![示意图](https://img-blog.csdnimg.cn/20190718154523875.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3Bhc2hhbmh1NjQwMg==,size_16,color_FFFFFF,t_70)
  
  2. 通过确定服务端与客户端以及它们之间的通信协议，就可以确定链接
  
  3. serverSocket.bind绑定端口
  
  4. serverSocket.listen
          
          允许连接失败次数，连接失败指代什么？ 
          
  5. serverSocket.accept
  
          等待客户端的连接，成功后返回代表这次连接的socket,以及客户端的地址，对IP协议来说就是(hostaddr, port)
          
  6. 阻塞的概念
          
          如果监听没有回应，该线程会暂停等候，而不会继续执行该进程下面的程序
          
  7. serverSocket.recv
  
          阻塞一直到接收到至少一个一比特数据或者远程端关闭（这个关闭的信息想必少于一比特）
          
8. 
