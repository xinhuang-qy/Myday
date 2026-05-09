# 

## 学习目标

12 周后，你应该能够：

- 独立搭建 Nakama 服务
- 使用 Go 编写 Runtime
- 为 Godot 开发游戏后端
- 编写登录、背包、任务、排行榜、多人房间等系统
- 理解 authoritative server（权威服务器）
- 完成一个小型多人游戏后端 Demo

---

# 学习原则

每天必须遵循：

```text
输入 → 理解 → 实践 → 输出
```

不要只看教程。
必须：

- 写代码
- 记录问题
- 提交 GitHub
- 做运行 Demo
- 写学习笔记

---

# 每日学习时间建议

| 时间 | 内容 |
|---|---|
| 1小时 | Go基础学习 |
| 2小时 | Nakama实战 |
| 1小时 | 小功能开发 |
| 30分钟 | 阅读源码/官方文档 |
| 30分钟 | 写学习笔记 |

总学习时长：4~6小时

---

# 推荐项目目录结构

```text
game-server-study/
├── docs/
├── demos/
├── nakama/
├── godot-client/
├── experiments/
└── problems/
```

---

# 第一阶段：Go基础（第1~2周）

目标：

```text
能看懂 Nakama Go Runtime
```

---

# 第1周：Go语法 + 环境

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day1 | Go安装、VSCode、package、main函数 | 输出 hello world | 笔记：《Go程序运行流程》 |
| Day2 | 变量、基础类型、:= | 玩家信息系统 | GitHub Demo |
| Day3 | if/else、switch、for | 每日签到奖励逻辑 | 笔记：《Go流程控制》 |
| Day4 | 函数、参数、返回值 | 伤害计算器 | GitHub Commit |
| Day5 | struct | Player数据结构 | 笔记：《Struct与游戏对象》 |
| Day6 | slice、map | 背包系统 | inventory demo |
| Day7 | JSON处理 | 玩家存档JSON | 第一个完整小Demo |

---

# 第2周：Go进阶（游戏方向）

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day8 | pointer（指针） | 修改玩家血量 | 指针理解笔记 |
| Day9 | method | AddGold()函数 | GitHub Commit |
| Day10 | interface | 敌人接口系统 | 行为抽象理解 |
| Day11 | error处理 | 金币不足错误 | error demo |
| Day12 | 文件读写 | 玩家存档保存 | save/load demo |
| Day13 | goroutine | 多玩家登录模拟 | 并发实验 |
| Day14 | 阶段总结 | CLI服务器模拟器 | 第一阶段总结文档 |

---

# 第一阶段产出目标

你应该完成：

## 项目

- CLI游戏服务器模拟器
- 玩家数据系统
- 背包系统
- 签到系统
- JSON存档系统

## 能力

- 理解Go基本语法
- 能看懂简单Runtime代码
- 理解游戏数据结构

---

# 第二阶段：Docker + PostgreSQL + Nakama（第3~4周）

目标：

```text
成功运行 Nakama
```

---

# 第3周：Docker与数据库

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day15 | Docker基础 | docker hello-world | Docker理解笔记 |
| Day16 | docker compose | 启动PostgreSQL | compose demo |
| Day17 | PostgreSQL基础 | SELECT/INSERT/UPDATE | SQL练习 |
| Day18 | Nakama架构 | 理解服务结构 | 架构图 |
| Day19 | 官方example | Godot连接Nakama | 成功连接截图 |
| Day20 | Nakama Console | 查看用户和Storage | Console笔记 |
| Day21 | 阶段总结 | 总结整体架构 | 第二阶段文档 |

---

# 第4周：Go Runtime正式入门

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day22 | Runtime结构 | 阅读 InitModule | Runtime理解 |
| Day23 | RPC系统 | 编写 ping rpc | 第一个RPC |
| Day24 | Storage API | 保存金币数据 | 玩家Storage Demo |
| Day25 | Account系统 | 游客登录 | 登录Demo |
| Day26 | Wallet系统 | 金币增加 | Wallet Demo |
| Day27 | Leaderboard | 上传分数 | 排行榜Demo |
| Day28 | 周项目 | 完整玩家系统 | 第一版游戏后端 |

---

# 第二阶段产出目标

## 项目

- Nakama运行环境
- RPC系统
- 玩家数据系统
- 排行榜系统
- 登录系统

## 能力

- 能写Go Runtime
- 理解客户端与服务器交互
- 能调试Nakama服务

---

# 第三阶段：游戏后端核心（第5~8周）

目标：

```text
真正理解游戏服务器逻辑
```

---

# 第5周：背包 + 商店系统

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day29 | 服务端验证 | 防作弊逻辑 | 安全性笔记 |
| Day30 | 商店系统设计 | 商品配置表 | 商店结构图 |
| Day31 | 购买逻辑 | 扣金币 | buy_item rpc |
| Day32 | 发放奖励 | 添加背包道具 | reward system |
| Day33 | 数据同步 | 更新客户端 | 数据流图 |
| Day34 | 测试 | 模拟非法请求 | 调试记录 |
| Day35 | 周项目 | 完整商城系统 | 商店Demo |

---

# 第6周：任务 + 签到系统

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day36 | 时间系统 | 每日重置 | 时间逻辑笔记 |
| Day37 | 任务结构设计 | 任务配置 | task config |
| Day38 | 任务进度 | 击杀计数 | progress demo |
| Day39 | 成就系统 | 长期目标 | achievement demo |
| Day40 | 每日签到 | 连续签到奖励 | 签到系统 |
| Day41 | 数据持久化 | 保存任务状态 | storage设计 |
| Day42 | 周项目 | 完整任务系统 | 第二版游戏后端 |

---

# 第7周：多人同步基础

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day43 | Realtime Match | 创建房间 | room demo |
| Day44 | 玩家加入 | 房间逻辑 | join room |
| Day45 | 消息广播 | 聊天同步 | broadcast demo |
| Day46 | Tick机制 | 游戏循环 | tick实验 |
| Day47 | 玩家状态 | 同步位置 | position sync |
| Day48 | MatchState | 状态管理 | 状态结构 |
| Day49 | 周项目 | 多人房间系统 | multiplayer demo |

---

# 第8周：Authoritative Multiplayer

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day50 | 权威服务器概念 | 理解防作弊 | authoritative笔记 |
| Day51 | 服务端移动判定 | 服务器校验 | movement validation |
| Day52 | 攻击判定 | 服务端伤害 | combat demo |
| Day53 | 状态广播 | 同步HP | hp sync |
| Day54 | 延迟理解 | 模拟网络延迟 | lag test |
| Day55 | 同步优化 | 减少消息 | optimization demo |
| Day56 | 周项目 | 实时战斗Demo | 第一个实时联机Demo |

---

# 第三阶段产出目标

## 项目

- 商店系统
- 背包系统
- 任务系统
- 多人房间
- 实时同步
- 实时战斗Demo

## 能力

- 理解 authoritative server
- 能开发联机玩法
- 理解服务器状态同步

---

# 第四阶段：真正的联机游戏（第9~10周）

目标：

```text
独立开发多人联机玩法
```

---

# 第9周：多人在线房间

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day57 | 房间管理 | 创建房间 | room manager |
| Day58 | 匹配系统 | 自动匹配 | matchmaking demo |
| Day59 | 玩家列表 | 房间信息 | player list |
| Day60 | 聊天系统 | 房间聊天 | chat system |
| Day61 | Ready机制 | 开始游戏 | ready check |
| Day62 | 房间销毁 | 离开逻辑 | room cleanup |
| Day63 | 周项目 | 完整多人大厅 | lobby system |

---

# 第10周：实时战斗系统

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day64 | 战斗循环 | Tick同步 | combat loop |
| Day65 | 技能系统 | 技能释放 | skill system |
| Day66 | 子弹系统 | Projectile逻辑 | bullet demo |
| Day67 | 碰撞判定 | 命中检测 | collision demo |
| Day68 | 死亡与复活 | 玩家状态切换 | respawn system |
| Day69 | 战斗结算 | 分数统计 | result system |
| Day70 | 周项目 | 完整实时战斗 | 联机战斗Demo |

---

# 第五阶段：工程化（第11~12周）

目标：

```text
具备真正的游戏后端工程思维
```

---

# 第11周：后端工程化

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day71 | 日志系统 | 服务器日志 | log system |
| Day72 | 配置管理 | config文件 | config loader |
| Day73 | 热更新思路 | 动态配置 | hot reload demo |
| Day74 | 错误监控 | panic处理 | error handling |
| Day75 | 服务结构优化 | 模块拆分 | project refactor |
| Day76 | Docker部署 | 生产环境运行 | deploy demo |
| Day77 | 周总结 | 工程化整理 | 工程化文档 |

---

# 第12周：最终项目

## 项目目标

制作：

# 《煤老板大亨》游戏后端Demo

---

## 功能要求

| 模块 | 功能 |
|---|---|
| 登录 | 游客登录、账号系统 |
| 玩家数据 | Storage存档 |
| 背包 | 道具系统 |
| 商店 | 购买与奖励 |
| 签到 | 每日奖励 |
| 排行榜 | 财富排行榜 |
| 多人房间 | 创建与加入 |
| 实时同步 | 玩家位置同步 |
| 战斗 | 简单实时战斗 |

---

# 最终阶段产出目标

## GitHub仓库

必须包含：

- README
- 架构图
- 启动说明
- Docker配置
- Nakama Runtime
- Godot客户端

---

## 技术文档

建议输出：

| 文档 | 内容 |
|---|---|
| architecture.md | 后端架构 |
| networking.md | 同步逻辑 |
| storage.md | 数据结构 |
| rpc.md | RPC说明 |
| match.md | Match系统 |
| problems.md | 调试问题记录 |

---

# 每周必须完成的事情

| 项目 | 要求 |
|---|---|
| GitHub Commit | 每天至少一次 |
| 学习笔记 | 每天至少一篇 |
| 可运行Demo | 每周至少一个 |
| 源码阅读 | 每天30分钟 |
| 架构图 | 每周至少一张 |

---

# 推荐学习资源

## Nakama官方

- Nakama Documentation
- Go Runtime Documentation
- 官方示例项目

---

## Go学习

推荐：

- A Tour of Go
- Go by Example

不要过度学习高级特性。
重点是：

```text
为游戏服务器开发服务
```

---

# 学习重点（非常重要）

你不是在学习：

```text
普通Web后端
```

你是在学习：

```text
游戏服务器工程
```

重点永远应该是：

- 状态同步
- 权威服务器
- 防作弊
- Match系统
- 实时同步
- Tick循环
- 数据安全

而不是：

- CRUD网页
- 管理后台
- 普通REST API

---

# 最终能力目标

12周后，你应该能够：

- 独立开发游戏后端
- 编写 Nakama Runtime
- 理解联机同步
- 开发多人房间
- 制作实时战斗Demo
- 为 Godot 提供完整服务端

你会真正进入：

```text
游戏服务器工程师
```

这个方向。

# Nakama + Go 游戏后端学习计划（12周）

## 学习目标

12 周后，你应该能够：

- 独立搭建 Nakama 服务
- 使用 Go 编写 Runtime
- 为 Godot 开发游戏后端
- 编写登录、背包、任务、排行榜、多人房间等系统
- 理解 authoritative server（权威服务器）
- 完成一个小型多人游戏后端 Demo

---

# 学习原则

每天必须遵循：

```text
输入 → 理解 → 实践 → 输出
```

不要只看教程。
必须：

- 写代码
- 记录问题
- 提交 GitHub
- 做运行 Demo
- 写学习笔记

---

# 每日学习时间建议

| 时间 | 内容 |
|---|---|
| 1小时 | Go基础学习 |
| 2小时 | Nakama实战 |
| 1小时 | 小功能开发 |
| 30分钟 | 阅读源码/官方文档 |
| 30分钟 | 写学习笔记 |

总学习时长：4~6小时

---

# 推荐项目目录结构

```text
game-server-study/
├── docs/
├── demos/
├── nakama/
├── godot-client/
├── experiments/
└── problems/
```

---

# 第一阶段：Go基础（第1~2周）

目标：

```text
能看懂 Nakama Go Runtime
```

---

# 第1周：Go语法 + 环境

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day1 | Go安装、VSCode、package、main函数 | 输出 hello world | 笔记：《Go程序运行流程》 |
| Day2 | 变量、基础类型、:= | 玩家信息系统 | GitHub Demo |
| Day3 | if/else、switch、for | 每日签到奖励逻辑 | 笔记：《Go流程控制》 |
| Day4 | 函数、参数、返回值 | 伤害计算器 | GitHub Commit |
| Day5 | struct | Player数据结构 | 笔记：《Struct与游戏对象》 |
| Day6 | slice、map | 背包系统 | inventory demo |
| Day7 | JSON处理 | 玩家存档JSON | 第一个完整小Demo |

---

# 第2周：Go进阶（游戏方向）

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day8 | pointer（指针） | 修改玩家血量 | 指针理解笔记 |
| Day9 | method | AddGold()函数 | GitHub Commit |
| Day10 | interface | 敌人接口系统 | 行为抽象理解 |
| Day11 | error处理 | 金币不足错误 | error demo |
| Day12 | 文件读写 | 玩家存档保存 | save/load demo |
| Day13 | goroutine | 多玩家登录模拟 | 并发实验 |
| Day14 | 阶段总结 | CLI服务器模拟器 | 第一阶段总结文档 |

---

# 第一阶段产出目标

你应该完成：

## 项目

- CLI游戏服务器模拟器
- 玩家数据系统
- 背包系统
- 签到系统
- JSON存档系统

## 能力

- 理解Go基本语法
- 能看懂简单Runtime代码
- 理解游戏数据结构

---

# 第二阶段：Docker + PostgreSQL + Nakama（第3~4周）

目标：

```text
成功运行 Nakama
```

---

# 第3周：Docker与数据库

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day15 | Docker基础 | docker hello-world | Docker理解笔记 |
| Day16 | docker compose | 启动PostgreSQL | compose demo |
| Day17 | PostgreSQL基础 | SELECT/INSERT/UPDATE | SQL练习 |
| Day18 | Nakama架构 | 理解服务结构 | 架构图 |
| Day19 | 官方example | Godot连接Nakama | 成功连接截图 |
| Day20 | Nakama Console | 查看用户和Storage | Console笔记 |
| Day21 | 阶段总结 | 总结整体架构 | 第二阶段文档 |

---

# 第4周：Go Runtime正式入门

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day22 | Runtime结构 | 阅读 InitModule | Runtime理解 |
| Day23 | RPC系统 | 编写 ping rpc | 第一个RPC |
| Day24 | Storage API | 保存金币数据 | 玩家Storage Demo |
| Day25 | Account系统 | 游客登录 | 登录Demo |
| Day26 | Wallet系统 | 金币增加 | Wallet Demo |
| Day27 | Leaderboard | 上传分数 | 排行榜Demo |
| Day28 | 周项目 | 完整玩家系统 | 第一版游戏后端 |

---

# 第二阶段产出目标

## 项目

- Nakama运行环境
- RPC系统
- 玩家数据系统
- 排行榜系统
- 登录系统

## 能力

- 能写Go Runtime
- 理解客户端与服务器交互
- 能调试Nakama服务

---

# 第三阶段：游戏后端核心（第5~8周）

目标：

```text
真正理解游戏服务器逻辑
```

---

# 第5周：背包 + 商店系统

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day29 | 服务端验证 | 防作弊逻辑 | 安全性笔记 |
| Day30 | 商店系统设计 | 商品配置表 | 商店结构图 |
| Day31 | 购买逻辑 | 扣金币 | buy_item rpc |
| Day32 | 发放奖励 | 添加背包道具 | reward system |
| Day33 | 数据同步 | 更新客户端 | 数据流图 |
| Day34 | 测试 | 模拟非法请求 | 调试记录 |
| Day35 | 周项目 | 完整商城系统 | 商店Demo |

---

# 第6周：任务 + 签到系统

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day36 | 时间系统 | 每日重置 | 时间逻辑笔记 |
| Day37 | 任务结构设计 | 任务配置 | task config |
| Day38 | 任务进度 | 击杀计数 | progress demo |
| Day39 | 成就系统 | 长期目标 | achievement demo |
| Day40 | 每日签到 | 连续签到奖励 | 签到系统 |
| Day41 | 数据持久化 | 保存任务状态 | storage设计 |
| Day42 | 周项目 | 完整任务系统 | 第二版游戏后端 |

---

# 第7周：多人同步基础

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day43 | Realtime Match | 创建房间 | room demo |
| Day44 | 玩家加入 | 房间逻辑 | join room |
| Day45 | 消息广播 | 聊天同步 | broadcast demo |
| Day46 | Tick机制 | 游戏循环 | tick实验 |
| Day47 | 玩家状态 | 同步位置 | position sync |
| Day48 | MatchState | 状态管理 | 状态结构 |
| Day49 | 周项目 | 多人房间系统 | multiplayer demo |

---

# 第8周：Authoritative Multiplayer

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day50 | 权威服务器概念 | 理解防作弊 | authoritative笔记 |
| Day51 | 服务端移动判定 | 服务器校验 | movement validation |
| Day52 | 攻击判定 | 服务端伤害 | combat demo |
| Day53 | 状态广播 | 同步HP | hp sync |
| Day54 | 延迟理解 | 模拟网络延迟 | lag test |
| Day55 | 同步优化 | 减少消息 | optimization demo |
| Day56 | 周项目 | 实时战斗Demo | 第一个实时联机Demo |

---

# 第三阶段产出目标

## 项目

- 商店系统
- 背包系统
- 任务系统
- 多人房间
- 实时同步
- 实时战斗Demo

## 能力

- 理解 authoritative server
- 能开发联机玩法
- 理解服务器状态同步

---

# 第四阶段：真正的联机游戏（第9~10周）

目标：

```text
独立开发多人联机玩法
```

---

# 第9周：多人在线房间

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day57 | 房间管理 | 创建房间 | room manager |
| Day58 | 匹配系统 | 自动匹配 | matchmaking demo |
| Day59 | 玩家列表 | 房间信息 | player list |
| Day60 | 聊天系统 | 房间聊天 | chat system |
| Day61 | Ready机制 | 开始游戏 | ready check |
| Day62 | 房间销毁 | 离开逻辑 | room cleanup |
| Day63 | 周项目 | 完整多人大厅 | lobby system |

---

# 第10周：实时战斗系统

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day64 | 战斗循环 | Tick同步 | combat loop |
| Day65 | 技能系统 | 技能释放 | skill system |
| Day66 | 子弹系统 | Projectile逻辑 | bullet demo |
| Day67 | 碰撞判定 | 命中检测 | collision demo |
| Day68 | 死亡与复活 | 玩家状态切换 | respawn system |
| Day69 | 战斗结算 | 分数统计 | result system |
| Day70 | 周项目 | 完整实时战斗 | 联机战斗Demo |

---

# 第五阶段：工程化（第11~12周）

目标：

```text
具备真正的游戏后端工程思维
```

---

# 第11周：后端工程化

| Day | 学习内容 | 实践任务 | 输出 |
|---|---|---|---|
| Day71 | 日志系统 | 服务器日志 | log system |
| Day72 | 配置管理 | config文件 | config loader |
| Day73 | 热更新思路 | 动态配置 | hot reload demo |
| Day74 | 错误监控 | panic处理 | error handling |
| Day75 | 服务结构优化 | 模块拆分 | project refactor |
| Day76 | Docker部署 | 生产环境运行 | deploy demo |
| Day77 | 周总结 | 工程化整理 | 工程化文档 |

---

# 第12周：最终项目

## 项目目标

制作：

# 《煤老板大亨》游戏后端Demo

---

## 功能要求

| 模块 | 功能 |
|---|---|
| 登录 | 游客登录、账号系统 |
| 玩家数据 | Storage存档 |
| 背包 | 道具系统 |
| 商店 | 购买与奖励 |
| 签到 | 每日奖励 |
| 排行榜 | 财富排行榜 |
| 多人房间 | 创建与加入 |
| 实时同步 | 玩家位置同步 |
| 战斗 | 简单实时战斗 |

---

# 最终阶段产出目标

## GitHub仓库

必须包含：

- README
- 架构图
- 启动说明
- Docker配置
- Nakama Runtime
- Godot客户端

---

## 技术文档

建议输出：

| 文档 | 内容 |
|---|---|
| architecture.md | 后端架构 |
| networking.md | 同步逻辑 |
| storage.md | 数据结构 |
| rpc.md | RPC说明 |
| match.md | Match系统 |
| problems.md | 调试问题记录 |

---

# 每周必须完成的事情

| 项目 | 要求 |
|---|---|
| GitHub Commit | 每天至少一次 |
| 学习笔记 | 每天至少一篇 |
| 可运行Demo | 每周至少一个 |
| 源码阅读 | 每天30分钟 |
| 架构图 | 每周至少一张 |

---

# 推荐学习资源

## Nakama官方

- Nakama Documentation
- Go Runtime Documentation
- 官方示例项目

---

## Go学习

推荐：

- A Tour of Go
- Go by Example

不要过度学习高级特性。
重点是：

```text
为游戏服务器开发服务
```

---

# 学习重点（非常重要）

你不是在学习：

```text
普通Web后端
```

你是在学习：

```text
游戏服务器工程
```

重点永远应该是：

- 状态同步
- 权威服务器
- 防作弊
- Match系统
- 实时同步
- Tick循环
- 数据安全

而不是：

- CRUD网页
- 管理后台
- 普通REST API

---

# 最终能力目标

12周后，你应该能够：

- 独立开发游戏后端
- 编写 Nakama Runtime
- 理解联机同步
- 开发多人房间
- 制作实时战斗Demo
- 为 Godot 提供完整服务端

你会真正进入：

```text
游戏服务器工程师
```

这个方向。

