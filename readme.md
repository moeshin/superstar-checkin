# Superstar Checkin

超星学习通签到助理。本程序正在开发中，目前只实现了预期的部分功能

本程序包含了 QQ 机器人，依赖 MongoDB 数据库存储数据。

## 功能（已实现部分）

- [x] 自动取 Cookie，过期自动更新
- [ ] 定时检测签到
- [x] 支持通过学习通 IM 协议实时获取签到推送
- [x] 在群内发送提醒并自动签到
- [x] 通过 QQ 机器人接收群内发送的二维码实现二维码签到
  本功能只需要一张已过期的二维码就可以
- [ ] 通过 REST API 设置课程信息
- [ ] 支持多用户共同签到
- [ ] 根据课程设置签到经纬度以及位置名称

## 部署方法

1. 安装 NodeJS 12.16 以上版本
2. `yarn install`
3. `cp config.example.yaml config.yaml` 并在 `config.yaml` 中填写配置项
4. `yarn build`
5. `yarn start`

## 限制

（据说）学习通禁止腾讯云阿里云这种 IP 签到，所以需要部署在家庭宽带下

## 参考

本程序借鉴了一些前人的项目：

- [mkdir700/chaoxing_auto_sign](https://github.com/mkdir700/chaoxing_auto_sign)
- [SSmJaE/XueXiTonsSign_Electron](https://github.com/SSmJaE/XueXiTonsSign_Electron)
- [cyanray/cx-auto-sign](https://github.com/cyanray/cx-auto-sign)

更多有关学习通签到的项目值得尝试

| 项目地址                                                | 开发语言   | 备注                                           |
| ------------------------------------------------------- | ---------- | ---------------------------------------------- |
| https://github.com/cyanray/cx-auto-sign                 | C#         | 超星学习通自动签到工具，通过IM协议监测签到活动。        |
| https://github.com/mkdir700/chaoxing_auto_sign          | Python     | 超星学习通自动签到脚本&多用户多任务&API       |
| https://github.com/PrintNow/ChaoxingSign                | PHP        | PHP版超星自动签到，支持多用户，二次开发便捷！|
| https://github.com/Wzb3422/auto-sign-chaoxing           | TypeScript | 超星学习通自动签到，梦中刷网课       |
| https://github.com/Huangyan0804/AutoCheckin             | Python     | 学习通自动签到，支持手势，二维码，位置，拍照等 |
| https://github.com/aihuahua-522/chaoxing-testforAndroid | Java       | 学习通（超星）自动签到               |
| https://github.com/yuban10703/chaoxingsign              | Python     | 超星学习通自动签到                   |
| https://github.com/SSmJaE/XueXiTonsSign_Electron        | TypeScript | 基于Electron，桌面端，GUI，签到队列            |
