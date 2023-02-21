[Back](../../README.md)

## CSL -> Service Management Block
>Service management block aims at managing the microservices both RESTful and RPC, also it has a message communication center to control all the async message communications based on the event driven architecture.

<hr>

### 1) Remote Service Center
>Remote service center is called mcp-rsc.

&nbsp;

### 2) Service Register Center

&nbsp;

### 3) Message Communication Center
>Message communication center is called mcp-mcc, it is the most important asynchronous component of micro-component platform. Developers can use it as the bridge to send messages or domain event via popular message middle-wares like apache kafka or rabbit mq etc.

##### 3-1) Send & Process Remote Event Demo

- 3-1-1) Start component services
    ```
    start mcp-mcc/mcp-event-producer [event message middle-ware]  8091
    start mcp-mcc/mcp-event-consumer [event message middle-ware]  8092
    ```

- 3-1-2) Start demo event sender and processor
    ```
    start mcp-ddd-cloud              [event sender]  8090
    start mcp-ddd-skeleton           [event processor]  8095
    ```

- 3-1-3) Event sender request
    [mcp-ddd-cloud]
    url: http://localhost:8090/test/emit-event 
    
    Request:
    ```
    {
    "appName": "MCP_MCC",
    "eventType": "REST",
    "moduleName": "test",
    "methodName": "processEvent",
    "payload": "{ \"a\": \"test a\", \"b\": \"test b\"}",
    "url": "http://localhost:8095/test/process-event"
    }
    ```

    Response:
    ```
    mcp-ddd-skeleton显示:
    2023-02-21 20:24:38.039 [http-nio-8095-exec-1] INFO  com.mcp.ddd.skeleton.api.controller.test.TestController -From remote call - method name: processEvent, payload: { "a": "test a", "b": "test b"}
    ```

&nbsp;




