# myqq
QQ robot python sdk
#### 安装：

```python
pip install myqq
```
#### 升级：

```python
 pip install --upgrade myqq
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

# 取QQ头像
qq_head_portrait(qq_number)

```
-----
-----

# 类型转换 
```pyhton
# python转换json
tool.python_to_json(content)

# json转换python
tool.json_to_python(content)



```



_____
_____
# 高级应用(支持所有官方api)
```python
bot = Send("http://localhost:8889/MyQQHTTPAPI", "666")
# 取好友列表
send = bot.div("Api_CreatQrCodeInfo", {"c1": 3414744631})
print(send)



# div自定义api
div("api名称", {'c1':"",'c2':""})






```

-----
-----
-----
-----
[API列表](https://myqqx.net/MyQQ/5.%E6%89%A9%E5%B1%95%E5%BC%80%E5%8F%91/5.API%E5%88%97%E8%A1%A8.html)








