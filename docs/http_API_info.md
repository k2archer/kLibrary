# HTTP API 交互数据格式

#### API 接口 URL 格式（目前仅作样例）

前期暂使用 GET 请求，后期必须修改为 POST 请求。

```
http://api.xxx.com/service/v1.0/user/login
http://api.xxx.com/service/v1.0/user/register
http://api.xxx.com/service/v1.0/user/logout
http://api.xxx.com/service/v1.0/user/info/update
http://api.xxx.com/service/v1.0/album/upload
http://api.xxx.com/service/v1.0/album/update
http://api.xxx.com/service/v1.0/album/delete
```

#### 消息格式(json)

在 HTTP 请求的 Body 体使用 JSON 格式。

```
{
    "code":000
    "message":"example message"
    "result":"example result"
}
```

| 字段     | 类型    | 说明      | 字段  | 类型    | 说明   |
| -------- | ------ | -------- | ---- | ------ | ------ |
| code   | 整数    | 消息类型编码 | message | 字符串  | 消息体 |
| result | 字符串  | 响应结果 |      |        |        |

* code 编码定义
| 编号   | 说明      | 编号   | 说明     | 编号   | 说明       |
| ----- | --------- | ----- | ------- | ------ | --------- |
| 200   |操作成功     | 500  |操作失败   |||




