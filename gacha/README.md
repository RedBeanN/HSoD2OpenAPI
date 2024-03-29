# gacha

## 十连扭蛋接口 [https://api.redbean.tech/gacha/:pool[?count=10]](https://api.redbean.tech/gacha/high)

### 参数

#### `pool<String>`

对应不同卡池

| pool | 对应蛋池 |
| ---- | ---- |
| high | 公主 |
| custom | 魔女 |
| special | 魔法少女 |
| middle | 大小姐 |

#### `count<Number>` (可选)

扭蛋次数, 默认10, 最小1, 最大100

### 返回值

`Array[Object]` 一个包含 `count` 个对象的数组.

对象的键值:

| key | value | type |
| --- | ----- | ---- |
| title | 装备名 | String |
| isGod | 是否为神器 | Boolean |

蛋池未开放、不存在或未指定时会返回`404`

### 例

`GET https://api.redbean.tech/gacha/high?count=10`

``` JSON
[
  {
    "title":"特勤作战服[4★]",
    "isGod":false
  }, {
    "title":"V制式试作型电锯[4★]",
    "isGod":false
  }, {
    "title":"手枪砖家(高段)[4★]",
    "isGod":false
  }, {
    "title":"克拉伦特[5★]",
    "isGod":true
  }, {
    "title":"暴风雨[5★]",
    "isGod":true
  }, {
    "title":"静籁永恒[5★]",
    "isGod":true
  }, {
    "title":"雷电芽衣",
    "isGod":true
  }, {
    "title":"V制式战斗服·骑士[4★]",
    "isGod":false
  }, {
    "title":"V制式战斗服·骑士[3★]",
    "isGod":false
  }, {
    "title":"V制式战斗服·强弩[4★]",
    "isGod":false
  }
]
```
