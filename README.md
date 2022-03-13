# myqq
QQ robot python sdk 


#### 安装：

```python
pip install myqq
```

-----
#### 创建你的第一个机器人
```python
# 导入库
from myqq import send
# 新建机器人
bot = send.Send("http://localhost:8889/MyQQHTTPAPI", "666")
# 取好友列表
f_list = bot.get_friend_list("123456789")
# 输出
print(f_list)

```
-----
-----

##### 发送消息
```python
# 导入库
from myqq import send
# 新建机器人
bot = send.Send("http://localhost:8889/MyQQHTTPAPI", "666")
# 发送消息
send = bot.send_msg("123456", "接受qq号码", "Hello world")
# 输出
print(f_list)

```









-----
-----
-----

# api

```python
# 发送消息
send_msg("机器人QQ号", "收信对象QQ", "内容")


# 发送消息
send_other_msg("机器人QQ号", "收信群_讨论组", "内容","信息类型")
"信息类型":[2群 3讨论组 4群临时会话 5讨论组临时会话 6在线临时会话]

# 取好友列表
get_friend_list("机器人QQ号")

# 取群管理
get_admin_list("机器人QQ号", "收信群_讨论组")

# 取群成员列表
get_group_member_list("机器人QQ号", "收信群_讨论组")

```











