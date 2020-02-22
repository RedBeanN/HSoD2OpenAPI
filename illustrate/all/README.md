# illustrate/all

## 装备图鉴/获取全图鉴 [https://api.redbean.tech/illustrate/all?server=merged](https://api.redbean.tech/illustrate/all)

从 API 服务器获取所有图鉴

### query 参数

#### `server` - 服务器名

`Optional` 指定检索的服务器, 具体可用选项:

| server | 对应服务器 | 备注 |
| ------ | ---------- | ---- |
| merged `<default>` | 国测合并 | `默认` 国服和测试服合并, 优先使用国服数据 |
| original | 国服 | |
| beta | 测试服 | |
| fangcun | 东南亚服 | |
| jporiginal | 日服 | |

例: `https://api.redbean.tech/illustrate/all?server=jporiginal` 获取日服图鉴

未指定服务器或指定的服务器不存在时返回`merged`图鉴

具体返回内容请自行尝试
