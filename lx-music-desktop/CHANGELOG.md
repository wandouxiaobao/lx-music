# lx-music-desktop change log

All notable changes to this project will be documented in this file.

Project versioning adheres to [Semantic Versioning](http://semver.org/).
Commit convention is based on [Conventional Commits](http://conventionalcommits.org).
Change log format is based on [Keep a Changelog](http://keepachangelog.com/).

## [0.17.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.16.0...v0.17.0) - 2020-03-15

### 新增

- 新增多语言设置，目前软件内置了简体中文、繁体中文、英语三种语言，欢迎提交PR翻译更多语言！
- 新增无法打开外部歌单FAQ
- 新增启动参数`search`，使用例子：`.\lx-music-desktop.exe -search="突然的自我 - 伍佰"`
- 新增音频输出设置
- 新增软件内的包括字体在内的界面内容大小调整，现在当窗口大小切换到“较小/大/较大”时，软件内的元素将会适当减小或加大，窗口大小的“小”与“中”内的元素将保持之前的大小暂不做改变
- 新增音源别名，默认将显示别名，想要显示回原名可到设置切换（免责声明：别名仅是本软件用于描述各音源的标签，其名字归版权方所有）
- 新增发现新版本更新失败弹窗的忽略提醒按钮，忽略提醒后，以后同一个版本再失败时将不会弹窗提醒，但仍可到设置-版本更新手动点开更新弹窗查看或恢复提醒
- 新增热搜词，默认关闭，可到设置开启
- 新增历史搜索记录，默认关闭，可到设置开启（右击单个历史记录标签可移除所点击的记录）

### 优化

- 优化月里嫦娥皮肤侧栏鼠标悬浮颜色
- 优化播放进度条的动画效果
- 现在添加下载任务时，后面添加的任务会在列表顶部插入
- 优化歌单打开机制，现在歌单加载失败时会提示加载失败了，并且支持直接打开企鹅、酷我手机分享出来的歌单了
- 优化右上角最小化/关闭按钮布局

### 修复

- 修复歌单详情处于加载状态时无法返回的问题
- 修复鼠标右击复制列表内容时会复制音质标签的问题
- 修复`0.6.2`及以前的版本导出的“所有数据”内的歌曲列表无法导入的问题
- 修复下载列表在某些情况下无法取消全选的问题

### 其他

- 更新Electron到 8.1.1

## [0.16.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.15.0...v0.16.0) - 2020-02-16

### 新增

- 允许选中列表内歌曲名、歌手名、专辑名内的文字，选中后可使用键盘快捷键进行复制
- 新增在列表可选内容区域**鼠标右击**时自动复制列表已选文字的功能
- 新增在搜索框**鼠标右击**时自动粘贴剪贴板的文本到搜索框中
- 任务下载失败时将显示搜索按钮，方便在其他源搜索该歌曲

### 优化

- 优化木叶之村主题翻页器背景颜色
- 优化各个主题音质标签颜色
- 优化其他一些界面细节及用户交互效果

### 修复

- 修复启用透明窗口鼠标不穿透的bug
- 修复大窗口时设置的音乐来源选项不换行的问题
- 修复某些情况下暂停任务会自动开始任务的问题
- 修复移除暂停、错误的任务时不删除未下载完成的文件的问题
- 修复酷狗源歌单热门标签歌单列表无法加载问题
- 修复QQ源歌单热门标签歌单列表无法加载问题

### 其他

- 更新electron到 8.0.1

## [0.15.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.14.1...v0.15.0) - 2020-01-23

洛雪提前祝大家新年快乐、身体健康、阖家幸福！

### 修复

- 修复歌曲下载列表无法加载的问题
- 修复歌曲下载任务数大于最大下载任务数的问题
- 修复某些情况下歌曲下载错误的问题
- 修复下载列表数据没有被迁移直接被丢弃的问题

## [0.14.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.14.0...v0.14.1) - 2020-01-22

洛雪提前祝大家新年快乐、身体健康、阖家幸福！

### 修复

- 修复由于旧版配置文件迁移出错导致的软件界面无法显示的问题

## [0.14.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.13.1...v0.14.0) - 2020-01-22

洛雪提前祝大家新年快乐、身体健康、阖家幸福！

### 新增

- 新增各大平台歌单热门标签显示（显示在歌单界面的第一个下拉标签菜单中）
- 恢复QQ音乐源128k音质试听
- 新增不强制win7开启透明效果即可使用，但要配置运行参数`-nt`，例如：`.\lx-music-desktop.exe -nt`，添加方法可自行百度“给快捷方式加参数”
- 新增“新年快乐”主题，可自行切换体验

### 优化

- 减淡各个主题的歌曲列表分隔线颜色
- 在线音乐列表音质标签优化，当歌曲有无损音质时隐藏高品质标签
- 更新改进的歌词播放插件，现在歌词的播放显示将更准确

### 修复

- 修复咪咕源无法搜索的问题
- 修复更新弹窗底部文字颜色没有适配当前主题颜色的问题
- 修复导入设置窗口大小、代理设置不立即生效的问题
- 修复在线音乐列表获取失败时无限循环请求的问题

### 其他

- 将软件设置与播放列表分离存储成两个文件
- 更新 Electron 到 7.1.9

## [0.13.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.13.0...v0.13.1) - 2019-12-16

### 修复

- 修复全局更新弹窗无法遮盖搜索框的问题

### 其他

- 由于electron 7.1.3 - 7.1.5 的自动更新功能存在Bug，现降级到7.1.2

## [0.13.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.12.1...v0.13.0) - 2019-12-15

### 新增

- 新增搜索框搜索建议键盘上下方向键选择功能
- 聚合搜索新增音源显示
- 新增“离开搜索界面时清空搜索列表”设置选项，默认关闭，可到设置-强迫症设置开启

### 优化

- 优化“信口雌黄”皮肤配色

### 修复

- 修复存在弹出层时，搜索建议列表被弹出层覆盖的问题
- 修复搜索、排行榜、歌单列表多选框从不定状态到选中的Bug

### 移除

- 因Q音接口失效，移除Q音源的试听与下载

### 其他

- 更新electron到7.1.5
- 更新vue到2.6.11

## [0.12.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.12.0...v0.12.1) - 2019-12-01

### 优化

- 优化定位歌曲时的列表滚动机制
- 优化链接点击效果

### 修复

- 修复使用酷我源下载歌曲时，当歌曲无封面时下载报错的问题
- 修复酷我源排行榜、歌单详情列表里的歌曲音质匹配问题（原来无论歌曲有无高品、无损都会显示有）
- 禁止外部链接在软件内打开，将所有外部链接从默认浏览器打开

### 其他

- 更新electron到7.1.2

## [0.12.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.11.0...v0.12.0) - 2019-11-17

由于新下载库仍然没有完成，但下载功能已经可用，so 移除之前使用的第三方下载库，暂时把新下载库的下载模块直接加入本程序，若出现下载问题欢迎反馈！

### 新增

- 新增下载功能对代理设置的支持，现在若在软件设置了代理服务器，下载功能也将会走代理网络了

### 优化

- 新下载模块将对恢复下载的任务进行字节校验，用于解决下载进度超过100%后仍然下载的问题
- 注意：目前仍然无法暂停处于**链接获取**状态中的任务

### 修复

- 修复Linux deb版本`.desktop`桌面文件缺少图标的问题，新增中文名称显示、软件分类，感谢@lowy的反馈！
- 修复下载列表歌曲状态分类列表操作Bug
- 修复歌曲封面下载失败时仍然执行嵌入封面操作导致报错的问题
- 跳过重复添加**相同歌曲名与扩展名的歌曲**，例如你之前下载了A歌曲的128k音质，现在想要下载它的320k音质，但由于两者都是MP3格式，会因为重名导致之前的128k音质被覆盖但列表中仍然显示两种音质的问题（但实际上都是指向后面的320k音质）

## [0.11.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.10.0...v0.11.0) - 2019-11-10

### 新增

- 新增歌曲缓冲定时器，尝试用于解决网络正常但是歌曲缓冲过久的问题
- 新增下载管理的任务状态分类
- 添加**杀毒软件提示有病毒或恶意行为**的说明，可到**常见问题**拉到最后查看（常见问题可在开源地址找到）

### 优化

- 优化更新弹窗机制及其内容描述，对于可以自动更新的版本，现在可以看到软件的下载进度了

## [0.10.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.9.1...v0.10.0) - 2019-11-02

#### 优化

- 大幅减少程序**播放时**对CPU与GPU的使用，经测试CPU使用减少60%以上，GPU使用减少90%以上，这应该能解决MAC系统上的温度上涨的问题

#### 修复

- 修复酷我源**搜索提示**、**排行榜**无法获取的问题
- 修复咪咕源无法播放的问题

## [0.9.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.9.0...v0.9.1) - 2019-10-27

#### 修复

- 修复没有配置文件时程序启动出错的问题

## [0.9.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.8.2...v0.9.0) - 2019-10-27

#### 新增

- 新增窗口大小设置，若觉得软件窗口小可以到设置页调大点
- 新增定位当前播放歌曲，点击播放栏左侧的**歌曲图片**可在播放列表定位当前播放的歌曲（该功能对播放下载列表的歌曲无效）

#### 修复

- 修复搜索提示失效的问题
- 修复从歌单或列表点击搜索按钮搜索目标歌曲时，搜索框未聚焦仍然弹出候选搜索列表的问题

## [0.8.2](https://github.com/lyswhut/lx-music-desktop/compare/v0.8.1...v0.8.2) - 2019-10-20

#### 修复

- 兼容旧版酷我源搜索列表过滤128k音质的bug（注：0.8.1版本仅修复了酷我源的歌曲过滤问题，该修复仅对以后添加的歌曲有效，如果是之前添加的歌曲仍会出现这个问题，现修复对之前旧列表数据的兼容处理）

## [0.8.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.8.0...v0.8.1) - 2019-10-20

#### 修复

- 修复酷我源搜索歌曲结果未添加128k音质导致播放128k音质时显示“该歌曲没有可播放的音频”的问题

## [0.8.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.7.0...v0.8.0) - 2019-10-19

#### 新增

- 新增网易云源歌曲搜索
- 新增网易云源歌单
- 新增各平台通过输入歌单链接或歌单ID打开歌单详情列表，目前只适配了**网页版歌单链接**，其他方式的歌单链接可能无法解析，但你可想办法获取歌单ID后输入打开。注：各平台歌单ID均为纯数字，若遇到链接里存在歌单ID但无法解析的歌单链接，可以到GitHub提交issue或发送邮件或加群830125506反馈！
- 新增音量调整滑动功能，现在支持鼠标左右拖动调整音量了

#### 优化

- 优化搜索框搜索体验
- 优化音量条交互视觉效果
- 缓存歌单详情列表数据

#### 修复

- 修复QQ源歌单无法翻页Bug
- 修复默认列表没有创建时无法显示收藏列表的Bug
- 修复网易云128k直接试听
- 修复歌曲音质不存在时仍然播放或下载的Bug
- 修复调整音量时，调整的位置与鼠标点击的位置不一致的问题

## [0.7.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.6.2...v0.7.0) - 2019-10-07

#### 新增

- 新增“我的收藏”本地播放列表
- 新增缓存清理功能，可到**设置-其他**查看与清理软件缓存
- 新增QQ音乐源搜索
- 新增咪咕源搜索
- 新增咪咕源歌单
- 新增咪咕源排行榜
- 新增我的音乐列表歌曲源显示，默认关闭，可到**设置-列表设置**开启

#### 优化

- 优化选择框动画效果
- 尝试优化选我的音乐列表内容很多时多选的卡顿问题

#### 修复

- 修复列表延迟显示的Bug
- 修复QQ音源128k音质试听

## [0.6.2](https://github.com/lyswhut/lx-music-desktop/compare/v0.6.1...v0.6.2) - 2019-10-01

祝贺祖国成立70周年~！

#### 新增

- 新增QQ音乐源歌单

#### 修复

- 修正火影皮肤名字
- 修复当试听列表为空时，无法切到其他界面的Bug
- 修复百度源搜索结果为空时的接口处理Bug
- 恢复**酷狗**其他音质播放

## [0.6.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.6.0...v0.6.1) - 2019-09-28

### 新增

- 新增试听列表**滚动条位置恢复**设置（可自动恢复到上次离开时的列表滚动位置），本功能默认开启，若不需要可到设置-列表设置将其关闭
- 新增 **《海贼王》** 皮肤，喜欢个性化的可以试试~

### 优化

- 新增DNS解析缓存，加快请求速度
- 优化代码逻辑，减少软件对系统资源的占用
- 优化新版本信息检测，尽量减少弹出版本获取失败弹窗弹出的概率
- 优化下拉列表动画效果

### 修复

- 修复请求超时的逻辑处理Bug，尝试修复请求无法取消导致的正在播放的歌曲与界面显示的信息不一致的问题
- 修复其他一些小Bug

### 移除

- 移除 `192k` 音质
- 移除酷我音源 `ape` 音质，无损推荐 `flac` 格式

## [0.6.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.5.5...v0.6.0) - 2019-09-21

### 新增

- 新增音乐**聚合搜索**，目前支持酷我、酷狗、百度源搜索
- 新增代理功能

### 优化

- 优化从《梦里嫦娥》皮肤切换到其他皮肤时侧栏动画的切换效果

### 修复

- 修复试听列表没有歌曲时会显示列表加载中的Bug
- 修复切换歌单列表详情时的UI Bug

## [0.5.5](https://github.com/lyswhut/lx-music-desktop/compare/v0.5.4...v0.5.5) - 2019-09-13

### 新增

- 月是故乡明，祝大家中秋快乐🥮~~新增个性皮肤 **《月里嫦娥》**，时间仓促，皮肤还不是很完善，可以试试喜不喜欢~😉
- 新增 MAC 版本退出快捷键支持
- 新增点击播放器中的歌曲标题可以复制标题的功能（遇到好听的歌曲方便分享）

### 修复

- 修复 MAC 系统下软件关闭时再次从 dock 打开时报错的Bug
- 修复下载的歌曲文件名中包含命名规则不允许的符号时下载失败的问题（若歌曲名包含这些符号会自动将其移除）
- 修复 MAC 版本不能复制粘贴的问题

## [0.5.4](https://github.com/lyswhut/lx-music-desktop/compare/v0.5.3...v0.5.4) - 2019-09-09

### 移除

- 下载的FLAC文件在修改歌曲信息后，软件无法播放，但使用本地播放器可以播放
- 为了稳妥起见，暂时移除FLAC格式的meta信息修改
- MP3格式无此问题

## [0.5.3](https://github.com/lyswhut/lx-music-desktop/compare/v0.5.2...v0.5.3) - 2019-09-09

### 优化

- 更新所有依赖包到最新

### 修复

- 修复试听酷狗源的音乐仍然获取320k音质导致获取失败的Bug

## [0.5.2](https://github.com/lyswhut/lx-music-desktop/compare/v0.5.1...v0.5.2) - 2019-09-09

### 新增

- 新增强迫症设置-离开搜索界面时是否清空搜索框
- 设置-关于板块新增常见问题链接
- 歌单左上角的分类按钮添加一个**向下图标**，方便识别该按钮为下拉框（该按钮可选择歌单类型，请自行尝试）

### 优化

- 略微优化最小化按钮字符
- 优化试听列表的加载体验，当歌曲数过多时列表将延迟加载

### 修复

- 修复下载管理的一些Bug

### 移除

- 因接口失效，移除网易云音源，酷狗音源仅支持播放128k音质

## [0.5.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.5.0...v0.5.1) - 2019-09-05

### 新增

- 新增右上角最小化/关闭按钮鼠标滑过符号
- 新增下载列表定位文件按钮

### 修复

- 修复百度源歌单全部分类无法加载的问题
- 修复更新弹窗无法弹出的问题

## [0.5.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.4.0...v0.5.0) - 2019-09-05

### 新增

- 新增**封面嵌入**（默认开启，可到设置-下载设置关闭）
- 新增**歌词下载**（默认关闭，可到设置-下载设置开启）
- 新增单例应用功能（实现软件单开功能，禁止软件多开）

### 优化

- 优化歌单列表动画

### 修复

- 修复歌单无法翻页的问题
- 修复在某些情况下，添加下载歌曲导致下载列表崩溃的问题
- 修复版本更新弹窗Bug
- 修复酷狗歌单推荐歌单出现在其他分类中的Bug

## [0.4.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.3.5...v0.4.0) - 2019-09-04


### 新增

- 新增**歌单**功能，目前支持酷我、酷狗、百度源歌单
- 在设置界面-关于洛雪音乐说明部分新增**最新版网盘下载地址**与**打赏地址**
- 新增酷狗 电音热歌榜、DJ热歌榜
- 新增版本更新超时功能，对于部分无法访问GitHub的用户做更新超时提醒

### 移除

- **注意**：0.4.0以前的版本即将失效，请更新到0.4.0版本

## [0.3.5](https://github.com/lyswhut/lx-music-desktop/compare/v0.3.4...v0.3.5) - 2019-08-30

### 新增

- 新增**测试接口**，该接口同样速度较慢，但软件的大部分功能可用，**请自行切换到该接口**，找接口辛苦，且用且珍惜！

### 优化

- 取消需要刷新URL时windows任务栏进度显示错误状态（现显示为暂停状态）

### 修复

- 修复使用临时接口时在试听列表双击灰色歌曲仍然会进行播放的Bug
- 修复歌词加载Bug

## [0.3.4](https://github.com/lyswhut/lx-music-desktop/compare/v0.3.3...v0.3.4) - 2019-08-29

### 优化

- 减少接口不稳定带来的影响，适当增加请求等待时间

### 修复

- 修复播放过程中URL过期不会刷新URL的问题

## [0.3.3](https://github.com/lyswhut/lx-music-desktop/compare/v0.3.2...v0.3.3) - 2019-08-29

### 修复

- **messoer**的接口已经关闭，暂时切换到临时接口使用，部分功能受限。。。
- 修复设置界面更新出错时仍然显示更新下载中的问题
- 修复手动定位播放进度条时存在偏差的问题
- 屏蔽播放器中没有歌曲时对进度条的点击


## [0.3.2](https://github.com/lyswhut/lx-music-desktop/compare/v0.3.1...v0.3.2) - 2019-08-24

### 新增

- 新增酷狗排行榜其他音质下载

## [0.3.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.3.0...v0.3.1) - 2019-08-24

### 修复

- 修复音量条主题适配

## [0.3.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.2.3...v0.3.0) - 2019-08-24

### 新增

- 新增**MAC**及**Linux**版本（需要的可自行下载）
- 新增音量调整
- 新增任务栏播放进度条控制选项（现在可在设置界面关闭在任务栏显示的播放进度）
- 新增更新出错时的弹窗提示
- 从该版本起，非安装版也会有更新弹窗提醒了，但仍然需要手动下载新版本更新，版本信息可到设置页面查看

### 修复

- 强制把临时接口设置回 `messoer` 接口

## [0.2.3](https://github.com/lyswhut/lx-music-desktop/compare/v0.2.2...v0.2.3) - 2019-08-22

### 新增

- 新增任务栏程序标题改变功能（播放歌曲时任务栏标题将显示当前播放的歌曲）

### 修复

- 使用临时接口时，试听列表中的下载按钮仍然能点击的Bug
- 修复某些情况下歌曲链接未能缓存的问题

### 移除

- 移除临时接口（因服务器被攻击，本接口已关闭）
- 移除列表栏设置的隐藏专辑栏选项（感觉这个设置并没有什么luan用，并且还会打破布局）

## [0.2.2](https://github.com/lyswhut/lx-music-desktop/compare/v0.2.1...v0.2.2) - 2019-08-21

### 修复

- 修复下载过程中出错重试5次都失败后不会自动开始下一个任务的Bug
- 修复播放到一半URL过期时不会刷新URL直接播放下一首的问题

## [0.2.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.2.0...v0.2.1) - 2019-08-20

### 优化

- 新增歌曲URL存储，当URL无效时才重新获取，以减少接口不稳定的影响

### 修复

- 修复歌曲加载无法加载时自动切换混乱的Bug
- 修复移除列表最后一首歌曲时播放器不停止播放的问题

## [0.2.0](https://github.com/lyswhut/lx-music-desktop/compare/v0.1.6...v0.2.0) - 2019-08-20

### 新增

- 新增**百度音乐**排行榜及其音乐直接试听与下载
- 新增网易云排行榜音乐直接试听与下载（目前仅支持128k音质）
- 新增酷狗排行榜音乐直接试听与下载（目前仅支持128k音质）

### 修复

- 修复更新弹窗历史版本描述多余的换行问题
- 修复歌曲无法播放的情况下歌词仍会播放的问题

## [0.1.6](https://github.com/lyswhut/lx-music-desktop/compare/v0.1.5...v0.1.6) - 2019-08-19

### 修复

- 修复列表多选音源限制Bug

## [0.1.5](https://github.com/lyswhut/lx-music-desktop/compare/v0.1.4...v0.1.5) - 2019-08-19

### 新增

- 新增搜索列表批量试听与下载功能
- 新增排行榜列表批量试听与下载功能
- 新增试听列表批量移除与下载功能
- 新增下载列表批量开始、暂停与移除功能

### 优化

- 优化歌曲切换机制

## [0.1.4](https://github.com/lyswhut/lx-music-desktop/compare/v0.1.3...v0.1.4) - 2019-08-18

### 新增

- 新增音乐来源切换，可到设置页面-基本设置 look look !
- 为搜索结果列表添加多选功能。
P.S：暂时没想好多选后的操作按钮放哪...

### 优化

- 重构与改进checkbox组件，使其支持不定选中状态
- 完善上一个版本的http请求封装并切换部分请求到该方法上
- 优化其他一些细节

## [0.1.3](https://github.com/lyswhut/lx-music-desktop/compare/v0.1.2...v0.1.3) - 2019-08-17

### 新增

- 新增win32应用构建

### 修复

- 修复安装包许可协议乱码问题
- **messoer 提供的接口已挂**，暂时切换到临时接口！

### 移除

- 由于messoer接口无法使用，QQ音乐排行榜直接播放/下载功能暂时关闭

## [0.1.2](https://github.com/lyswhut/lx-music-desktop/compare/v0.1.1...v0.1.2) - 2019-08-17

### 修复

- 修复更新弹窗的内容显示问题

## [0.1.1](https://github.com/lyswhut/lx-music-desktop/compare/v0.1.0...v0.1.1) - 2019-08-17

### 新增

- QQ音乐排行榜直接试听与下载（该接口貌似不太稳定，且用且珍惜！）

### 优化

- 优化http请求机制
- 更新关于本软件说明

### 修复

- 修复当上一个歌曲链接正在获取时切换歌曲请求不会取消的问题
- 修复切换歌曲时仍然播放上一首歌曲的问题

## [0.1.0] - 2019-8-16

* 0.1.0版本发布