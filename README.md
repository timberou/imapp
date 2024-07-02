# imapp-即时通讯应用Android客户端

支持Android 8 及以上

v0.2: 

    1.修复部分设备通过MediaDrm获取id出现UnsupportedSchemeException的错误

v0.3: 

    1.修复用户登录后接收到重复消息的bug、修改部分UI

v0.4: 

    1.Android客户端增加网络检测，亮屏检测与服务器的连接，断开后自动重连

    2.优化Android客户端的心跳机制，使用Alarm Manager控制心跳频率，不受电池优化（Doze）的干扰
  
    3.服务端增加消息确认逻辑，发送消息后客户端800ms内不回应确认被认为是离线状态并移除在线用户列表
  
    4.服务端根据cpu的核心数自动对发送消息的速度做出调整，避免并发引起的问题
