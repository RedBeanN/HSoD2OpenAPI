# illustrate/title/:title

## 装备图鉴/按装备名查询

### 根据装备名查询装备

仅支持查询国测合并(`merged`)图鉴

### 参数

#### `title`

装备名, 必须是全名, 暂不支持模糊查询

### 返回值

`Array[Object]` 对应的装备数组, 可能包含多个装备, 按 uid 排序

### 例

`GET https://api.redbean.tech/illustrate/title/犹大的誓约`

``` JSON
[{"img":"838", "title":"犹大的誓约", "desc":"", "rarity":"5", "cost":"15", "maxlv":"50", "uid":"371", "baseType":"放置-远古兵器", "id":"827", "damageBase":"480", "damageAdd":"15.673", "damageMaxLv":"1247", "ammoBase":"3", "ammoAdd":"0.082", "ammoMaxLv":"7", "fireRateBase":"3.3", "fireRateAdd":"0", "fireRateMaxLv":"3.3", "countDownTimeBase":"4", "countDownTimeAdd":"0", "countDownTimeMaxLv":"4", "hpBase":"100", "hpAdd":"100", "hpMaxLv":"5000", "criticalRate":"0", "multiShootLineNum":"0", "limitedNumber":"1", "damageType":"power", "seriesId":11,"seriesText":"角色", "prop1":{"title":"圣洁的束缚", "damageType":"power", "desc":"放置后，发射13根光之矛，每根光矛落下后对范围内目标造成50(+1.8每破)%武器攻击力伤害，并有150%几率使其陷入禁锢状态，持续3(+0.1每破)秒", "alb":"41", "maxLvDesc":"放置后，发射13根光之矛，每根光矛落下后对范围内目标造成50(68)%武器攻击力伤害，并有150%几率使其陷入禁锢状态，持续3(4)秒"},"posterId":"2", "decompose":true,"decomposeEquip":{"uid":"371", "title":"[5★]犹大的誓约", "img":"838"},"evolveFormula":{"input":[{"id":"385", "input":"371", "output":"372", "materials":["239", "239", "218", "601", "225"],"inputEquip":"838", "outputEquip":"839"},{"id":"452", "input":"371", "output":"453", "materials":["243", "239", "239", "1041", "225"],"inputEquip":"838", "outputEquip":"1015"}],"output":[]},"awakenFormula":["1146", "1146", "1148", "1149", "1150"]},{"img":"839", "title":"犹大的誓约", "desc":"", "rarity":"6", "cost":"20", "maxlv":"99", "uid":"372", "baseType":"放置-远古兵器", "id":"828", "damageBase":"1073", "damageAdd":"9.918", "damageMaxLv":"2044", "ammoBase":"4", "ammoAdd":"0.061", "ammoMaxLv":"9", "fireRateBase":"3.3", "fireRateAdd":"0", "fireRateMaxLv":"3.3", "countDownTimeBase":"4", "countDownTimeAdd":"0", "countDownTimeMaxLv":"4", "hpBase":"100", "hpAdd":"100", "hpMaxLv":"9900", "criticalRate":"0", "multiShootLineNum":"0", "limitedNumber":"1", "damageType":"power", "seriesId":11,"seriesText":"角色", "prop1":{"title":"圣洁的束缚", "damageType":"power", "desc":"放置后，发射13根光之矛，每根光矛落下后对范围内目标造成50(+1.8每破)%武器攻击力伤害，并有150%几率使其陷入禁锢状态，持续3.5(+0.1每破)秒", "alb":"41", "maxLvDesc":"放置后，发射13根光之矛，每根光矛落下后对范围内目标造成50(68)%武器攻击力伤害，并有150%几率使其陷入禁锢状态，持续3.5(4.5)秒"},"posterId":"2", "decompose":true,"decomposeEquip":{"uid":"371", "title":"[5★]犹大的誓约", "img":"838"},"evolveFormula":{"input":[{"id":"986", "input":"372", "output":"20005", "materials":["1720", "1720", "2232", "2232", "2232"],"inputEquip":"839", "outputEquip":"2201"},{"id":"1442", "input":"372", "output":"20382", "materials":["682", "684", "779", "779", "1717"],"inputEquip":"839", "outputEquip":"3187"}],"output":[{"id":"385", "input":"371", "output":"372", "materials":["239", "239", "218", "601", "225"],"inputEquip":"838", "outputEquip":"839"}]},"awakenFormula":["1146", "1146", "1148", "1149", "1150"]}]
```
