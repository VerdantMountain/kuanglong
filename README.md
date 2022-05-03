<p align="center">
  <img src="https://github.com/qingshan2048/img/blob/main/ethereum.png" width="260">
</p>
<p align="center">
  <img src='https://img.shields.io/github/license/matevip/matecloud' alt='License1'/>
  <img src="https://img.shields.io/github/stars/matevip/artemis" alt="Stars"/>
  <img src="https://img.shields.io/badge/VUE-3.2.2-green" alt="VUE"/>
  <img src="https://img.shields.io/badge/VueRouter-4.0.11-blue" alt="vue-router4"/>
  <img src="https://img.shields.io/badge/Vite-2.5.0-brightgreen" alt="Vite"/>
</p>


# 🌿 矿龙  `最好用的智能挖矿系统`

## 💡 软件简介

- **适用范围**：网吧网咖，电竞酒店，数据中心，均适用
- **图形界面**：操作界面干净整洁，简易易懂，配置简洁方便
- **矿龙算法**：采用计算机底层纯C语言编写，运行稳定流畅不卡顿
- **挖矿内核**：内置性能优良的挖矿内核，保证物理机算力的最大利用率
- **游戏避让**：可以对显存进行检测并智能躲避大型游戏，优先保证客户体验
- **软件更新**：软件保持高频率的更新，最大限度的保证与政策和性能的高度兼容
- **加密数据**：矿龙处理的数据采用了数据加密处理，数据在传输中被通信运营商侦测

## 🍯 界面展示
![Image text](https://github.com/qingshan2048/img/blob/main/zhanshi.png)

## 📝 文件说明

- `KUANGLONG vx.xx.N.exe` - 矿龙智能挖矿系统主程序
- `README.md` - 程序说明文件

## 🔧 安装使用

- 运行系统 Windows 7/8/10/11

```bash
1.双击运行软件，配置参数，选择输出目录，生成挖矿程序

2.将生成的挖矿程序存放于任意目录下，设置开机启动即可

3.稍等片刻，当有份额提交到矿池即可在矿池后台看到数据
```

## 🌭 参数格式

|  矿池配置  |  格式  |  说明  |
|---|---|---|
|  TCP协议   |  eth.f2pool.com:6688   |   直接填写（ip:端口）则默认走tcp协议，备用矿池地址可留空   |
|  TCP协议   |  stratum+tcp://eth.f2pool.com:6688   |  完整格式，备用矿池地址可留空   |
|  SSL加密   |  stratum+ssl://eth.f2pool.com:6688   |  完整格式，备用矿池地址可留空   |

## 🔨 更新日志

- 参考 [vue](https://github.com/vuejs/vue/blob/dev/.github/COMMIT_CONVENTION.md) 规范 ([Angular](https://github.com/conventional-changelog/conventional-changelog/tree/master/packages/conventional-changelog-angular))
```bash
2022-05-?? - v1.44.N  (即将发布)

2022-05-01 - v1.42.N
新增了软件启动默认ETH选项和万象网管OL客户端系统选项
修改了软件内置的敏感挖矿端口
新增锁屏模式和空闲模式的软件超频参数配置和风扇调节
新增空闲挖矿模式锁屏状态息屏功能
增容了内核传参字符串容量，避免了传参溢出异常的问题

2022-04-05 - v1.40.N
因为有些高端显卡开启后台挖矿并不卡，所以将后台挖矿的红字标识改为蓝字
新增ETC锁屏挖矿
新增了后台挖矿强度100%选择，解决部分高端显卡用户后台挖矿算力低的问题
有用户反应nb40.1在win10上拒绝率100%的问题，此版本采用nb39.6进行了替换
增加了线程互斥机制

2022-03-18 - v1.38.N
修复解决了 Windows 10 企业版 LTSC 1809 兼容问题
调整优化了定时器的个数

2022-03-15 - v1.36.N
新增计费系统锁屏界面识别功能，自动识别锁屏状态执行挖矿程序
新增矿工名按照机器名称进行生成功能
新增nod32备选项

2022-03-08 - v1.34.N
对后台挖矿进行了建议不选的红字提示
新增了锁屏挖矿模式，支持锁屏挖矿息屏（黑屏）功能，支持网维管理费分发功能

2022-03-03 - v1.32.N
修改了切换账户端口
定制配置更名为自选配置，更加清晰明了
对界面的一些功能进行了完善
将QQPCTray修改为QPCTray，防止QQ运行时在查找子串的时候进行进程误判退出
软件启动默认空闲挖矿模式，大幅提升用户上机体验，将上机挖矿改为后台挖矿并调整了挖矿强度参数
修正了代码中的worker问题

2022-02-18 - v1.30.N
挖矿程序无法正常挖矿的时候会不停的查询gpu信息，由于显卡驱动的设计缺陷会导致涨爆内存的情况
-此版本通过对显卡驱动接口的空占用，防止内核查询gpu信息，从而有效控制内存爆涨
禁用了看门狗功能

2022-02-17 - v1.28.N
增加了火绒，暗黑破坏神3，地下城与勇士备选项，修改了英雄联盟的进程名称字母大小写
大幅增加了推荐配置的进程数量并将推荐配置设置为启动默认配置
升级了加密服务器
缩短了定时检测时间，提高了检测的灵敏性
增加了互斥机制，防止程序被重复调用导致程序重复启动的问题

2022-02-13 - v1.26.N
增加了屏幕分辨率的高DPI识别，界面更清晰
补充了保存路径可能为空的异常情况提示信息
新增加了十余项暂停和退出进程备选项
取消了联网验证版本的功能
因为100%强度和99%强度在内核调度上有一半的算力差距，防止误加算力造成的机器卡顿
-将上机挖矿的100%强度取消，变更后为1-99%
  
2022-02-10 - v1.24.N 
支持矿池子账户钱包挖矿
优化了软件版本的算法，版本识别更准确
改进了进程识别的程序算法，最大支持暂停和退出功能总计1000个字节的进程名称排除量
-并做出了进程暂停和退出的定制界面
改进了软件挖矿强度的计算算法
用暂停关键字替换了停止关键字，形容更加准确
增加了使用说明页面，增加了产品信息和使用文档
采用了全新的版本命名规则，N代表智能挖矿系列标准发布版，P则代表加强版或者定制版

2022-02-05 - 1.22版本
增加了多币种选项，不只可以挖以太坊，还增加了以太经典币种的选项
将用户改名为矿工，形容更加准确，避免了使用者把用户名和矿池账户名混肴的情况
对屏蔽窗口选项界面做了优化，操作更容易上手
对内核的强度参数进行了程序调节，缓解了用户不敢加强度，挖矿强度和算力不对等的情况
更新了版本更新的下挂窗口提示，可以更好的保证软件的更新效率
取消了更新提示窗口在任务栏的显示状态，界面更加简洁高效
考虑到有些人对引擎的意思理解不是很透彻，所以将程序内的引擎替换为程序关键字
-软件名字更名为矿龙智能挖矿系统
1.22版本（包括）后将开始发布release版本

2022-01-28 - 1.20版本
重新规范了生成程序的界面，增加了内存检测和屏蔽窗口选项
对内核的etc挖矿功能进行了测试

2022-01-27 - 1.18版本
修改了账户的切换时序，保证程序运行及时上线
去掉了软件自带的默认地址，防止误生成参数无效的文件，造成程序的不上线
增加了生成文件可能再运行的情况提示
将软件底部的版权信息由青山软件改成矿龙软件，不容易造成信息的混肴
将待机挖矿命名改成空闲挖矿，形容更加准确易懂

2022-01-26 - 1.16版本
修改了软件的logo，看起来更加温和舒适
新增了开机启动选项，启动项采用线程写入注册表
重新修改了软件的界面
对1.12和1.14版本做了cpu算力100%压力测试，软件均可以稳定运行

2022-01-21 - 1.14版本
对挖矿引擎中的调试输出进行了清除，代码更加简洁高效，避免了输出流阻塞进程的情况

2022-01-21 - 1.12版本
软件将支持数据加密传输，保证挖矿数据的安全
做了软件的自身加密，对关键数据全部与功能绑定，防止被他人进行代码的恶意篡改
取消了单线程轮滚式执行模式，采用了更先进的多路定时器自动触发执行
-同时缓解了定时机制在windows系统中优先级低下的天然缺陷
采用多线程并行处理内核调控机制，增加了程序的流畅性同时避免了进程阻塞的情况
重新设计了程序的账户切换时序和逻辑，程序运行更缜密

2022-01-17 - 1.10版本
同时改进了程序的定时系统，规避了旧版本程序自我卡死的几率
在生成界面新增了官网网址，可以方便更新到最新版本

2022-01-15 - 1.08版本
程序名字重新命名为矿龙网吧挖矿引擎，做出图形界面，可以用来配置生成器
取消了GPU防中断系统，实测此功能效率并不明显
增加了程序自动释放的功能，取消了windows自带的iexpress打包机制
将上机挖矿，待机挖矿，躲避游戏挖矿合并为统一进程集中调度

2021-12-25 - 1.06版本
对挖矿内核的本地访问端口进行了不规则端口设置，使程序不暴漏自己的挖矿特征
将风扇调节模式设置为自动调节
引入了全新的矿工警报系统，当发现有某游戏程序在进行或者远端服务器发出指令后
-可以进行挖矿程序的停止和清除
该版本屏蔽了以下游戏
穿越火线 crossfire
绝地求生 TslGame
反恐精英 csgo
守望先锋 Overwatch
反恐精英OL cstrike-online
赛博朋克2077 Cyberpunk2077

2021-12-22 - 1.04版本
对电脑的风扇转速进行了控制和调节，更好的散热处理，有利于缓解卡顿现象
重新设定了挖矿内核的本地访问端口，使程序不暴漏自己的挖矿特征
挖矿程序自行设置自己为系统隐藏文件，提高了程序的隐蔽性，对试图删除自己的程序提出了更高的权限要求
为挖矿程序增加了GPU防中断模式，当GPU再对游戏程序进行运算时，挖矿程序则不进行中断操作，保证游戏体验
新增加了10个挖矿强度的版本，0.1到1.0为分别为10%到100%挖矿强度
升级了网吧卡顿解决程序v1.04，兼容历史所有版本，一键清除所有挖矿程序

2021-12-20 - 1.02版本
采用了新的命名规则如QSRM(青山如梦)加上版本号，QSRM_1.02，方便后续版本升级进行挖矿效率的对比
采用了全新的内核，硬件识别更准确更省时，挖矿效率更高，平均可提高1.5%的挖矿收益
降低了挖矿账户的切换频率，可以更好减少检测硬件以及软件启动的时间成本，提升挖矿效益
增加了挖矿程序的备用服务器，当挖矿程序无法进行联网的时候会启用内置的备用服务器进行连接
新增加了3个挖矿强度的版本，0.4为40%挖矿强度，0.7为70%挖矿强度，1.0为100%挖矿强度
测试设备用3dmark11跑分，显卡分数会随着挖矿强度的降低而升高，游戏体验有所增加

2021-12-18 - 1.00版本
第一个不调用bat启动的程序在网吧进行了使用

2021-11-25 - 0.00版本
用winrar自解压+bat批处理+exe挖矿内核，实现挖矿程序开机后台自启动
2021.12.17在SZDB的协助下在网吧用10台机器进行了第一次测试，并成功上线
```

## 🐛 其他事项 🚑🎨🔥💥🌐✨👉🚀

- **机场推荐**：https://i.sw19.icu/kUeN
- **注意事项**：用网维大师调用需要再虚拟盘中调用，用菜单调用可能会出现运行两次的情况
- **特别鸣谢**：本软件的第一个忠实用户SZDB
- **关于作者**：如有其他业务可以通过下面的方式联系作者

<img src="https://github.com/qingshan2048/img/blob/main/weixin.jpg" width="320">
