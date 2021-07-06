# zipkin 链路追踪学习
在分布式系统中，由于异步调用的存在，通过日志埋点的方式有时候解决线上问题不是很高效，zipkin可以追踪每次调用的过程。

## 使用方法
```docker run -d -p 9411:9411 openzipkin/zipkin```
运行zipkin；

```go run main.go```

```go run cli.go```

浏览器打开```http://127.0.0.1:9411/zipkin```就可以看到客户端调用服务端的流程