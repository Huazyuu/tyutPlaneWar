# 太原理工大学程序设计课设

## 飞机大战

> 问题描述：设计一款单机版的射击类游戏。

- java gui实现
- 超级简陋,仅仅能用来答辩
- 需要自己下载数据库的jar
- mysql端口在3307(自己修改就行)

### （1）基本要求

- 玩家注册

- 玩家登录

- 游戏数据持久化到文件或者数据库中

- 游戏具有成绩排行榜

- 游戏具有开始、暂停、结束功能键

  

### （2）核心功能需求分析参考样例

- 参与的角色
    ? 英雄机、子弹、大敌机、小敌机、子弹补给、炸弹补给、天空
- 英雄机发射子弹
    ? 英雄机、子弹、小敌机、大敌机、子弹补给、炸弹补给都在天空上飞行
    ? 子弹可以射击小敌机、大敌机、子弹补给、炸弹补给
    ? 小敌机、大敌机、子弹补给、炸弹补给可以和英雄机撞击
-   英雄机发射单倍、双倍子弹，由火力值控制
    英雄机发射单倍火力，火力值不减
    英雄机发射一次双倍火力，则火力值减2
-   子弹射击小敌机，子弹与小敌机消失，玩家得分1
    子弹射击大敌机，子弹与大敌机消失，玩家得分2
    子弹射击子弹补给，子弹与子弹补给消失，英雄机得奖励（20火力值）
    子弹射击炸弹补给，子弹与炸弹补给消失，英雄机得奖励（1炸弹）
-   小敌机、大敌机、子弹补给、炸弹补给撞击英雄机，命减命1，火力值清空，小敌机、大敌机、子弹补给、
    炸弹补给消失
-   英雄机发射炸弹，屏幕内的所有敌机消失

