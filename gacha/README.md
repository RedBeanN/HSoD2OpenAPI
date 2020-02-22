# API-gacha

## [https://api.redbean.tech/gacha/:pool](https://api.redbean.tech/gacha/high)

### 参数

#### `pool: String`

对应不同卡池

| pool | 对应蛋池 |
| ---- | ---- |
| high | 公主 |
| custom | 魔女 |
| special | 魔法少女 |
| middle | 大小姐 |

### 返回值

`Array[Object]` 一个包含 10 个对象的数组.

对象的键值:

| key | value | type |
| --- | ----- | ---- |
| title | 装备名 | String |
| isGod | 是否为神器 | Boolean |

例:

``` JSON
[
  { "title":"特勤作战服[4★]",       "isGod":false },
  { "title":"V制式试作型电锯[4★]",  "isGod":false },
  { "title":"手枪砖家(高段)[4★]",   "isGod":false },
  { "title":"克拉伦特[5★]",         "isGod":true  },
  { "title":"暴风雨[5★]",           "isGod":true  },
  { "title":"静籁永恒[5★]",         "isGod":true  },
  { "title":"雷电芽衣",             "isGod":true  },
  { "title":"V制式战斗服·骑士[4★]", "isGod":false },
  { "title":"V制式战斗服·骑士[3★]", "isGod":false },
  { "title":"V制式战斗服·强弩[4★]", "isGod":false }
]
```

蛋池未开放时会返回404
