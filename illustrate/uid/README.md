# illustrate/uid/:uid

## 装备图鉴/按 UID 查询

### 根据 UID 查询装备

仅支持查询国测合并(`merged`)图鉴

### 参数

#### `uid`

装备 uid , 注意 uid **不是** 游戏内的装备编号, 如果不清楚 uid 的来源请勿使用

### 返回值

`Object` 对应的装备, 不存在时返回`404`

### 例

`GET https://api.redbean.tech/illustrate/uid/1`

``` JSON
{"img":"1", "title":"M617左轮手枪", "desc":"能快速提升至五星，潜力巨大的装备", "rarity":"2", "cost":"2", "maxlv":"5", "uid":"1", "baseType":"手枪-速射", "id":"1", "damageBase":"12", "damageAdd":"2.25", "damageMaxLv":"21", "ammoBase":"80", "ammoAdd":"2.5", "ammoMaxLv":"90", "fireRateBase":"10", "fireRateAdd":"0", "fireRateMaxLv":"10", "countDownTimeBase":"0", "countDownTimeAdd":"0", "countDownTimeMaxLv":"0", "hpBase":"0", "hpAdd":"0", "hpMaxLv":"0", "criticalRate":"0.05", "multiShootLineNum":"0", "limitedNumber":"0", "damageType":"physic", "seriesId":1,"seriesText":"Start", "posterId":"0", "evolveFormula":{"input":[{"id":"111", "input":"1", "output":"2", "materials":["216", "229"],"inputEquip":"1", "outputEquip":"2"}],"output":[]}}
```
