项目教学地址https://blog.csdn.net/weixin_38007185/article/details/108119724
# springcloud-config
springcloud的配置中心

分组消费和持久化——重复消费问题（一条消息被多个消费者消费）
在RabbitMQ中，默认分组是不同的，组流水号不一样，被认为不同组

更方便的是，添加组名属性
spring:
  cloud:
    stream:
      bindings:
        input:
          group: A/B ## 分组名称
          
#链路跟踪
SpringCloud Sleuth负责对微服务调用链路的收集整理，而zipkin负责对链路的展现。
