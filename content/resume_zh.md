+++
title = "简历"
date = "2023-01-17T15:45:38+08:00"

+++

## 自我介绍

#### 王玉飞

- 求职意向：`研发工程师`

- 性别：`男`

- 年龄：`23`

- 手机：`+86 17610603152`

- 邮箱：`zhongliwang48@gmail.com`

- 座右铭：`荼靡易逝，苦蛊甘饴​`

------

## 教育及工作经历

#### 字节跳动 `2021.7 - 至今` `互娱研发内容安全 前端工程师`
#### 腾讯 `2020.7 - 2020.10` `云与智慧产业事业群 前端实习生`
#### Google Summer of Code `2019.7 - 2019.10` `OpenWISP Contributor`
#### 华中师范大学 `2017.9 - 2021.7` `数字媒体技术 本科`

------

## 专业技能

- `Javascript` 熟练工，`Solidity`、`Golang`、`Rust` 学习中

- 近 `5` 年的前端学习、项目开发经验，熟悉主流的前端技术栈、技术方案设计及项目开发流程

- 熟练掌握前端框架、工程化、CI / CT / CD，熟悉 `NodeJS`，维护过 `BFF` 服务

- 熟悉`区块链技术`、`合约安全`，了解 `反编译`、`DeFi` 原语，掌握 `符号分析` 合约

- 热爱开源和编程，涉猎广泛：`网络安全`、`游戏开发`、`图形学`，目前在 `区块链` 兔子洞探索中

------

## 项目经历

#### 区块链安全 `尝试挖掘各种兔子洞`

- 编写 `front-run` / `back-run` bot

- 用 `Foundry` 框架，复现各种 `DeFi` 攻击的 `POC`

- 用 `Mythril` 工具，`符号分析`合约漏洞、寻找`可执行路径`

- 尝试挖掘 `mev bot` 漏洞

------

#### 字节跳动 `负责维护 人审质量各平台`

- 中台业务以表单场景居多，单独维护各组件内部状态逻辑杂乱，数据流向不清晰
  1. 以 `MVC` 模式重构，将状态、逻辑解耦，实现 URL 到 组件value 的直接、`双向映射`；

  2. `Model`：URL作为全局主要状态存储；同时 URL Search 原生支持`场景快照`，方便场景复现、`集成测试`；

  3. `Controller`：作为中间层负责读取、变更逻辑，通过`状态机`维护，直观观察所有变更分支，方便打点、监测；

  4. `View`：只负责渲染相关逻辑、样式，只与 Controller 通信；

- 历史问题如海内外业务拆分前，代码中存在不同条件分支场景，逻辑杂乱、不易维护
  1. 通过BFF层集成下发`功能开关`，来更好地管理功能分支，发生事故时也能及时回退，降低事故影响面；

  2. 搭建功能开关可视化管理平台，负责平台相关维护

- 负责人审质量各平台一体化建设，推进`Monorepo仓库迁移`和`微前端平台`改造

------

#### 腾讯 `负责 中台客服系统 的业务和技术需求`

- 前端日志工具开发，利用 `AOP` 和`事件监听`等技术，实现性能指标监控的`黑盒埋点`
  1. 利用`策略模式`、`观察者模式`等对工具库进行抽象和重构，使模块`插件化`，支持自定义埋点策略；

  2. 离线化存储日志数据，利用`节流模式`周期性上报埋点；

  3. 后端服务采用 `SCF + Elastic`，实现完整的日志流存储、可视化服务；

- 基于腾讯开源的 `FeFlow` 框架，开发相应的扩展插件，用于项目的打包、部署、ts、测试、eslint等功能，保证各项目结构和规范配置的一致性

- 利用 `Vue + HighCharts` 搭建数据可视化面板，对工单数据进行可视化展示；添加日志埋点，对面板的使用情况进行日志监控与价值分析

------

#### Google Summer of Code `负责 节点可视化平台 的搭建和优化`

- 参加开源活动，为开源组织重写一个可视化工具库，用于编排网络设备节点数据，绘制网络设备拓扑图
  1. 利用 `WebWorker` 并行计算优化编排性能；

  2. `ECharts + Leaflet` 渲染，踩坑了两个框架的兼容性问题，也给第三方插件提了一些`PR`；

  3. 年底以 Mentor 身份，参与了 `Google Code-in`，帮助高校学生接触开源项目提升编程技能，与他们一同完善这个项目；

------