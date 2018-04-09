### 项目简介
一个基于SpringCloud的微服务完整示例


### 服务规划简介

![](https://github.com/cse-sample/springcloud-2-cse/blob/master/springcloud-sample/images/design.png)

| 微服务工程名                     | 描述                     | 端口号     | 接口                          |
| ------------------------------- | ------------------------ | --------- | ----------------------------- |
| api-gateway-zuul                | 网关-API GateWay         | 8080      | /hello/xxx                    |
| config-server                   | 配置服务中心              | 7061      | /hello/xxx                    |
| config-client                   | 配置服务客户端            | 7092      | /profile                      |
| eureka-server                   | 服务注册中心              | 7071      | /hello/xxx                    |
| service-provider                | 服务提供者                | 7081,7082 | /hello/xxx                    |
| service-consume                 | 服务消费者                | 7091      | /consumer/hello-sync/xxx      |
| service-consume-ribbon          | 服务消费者-Ribbon         | 7092      | /ribbon/hello-sync/xxx        |
| service-consume-feign           | 服务消费者-Feign          | 7093      | /feign/hello-sync/xxx         |
| service-consume-ribbon-hystrix  | 服务消费者-Ribbon-Hystrix | 7094      | /ribbon-hystrix/hello-sync/xxx|
| service-consume-feign-hystrix   | 服务消费者-Feign-Hystrix  | 7095      | /feign-hystrix/hello-sync/xxx |