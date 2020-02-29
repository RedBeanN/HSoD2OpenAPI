# illustrate/:key/:value

## 装备图鉴/按其他属性值查询

### 根据指定的属性值查询装备

仅支持查询国测合并(`merged`)图鉴

### 参数

#### `key`

属性名

### `value`

属性值

### 返回值

`Array[Object]` 对应的装备数组, 可能包含多个装备, 按 uid 排序

装备不存在时返回空数组

### 例

`GET https://api.redbean.tech/illustrate/damageMaxLv/582`

获取满级攻击力为 582 的装备

``` JSON
[{"img":"3515","title":"闪亮旋律","desc":"","rarity":"7","cost":"45","maxlv":"99","uid":"20487","baseType":"自动步枪","id":"3695","damageBase":"388","damageAdd":"1.98","damageMaxLv":"582","ammoBase":"321","ammoAdd":"0.816","ammoMaxLv":"400","fireRateBase":"10","fireRateAdd":"0","fireRateMaxLv":"10","countDownTimeBase":"0","countDownTimeAdd":"0","countDownTimeMaxLv":"0","hpBase":"0","hpAdd":"0","hpMaxLv":"0","criticalRate":"0.05","multiShootLineNum":"0","limitedNumber":"0","damageType":"power","seriesId":21,"seriesText":"歌姬","prop1":{"title":"涤荡的心之辉光","damageType":"none","desc":"攻击时，回复3(+0.1每破)%最大生命值","alb":"41","maxLvDesc":"攻击时，回复3(4)%最大生命值"},"prop2":{"title":"汇聚的爱之勇气","damageType":"none","desc":"击中目标时，提升4.08(+0.04每级/+0.2每破)%生命值上限和15.3(+0.15每级/+1每破)%全伤害，持续5秒，可叠8层","alb":"41","maxLvDesc":"击中目标时，提升8(10)%生命值上限和30(40)%全伤害，持续5秒，可叠8层"},"posterId":"0","decompose":true,"decomposeEquip":{"uid":"359","title":"[6★]歌姬吉他","img":"794"},"evolveFormula":{"input":[],"output":[{"id":"1560","input":"359","output":"20487","materials":["682","683","779","1718","1718"],"inputEquip":"794","outputEquip":"3515"}]}}]
```
