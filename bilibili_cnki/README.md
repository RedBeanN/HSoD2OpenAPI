# bilibili_cnki

## B站评论区查重

从 [AsoulCnki](https://github.com/ASoulCnki) 项目发展而来

检查小作文是否在B站评论区出现过, 数据库包含B站虚拟主播分区20万粉以上的vup及米哈游相关账号

## API

### [POST] https://api.redbean.tech/bilibili_cnki

**必须使用POST方法**

#### 请求体(JSON)

```json
{
    "text": "我好想做嘉然小姐的狗啊。\n可是嘉然小姐说她喜欢的是猫，我哭了。..."
}
```

text最小长度为30, 最大长度为1000

#### 返回内容

```json
{
    "code": 0,
    "message": "success",
    "error": null,
    "data": {
        "url": "https://t.bilibili.com/472642570902204872/#reply3866856390",
        "content": "我好想做嘉然小姐的狗啊。\n可是嘉然小姐说她喜欢的是猫，我哭了。...",
        "similarity": "100.00%",
        "name": "账号已注销299444",
        "id": "11192497",
        "timestamp": 1608885894000,
        "uname": "嘉然今天吃什么",
        "uid": "672328094"
    }
}
```

#### data 内容
|key|value|
|---|---|
|url|跳转到该评论的链接|
|content|原始小作文内容|
|similarity|查重率(百分比, 精确到2位小数)|
|name|评论作者的昵称|
|id|评论作者的ID|
|timestamp|评论的时间戳(ms)|
|uname|评论所属up主的昵称|
|uid|评论所属up主的ID|
