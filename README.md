# LV-0

### 实时通讯

> 基于js 做前端，php做后端，nginx做web服务器

#### 具体流程

1. 网页的前端是用js写（copy）的后面打算改成php
2. 网页的nginx基本都是自己写的，实现是用一个服务监听8010端口，当监听到请求后通过更改消息，然后转发给8020端口
3. 后端的server.php服务（copy）连接在本地的8020端口，当收到消息后就可以进行通讯

#### 实现过程

1. 能够正常完成websocket的连接，能够实现基本的功能
2. nginx能后顺利完成服务的转发（虽然只有一个localhost）

#### 不足点

1. 实时通讯并不实时，而且是服务端和多个客户端的通讯，当服务端卡住的时候，整个服务就会卡住。
2. 前端不具有实用性。
3. nginx的服务需要另外监听一个端口，希望能直接在80端口中实现服务代理。
4. 个别代码后面会改成原创的

