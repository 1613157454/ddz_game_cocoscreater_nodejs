# ddz_game_cocoscreater_nodejs
# 本项目在https://github.com/tinyshu/ddz_game 基础上修改及增加功能。仅供学习交流，如有侵权，请联系我删除 qq 437868141


斗地主游戏 cocoscreator-nodejs-mysql

服务器 : node.js

客户端: cocos creator2.0

数据库 ：mysql

本项目在他人项目上修改及增加功能 https://github.com/tinyshu/ddz_game
如有侵权，请联系删除。 qq 437868141

## 在他人基础上修改及增加如下

### 前端：
 修改：增加登录缓存，使游客登录相同账号。（原：每次登录生成新账号） 
 
 添加：进入大厅显示 用户头像、昵称。（原：固定头像和昵称）
 
 添加：大厅-创建房间-高级房 添加点击及相关功能。（原：点击没反应）
 
 修复：大厅-加入房间-房间号长度大于6-点击后退。（原：点击后退报错）
 
 添加：游戏界面-返回大厅按钮。
 
 添加：叫地主 定时器功能。
 
 添加：等待出牌 定时器功能。
 
 修复：重新回到游戏界面报错，移除事件监听。（原：退出游戏界面，事件监听未去除）
 
 增加：重新回到游戏界面，恢复手牌、底牌、计时器、上次出牌等。
 
 修复：大厅-加入房间-增加游戏满员提示。（原：超过3人进入游戏、玩家界面重叠）
 
 修改：统一座位出牌顺序为逆时针。（原：抢地主和出牌时，有些座位看是顺时针，有些座位看是逆时针）
 
 添加：有玩家游戏掉线提示。
 
 添加：有玩家离开房间通知。
 
 添加：有玩家游戏中逃跑通知及强制结束游戏。 
 
 添加：游戏结束得分提示。
 
 添加：有玩家游戏中掉线 后  重新回到游戏 提示。
 
 修复：手牌不是17张时 发牌动画 报错。
 
 添加：全局 Alert 和 Toast 插件。
 
 添加：本局结束后 分数不够 被踢出房间提示。
 
 删除：弃用本地 createRoomConfig 配置，改为服务器 配置 房间等级 分数 倍数。
 
 添加：玩家分数变更 后 刷新界面分数。
 
 
### 服务端
 修改： 每个房间新建一个数据库连接。（原：app全局共用一个数据库连接）
 
 修改：用户登录连接 转移到 player.js
 
 增加：用户断线后 未登录判断
 
 添加：玩家掉线，从在线列表移除。
 
 添加：玩家掉线后，自动从房间中退出 或 游戏中离线。

 添加：玩家掉线后，通知其它玩家 有玩家退出或掉线。
 
 

 
