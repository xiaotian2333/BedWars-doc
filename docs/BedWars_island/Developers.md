# 起床战争-海岛 文档中心

文档作者 - Luckly 小优

> 本页面为玩家独立制作，非 Luckly 小优 官方制作

## API文档

[点击前往](/BedWars_island/tag_api.md)

---

## 时间类 设置

### 结束倒计时

说明： 将一局游戏的结束倒计时为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.game_time bw.world_set 1800

用法： /scoreboard players set bw.game_time bw.world_set <value>
```

---

### 游戏结束等待重置时间

说明： 游戏结束后等待 \<value\> 秒开始重置

``` 指令
默认： /scoreboard players set bw.over_time bw.world_set 20

用法： /scoreboard players set bw.over_time bw.world_set <value>
```

---

### 游戏即将开始等待时间

说明： 人数达标后等待 \<value\> 秒后开始游戏

``` 指令
默认： /scoreboard players set bw.start_time bw.world_set 15

用法： /scoreboard players set bw.start_time bw.world_set <value>
```

---

### 玩家重生倒计时

说明： 将玩家的重生倒计时设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.respawn_time bw.world_set 5

用法： /scoreboard players set bw.respawn_time bw.world_set <value>
```

---

### 烟花数量

说明： 将游戏结束时胜利玩家燃放烟花数量设置为 \<value\> , 烟花 0.5s 释放一次

``` 指令
默认： /scoreboard players set bw.fireworks_time bw.world_set 16

用法： /scoreboard players set bw.fireworks_time bw.world_set <value>
```

---

### 床无敌时间

说明： 将游戏开始后的床无敌时间设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.bed_protect bw.world_set 180

用法： /scoreboard players set bw.bed_protect bw.world_set <value>
```

---

## 财富类 设置

### 保留财富

说明： 设置死亡后玩家经验的处理方式

``` 指令
默认： /scoreboard players set bw.keep_money bw.world_set 4

用法： /scoreboard players set bw.keep_money bw.world_set <value>
```

``` 参数说明
<value> = 0 : 丢失
<value> = 1 : 保留
<value> = 2 : 设置为 初始值<bw.init_money>
<value> = 3 : 减少 指定量<bw.demote_money>
<value> = 4 : 保留 1 / 指定数<bw.divide_money>
```

---

### 初始财富

说明： 设置玩家的初始经验为 \<value\> 级

``` 指令
默认： /scoreboard players set bw.init_money bw.world_set 0

用法： /scoreboard players set bw.init_money bw.world_set <value>
```

---

### 减少财富

说明： 设置玩家死亡后经验减少 \<value\> 级

-条件： <bw.keep_money> = 3

``` 指令
默认： /scoreboard players set bw.demote_money bw.world_set 0

用法： /scoreboard players set bw.demote_money bw.world_set <value>
```

---

### 保留 1 / \<value\> 财富

说明： 设置玩家死亡后财富保留 1 / \<value\>

-条件： <bw.keep_money> = 4

``` 指令
默认： /scoreboard players set bw.divide_money bw.world_set 2

用法： /scoreboard players set bw.divide_money bw.world_set <value>
```

---

## 物品类 设置

### 保留物品

说明： 死亡后是否保留物品

``` 指令
默认： /scoreboard players set bw.keep_inventory bw.world_set 0

用法： /scoreboard players set bw.keep_inventory bw.world_set <value>
```

``` 参数说明
<value> = 0 : 丢失
<value> = 1 : 保留
```

---

### 保留武器

说明： 死亡后是否保留武器(剑)

-条件： \<bw.keep_inventory\> = 0

``` 指令
默认： /scoreboard players set bw.keep_sword bw.world_set 2

用法： /scoreboard players set bw.keep_sword bw.world_set <value>
```

``` 参数说明
<value> = 0 : 丢失
<value> = 1 : 保留
<value> = 2 : 保留为最低品质(木)
<value> = 3 : 降低一级品质
<value> = 4 : 设置为初始武器
```

---

### 保留工具

说明： 玩家死亡后是否保留工具(剪,镐,斧)

-条件： \<bw.keep_inventory\> = 0

``` 指令
默认： /scoreboard players set bw.keep_tool bw.world_set 1

用法： /scoreboard players set bw.keep_tool bw.world_set <value>
```

``` 参数说明
<value> = 0 : 丢失
<value> = 1 : 自定义
<value> = 2 : 保留为最低品质(木)
<value> = 3 : 降低一级品质
<value> = 4 : 设置为初始工具
```

---

### 保留斧头

说明： 玩家死亡后是否保留斧头

-条件:  \<bw.keep_inventory\> = 0  且  \<bw.keep_tool\> = 1

``` 指令
默认： /scoreboard players set bw.keep_axe bw.world_set 2

用法： /scoreboard players set bw.keep_axe bw.world_set <value>
```

``` 参数说明
<value> = 0 : 丢失
<value> = 1 : 保留
<value> = 2 : 保留为最低品质(木)
<value> = 3 : 降低一级品质
<value> = 4 : 设置为初始工具
```

---

### 保留镐子

说明： 玩家死亡后是否保留镐子

-条件:  \<bw.keep_inventory\> = 0  且  \<bw.keep_tool\> = 1

``` 指令
默认： /scoreboard players set bw.keep_pickaxe bw.world_set 2

用法： /scoreboard players set bw.keep_pickaxe bw.world_set <value>
```

``` 参数说明
<value> = 0 : 丢失
<value> = 1 : 保留
<value> = 2 : 保留为最低品质(木)
<value> = 3 : 降低一级品质
<value> = 4 : 设置为初始工具
```

---

### 保留剪刀

说明： 玩家死亡后是否保留剪刀

-条件:  \<bw.keep_inventory\> = 0  且  \<bw.keep_tool\> = 1

``` 指令
默认： /scoreboard players set bw.keep_shears bw.world_set 0

用法： /scoreboard players set bw.keep_shears bw.world_set <value>
```

``` 参数说明
<value> = 0 : 丢失
<value> = 1 : 保留
<value> = 4 : 设置为初始工具
```

---

### 初始工具 斧头

说明： 设置玩家的初始工具 斧头

``` 指令
默认： /scoreboard players set bw.init_eqp_axe bw.world_set 0

用法： /scoreboard players set bw.init_eqp_axe bw.world_set <value>
```

``` 参数说明
<value> = 0 : 无
<value> = 1 : 木斧
<value> = 2 : 石斧
<value> = 3 : 铁斧
<value> = 4 : 钻石斧
```

---

### 初始工具 镐子

说明： 设置玩家的初始工具 镐子

``` 指令
默认： /scoreboard players set bw.init_eqp_pickaxe bw.world_set 0

用法： /scoreboard players set bw.init_eqp_pickaxe bw.world_set <value>
```

``` 参数说明
<value> = 0 : 无
<value> = 1 : 木镐
<value> = 2 : 石镐
<value> = 3 : 铁镐
<value> = 4 : 钻石镐
```

---

### 初始工具 剪刀

说明： 设置玩家是否拥有初始工具(剪)

``` 指令
默认： scoreboard players set bw.init_eqp_shears bw.world_set 0

用法： scoreboard players set bw.init_eqp_shears bw.world_set <value>
```

``` 参数说明
<value> = 0 : 无
<value> = 1 : 有
```

---

### 初始武器

说明： 设置玩家的初始武器(剑)

``` 指令
默认： /scoreboard players set bw.init_eqp_sword bw.world_set 1

用法： /scoreboard players set bw.init_eqp_sword bw.world_set <value>
```

``` 参数说明
<value> = 0 : 无
<value> = 1 : 木剑
<value> = 2 : 石剑
<value> = 3 : 铁剑
<value> = 4 : 钻石剑
```

---

## 资产类 设置

### 铁锭产出时间

说明： 将铁锭产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time_iron bw.world_set 1

用法： /scoreboard players set bw.time_iron bw.world_set <value>
```

---

### 铁锭价值

说明： 将铁锭给予经验设置为 \<value\> 级

``` 指令
默认： /scoreboard players set bw.money_iron bw.world_set 1

用法： /scoreboard players set bw.money_iron bw.world_set <value>
```

---

### 金锭产出时间(1~4人)

说明： 将金锭产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time1_gold bw.world_set 10

用法： /scoreboard players set bw.time1_gold bw.world_set <value>
```

---

### 金锭产出时间(5~8人)

说明： 将金锭产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time2_gold bw.world_set 8

用法： /scoreboard players set bw.time2_gold bw.world_set <value>
```

---

### 金锭产出时间(9人以上)

说明： 将金锭产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time3_gold bw.world_set 6

用法： /scoreboard players set bw.time3_gold bw.world_set <value>
```

---

### 金锭价值

说明： 将金锭给予经验设置为 \<value\> 级

``` 指令
默认： /scoreboard players set bw.money_gold bw.world_set 10

用法： /scoreboard players set bw.money_gold bw.world_set <value>
```

---

### 绿宝石产出时间(1~4人)

说明： 将绿宝石产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time1_emerald bw.world_set 80

用法： /scoreboard players set bw.time1_emerald bw.world_set <value>
```

---

### 绿宝石产出时间(5~8人)

说明： 将绿宝石产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time2_emerald bw.world_set 60

用法： /scoreboard players set bw.time2_emerald bw.world_set <value>
```

---

### 绿宝石产出时间(9人以上)

说明： 将绿宝石产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time3_emerald bw.world_set 40

用法： /scoreboard players set bw.time3_emerald bw.world_set <value>
```

---

### 绿宝石价值

说明： 将绿宝石给予经验设置为 \<value\> 级

``` 指令
默认： /scoreboard players set bw.money_emerald bw.world_set 100

用法： /scoreboard players set bw.money_emerald bw.world_set <value>
```

---

### 钻石产出时间(1~4人)

说明： 将钻石产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time1_diamond bw.world_set 80

用法： /scoreboard players set bw.time1_diamond bw.world_set <value>
```

---

### 钻石产出时间(5~8人)

说明： 将钻石产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time2_diamond bw.world_set 60

用法： /scoreboard players set bw.time2_diamond bw.world_set <value>
```

---

### 钻石产出时间(9人以上)

说明： 将绿宝石产出间隔设置为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.time3_diamond bw.world_set 40

用法： /scoreboard players set bw.time3_diamond bw.world_set <value>
```

---

### 钻石价值

说明： 将钻石给予经验设置为 \<value\> 级

``` 指令
默认： /scoreboard players set bw.money_diamond bw.world_set 100

用法： /scoreboard players set bw.money_diamond bw.world_set <value>
```

---

## 世界类 设置

### 游戏难度

说明： 设置游戏难度

``` 指令
默认： /scoreboard players set bw.difficult bw.world_set 1

用法： /scoreboard players set bw.difficult bw.world_set <value>
```

``` 参数说明
<value> = 0 : 和平
<value> = 1 : 简单
<value> = 2 : 普通
<value> = 3 : 困难
```

---

### 饱和效果

说明： 设置是否给予饱和效果

``` 指令
默认： /scoreboard players set bw.saturation bw.world_set 0

用法： /scoreboard players set bw.saturation bw.world_set <value>
```

``` 参数说明
<value> = 0 : 否
<value> = 1 : 是
```

---

### 夜视效果

说明： 设置是否给予夜视效果

``` 指令
默认： /scoreboard players set bw.night_vision bw.world_set 0

用法： /scoreboard players set bw.night_vision bw.world_set <value>
```

``` 参数说明
<value> = 0 : 否
<value> = 1 : 是
```

---

### 达标玩家数

说明： 设置达标人数为 \<value\> 人数足够开始游戏

``` 指令
默认： /scoreboard players set bw.min_player_ct bw.world_set 4

用法： /scoreboard players set bw.min_player_ct bw.world_set <value>
```

---

### 队伍数量

说明： 设置游戏开始后玩家会被分为指定数量的队伍

``` 指令
默认： /function bw.game/bw.data/mode/set_4team

-4队： /function bw.game/bw.data/mode/set_4team

-3队： /function bw.game/bw.data/mode/set_3team

-2队： /function bw.game/bw.data/mode/set_2team
```

---

### 队伍粒子

说明： 队伍成员头顶是否生成对应颜色的粒子

``` 指令
默认： /scoreboard players set bw.team_ptc bw.world_set 1

用法： /scoreboard players set bw.team_ptc bw.world_set <value>
```

``` 参数说明
<value> = 0 : 否
<value> = 1 : 是
```

---

## 道具类 设置

### 救援平台道具冷却

说明： 设置救援平台的道具冷却为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.prop1_cd bw.world_set 3

用法： /scoreboard players set bw.prop1_cd bw.world_set <value>
```

---

### 救援平台存在时间

说明： 设置救援平台的存在时间为 \<value\> 秒

``` 指令
默认： /scoreboard players set bw.prop1_time bw.world_set 15

用法： /scoreboard players set bw.prop1_time bw.world_set <value>
```

---

### 回城道具使用时间

说明： 设置回城道具使用 \<value\> 秒生效

``` 指令
默认： /scoreboard players set bw.prop_back_time bw.world_set 4

用法： /scoreboard players set bw.prop_back_time bw.world_set <value>
```

---

## 权限类 设置

### 获得管理员权限

说明： 允许自己开启创造模式

``` 指令
用法： /tag @s add bw.admin
```
