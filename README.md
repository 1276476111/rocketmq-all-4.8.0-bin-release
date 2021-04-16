# 官方的RocketMq。

### 此处搭建的是单机mq
### 使用的配置文件夹为 /rocketmq-all-4.8.0-bin-release/conf/2m-2s-sync

### 搭建mq步骤：
   #### 配置环境变量 ROCKETMQ_HOME 并重启电脑
 		先启动NameServer，然后再启动Broker；
		
   #### 切换到bin目录下：
   
	- 执行mqnamesrv.cmd 出现 The Name Server boot success. serializeType=JSON 则启动成功 （默认端口为9876）
	- 执行mqbroker -c ../conf/2m-2s-sync/broker-a-s.properties The broker[broker-a, 192.168.0.16:10921] boot success. serializeType=JSON and name server is 127.0.0.1:9876

   	`此处需要注意的是：启动broker时，需要指定配置文件。 否则mq控制台显示无集群`
      
     
