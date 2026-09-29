# runninghub-workbuddy-connectors

> Developer: **AI芳程式** ｜ Feedback & suggestions: **zzdh518**
> 开发者：**AI芳程式** ｜ 问题反馈 / 建议：**zzdh518**

**RunningHub 连接器家族 · 总入口** —— 一个仓库看全家族：每个包的定位、痛点、安装方式，外加 4 个可直接上传 WorkBuddy 的连接器 zip。

**RunningHub connector family · entry point** — one repo to see the whole family: what each package does, who it is for, and 4 ready-to-upload WorkBuddy connector zips.

> **30 秒判断从哪开始**：不想挑就先装全能连接器 `runninghub-connector`（一个顶四个）；只想做图/视频/配音的，装对应单品；用 Claude Desktop / Cursor 的开发者走 npm 引擎。
> **30-second check**: undecided → install the all-in-one connector; single-category users → pick one; developers on any MCP client → use the npm engine.


## 🧭 本仓库在家族里的位置 / Where this repo fits

| | |
| --- | --- |
| **本仓库 / This repo** | 🏠 **runninghub-workbuddy-connectors** — 总入口（家族导航） |
| **品类 / Category** | 家族总入口 · 导航与安装指南 |
| **形态 / Form** | 家族导航仓库（文档 + 4 个可直接上传的连接器 zip） |
| **独立可用 / Standalone** | ✅ 单独安装即可用，一条 `npx` 命令跑起来（核心引擎经 npm 分发，源码闭源） |
| **联动可用 / Interop** | ✅ 与家族其它 5 个仓库共用同一套 RunningHub 账号与 API Key，可任选组合安装 |
| **适合谁 / Who it's for** | 第一次接触、不知道从哪个包开始的新用户 |
| **解决的痛点 / Pain it kills** | 连接器有好几个包，不知道哪个适合自己、从哪开始装；各个仓库来回跳，信息零散。 |
| **给你的价值 / What you get** | 一个仓库看全家族：每个包的定位、痛点、安装方式一目了然，还有 4 个可直接上传 WorkBuddy 的连接器 zip 免打包下载。 |

### 🚀 两种用法 / Two ways to use it

**A. 只装这一个（独立部署，最小依赖）** — 你只想在这一个品类上用 AI：

- **WorkBuddy 用户**：在连接器市场搜「RunningHub」，装这一个就行（见下方「安装」）。
- **任意 MCP 客户端 / 开发者**：一条 `npx` 命令，核心引擎经 npm 分发（核心引擎经 npm 分发，源码闭源）：

```bash
# 方式一：npx 直接跑（推荐，需要 runninghub-mcp 已发布到 npm）
npx -y runninghub-mcp@latest

# 方式二：写进 MCP 客户端配置
# { "command": "npx", "args": ["-y", "runninghub-mcp@latest"] }
```

> `--scope` 让后端只加载本品类模型：启动更快、上下文更省、也更不容易挑错模型。

**B. 家族联动（图 + 视频 + 音频一次到位）** — 你想让 AI 一次干完整条链路：

同一个 API Key 下装多个连接器，或在 WorkBuddy 里直接装**全能连接器** [runninghub-connector](https://github.com/fancy5166/runninghub-connector)——一个顶四个；开发者还可以直接用核心引擎 [runninghub-mcp](https://github.com/fancy5166/runninghub-mcp) 自己拼。

### 🔗 家族全部仓库 / The whole family

| | 仓库 / Repo | 品类 / Category | 一句话 / In one line |
| --- | --- | --- | --- |
| ⚙️ | **[runninghub-mcp](https://github.com/fancy5166/runninghub-mcp)** | 核心引擎 · MCP 服务器（npm 包，非连接器） | 给任何 MCP 客户端装上 RunningHub 的 350+ 模型双手 |
| 🧰 | **[runninghub-connector](https://github.com/fancy5166/runninghub-connector)** | 全能 · 图 + 视 + 音 + 3D + 工作流 + LLM | 一个连接器顶掉一堆账号：350+ 模型，一句话从出图切到出片再切到配音 |
| 🎨 | **[runninghub-image-connector](https://github.com/fancy5166/runninghub-image-connector)** | 图像 · 90+ 图像模型 | 电商主图、模特换背景、老图 4K 放大，中文提示词直接可用 |
| 🎬 | **[runninghub-video-connector](https://github.com/fancy5166/runninghub-video-connector)** | 视频 · 200+ 视频模型 | 一条片子不用换五个平台，首尾帧与数字人口播全覆盖 |
| 🔊 | **[runninghub-audio-connector](https://github.com/fancy5166/runninghub-audio-connector)** | 音频 · 50+ 音频模型 | 配音、配乐、人声分离一站搞定，不用买音色包 |

> 💡 **不确定装哪个？** 先装全能连接器 [runninghub-connector](https://github.com/fancy5166/runninghub-connector) 一个就够；
> 只做图片就装 [runninghub-image-connector](https://github.com/fancy5166/runninghub-image-connector)，
> 只做视频装 [runninghub-video-connector](https://github.com/fancy5166/runninghub-video-connector)，
> 只做配音/音乐装 [runninghub-audio-connector](https://github.com/fancy5166/runninghub-audio-connector)，
> 要自己二次开发从 [runninghub-mcp](https://github.com/fancy5166/runninghub-mcp) 入手。

> 全部由 **AI芳程式** 开发，问题反馈或建议请联系 **zzdh518**。


## 📦 直接下载连接器 zip / Download connector zips

[`zips/`](zips) 目录里有 4 个连接器 zip，下载后直接上传 WorkBuddy 开发者后台即可：

| 文件 | 对应仓库 |
| --- | --- |
| `runninghub-1.0.0.zip` | [runninghub-connector](https://github.com/fancy5166/runninghub-connector)（全能） |
| `runninghub-image-1.0.0.zip` | [runninghub-image-connector](https://github.com/fancy5166/runninghub-image-connector)（图像） |
| `runninghub-video-1.0.0.zip` | [runninghub-video-connector](https://github.com/fancy5166/runninghub-video-connector)（视频） |
| `runninghub-audio-1.0.0.zip` | [runninghub-audio-connector](https://github.com/fancy5166/runninghub-audio-connector)（音频） |

## 🧰 从哪开始装 / Where to start

1. **WorkBuddy 用户**：连接器市场搜「RunningHub」，或直接上传上面的 zip。
2. **Claude Desktop / Cursor / 其它 MCP 客户端**：`npx -y runninghub-mcp@latest`（见 [runninghub-mcp](https://github.com/fancy5166/runninghub-mcp)）。
3. **前置条件**：[RunningHub API Key](https://www.runninghub.cn/enterprise-api/consumerApi)（新建即得）+ 账户余额（[邀请注册](https://www.runninghub.cn?inviteCode=zlhtnu0f)填邀请码 `zlhtnu0f` 得 500 RH 币）。

一键安装提示词 / One-click install prompt：[`INSTALL_PROMPT.md`](INSTALL_PROMPT.md)

## 🔒 关于源码 / About the source

本仓库是**导航与文档仓库**，不包含任何服务器源码。核心引擎以 **npm 包 `runninghub-mcp`** 的形式分发（源码闭源）；连接器仓库均为**连接器壳**（只含安装、配置、指南与使用说明）。

This repo is a **navigation & docs repo** and contains no server source. The engine is distributed as the closed-source npm package `runninghub-mcp`; connector repos are shells (install/config/guides only).

## 许可证 / License

[MIT](LICENSE) © AI芳程式
