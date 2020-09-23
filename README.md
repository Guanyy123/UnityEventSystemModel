# UnityEventSystemModel
适用于Unity的消息转发模块，对脚本之间的调用进行解耦

#### 使用方法

1. 注册事件
EventCenter.AddListener<事件方法中的变量类型T>(EventDefine.<事件名称>, 事件方法方法);

2. 定义事件
public enum EventDefine
{
    事件名称,
}

3. 广播事件
EventCenter.BroadCast(EventDefine.<事件名称>);

4. 解绑事件
EventCenter.RemoveListener(EventDefine.<事件名称>, 事件方法方法);