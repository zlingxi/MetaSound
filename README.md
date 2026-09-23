<div align="center">

# MetaSound · AI 元声造影

**面向 Windows 的本地 AI 语音、音乐与视频创作工作台**

模型在本机运行，数据不出本机，无需调用云端 API。

<p><a href="https://www.aizzx.top/2109.html">下载与更新</a> · <a href="#快速开始">快速开始</a> · <a href="#常见问题">常见问题</a> · <a href="#技术架构">技术架构</a></p>

![Windows](https://img.shields.io/badge/Windows-10%2F11-0078D4?logo=windows&logoColor=white)
![Version](https://img.shields.io/badge/GUI-v0.0.4-4C8BF5)
![Local AI](https://img.shields.io/badge/运行方式-本地推理-16A085)
![License](https://img.shields.io/badge/软件-免费-2E7D32)

</div>

## 产品概览

MetaSound（AI 元声造影）是一款面向创作者的本地 AI 工作台，统一提供语音合成、声音克隆、音乐创作和视频生成能力。GUI 与推理引擎分离部署，按需启动模型，适合对隐私、成本和本地可控性有要求的个人创作者与开发者。

### 核心能力

| 能力 | 说明 | 引擎 | 状态 |
| --- | --- | --- | --- |
| 语音设计 | 通过音色风格、声音特质和自定义描述生成全新音色并朗读文本 | VoxCPM2 | ✅ 已完成 |
| 声音克隆 | 使用至少 3 秒参考音频，克隆音色朗读任意文本 | VoxCPM2 | ✅ 已完成 |
| 音乐创作 | 生成带人声歌曲或纯音乐，44.1 kHz 立体声，最长约 6 分钟 | MiniMax-Music3 | ✅ 已完成 |
| 视频生成 | 支持文生视频、图生视频、全能参考，画面与立体声音轨同步生成 | MiniMax-H3 | ✅ 已完成 |
| 任务中心 | 统一查看音频与视频任务的进度、阶段、错误和输出目录 | — | ✅ 已完成 |

## 界面截图

大部分界面截图集中在此处，每个功能同时展示浅色和深色主题缩略图。点击任意缩略图可打开对应主题的原图。

<table>
  <tr>
    <td align="center"><a href="assets/Light/MetaSound01-语音设计.png"><img src="assets/Light/MetaSound01-语音设计.png" alt="语音设计浅色主题" width="135"></a><a href="assets/Dark/MetaSound01-语音设计.png"><img src="assets/Dark/MetaSound01-语音设计.png" alt="语音设计深色主题" width="135"></a><br><sub>语音设计<br>浅色 · 深色</sub></td>
    <td align="center"><a href="assets/Light/MetaSound02-语音克隆.png"><img src="assets/Light/MetaSound02-语音克隆.png" alt="声音克隆浅色主题" width="135"></a><a href="assets/Dark/MetaSound02-语音克隆.png"><img src="assets/Dark/MetaSound02-语音克隆.png" alt="声音克隆深色主题" width="135"></a><br><sub>声音克隆<br>浅色 · 深色</sub></td>
    <td align="center"><a href="assets/Light/MetaSound03-音乐创作-歌曲.png"><img src="assets/Light/MetaSound03-音乐创作-歌曲.png" alt="歌曲创作浅色主题" width="135"></a><a href="assets/Dark/MetaSound03-音乐创作-歌曲.png"><img src="assets/Dark/MetaSound03-音乐创作-歌曲.png" alt="歌曲创作深色主题" width="135"></a><br><sub>歌曲创作<br>浅色 · 深色</sub></td>
    <td align="center"><a href="assets/Light/MetaSound04-音乐创作-纯音乐.png"><img src="assets/Light/MetaSound04-音乐创作-纯音乐.png" alt="纯音乐创作浅色主题" width="135"></a><a href="assets/Dark/MetaSound04-音乐创作-纯音乐.png"><img src="assets/Dark/MetaSound04-音乐创作-纯音乐.png" alt="纯音乐创作深色主题" width="135"></a><br><sub>纯音乐创作<br>浅色 · 深色</sub></td>
    <td align="center"><a href="assets/Light/MetaSound05-文生视频.png"><img src="assets/Light/MetaSound05-文生视频.png" alt="文生视频浅色主题" width="135"></a><a href="assets/Dark/MetaSound05-文生视频.png"><img src="assets/Dark/MetaSound05-文生视频.png" alt="文生视频深色主题" width="135"></a><br><sub>文生视频<br>浅色 · 深色</sub></td>
  </tr>
  <tr>
    <td align="center"><a href="assets/Light/MetaSound06-图生视频.png"><img src="assets/Light/MetaSound06-图生视频.png" alt="图生视频浅色主题" width="135"></a><a href="assets/Dark/MetaSound06-图生视频.png"><img src="assets/Dark/MetaSound06-图生视频.png" alt="图生视频深色主题" width="135"></a><br><sub>图生视频<br>浅色 · 深色</sub></td>
    <td align="center"><a href="assets/Light/MetaSound07-全能参考.png"><img src="assets/Light/MetaSound07-全能参考.png" alt="全能参考浅色主题" width="135"></a><a href="assets/Dark/MetaSound07-全能参考.png"><img src="assets/Dark/MetaSound07-全能参考.png" alt="全能参考深色主题" width="135"></a><br><sub>全能参考<br>浅色 · 深色</sub></td>
    <td align="center"><a href="assets/Light/MetaSound08-模型管理.png"><img src="assets/Light/MetaSound08-模型管理.png" alt="模型管理浅色主题" width="135"></a><a href="assets/Dark/MetaSound08-模型管理.png"><img src="assets/Dark/MetaSound08-模型管理.png" alt="模型管理深色主题" width="135"></a><br><sub>模型管理<br>浅色 · 深色</sub></td>
    <td align="center"><a href="assets/Light/MetaSound09-输出设置.png"><img src="assets/Light/MetaSound09-输出设置.png" alt="输出设置浅色主题" width="135"></a><a href="assets/Dark/MetaSound09-输出设置.png"><img src="assets/Dark/MetaSound09-输出设置.png" alt="输出设置深色主题" width="135"></a><br><sub>输出设置<br>浅色 · 深色</sub></td>
    <td align="center"><a href="assets/Light/MetaSound10-关于软件.png"><img src="assets/Light/MetaSound10-关于软件.png" alt="关于软件浅色主题" width="135"></a><a href="assets/Dark/MetaSound10-关于作者.png"><img src="assets/Dark/MetaSound10-关于作者.png" alt="关于软件深色主题" width="135"></a><br><sub>关于软件<br>浅色 · 深色</sub></td>
  </tr>
</table>

## 快速开始

### 1. 下载软件与模型

从[官方页面](https://www.aizzx.top/2109.html)下载 Windows x64 安装包，以及按需选择的模型包：

- `MetaSound v0.0.x Windows x64.exe（标准程序安装包）`
- `MetaSoundVoiceEngine.7z（语音合成引擎模型）`
- `MetaSoundMusicEngine.7z（音乐创作引擎模型）`
- `MetaSoundVideoEngine.7z（视频生成引擎模型）`

### 2. 安装模型

将 7z 模型包解压到**不含中文、空格或特殊符号的英文路径**。模型体积较大，建议使用固态硬盘，并确保磁盘空间充足。

### 3. 启动引擎

启动 MetaSound，进入 **偏好设置 → 模型管理**，选择引擎目录并点击「启动」。等待状态变为「运行中」后，即可进入对应创作页面。

> 同一时间只能运行一个引擎。切换能力前，请先停止当前引擎。GUI 退出不会自动关闭引擎进程。

### 4. 开始创作

进入语音、音乐或视频页面，填写提示词和参数，点击「开始生成」。结果会保存到 **偏好设置 → 输出设置** 中配置的目录。

## 创作功能

### 语音：设计音色与克隆声音

#### 语音设计

从音色风格和声音特质预设中组合参数，也可以加入自定义描述；适合创建旁白、角色、播音和有声书等全新音色。

#### 声音克隆

选择 wav、mp3、flac、m4a 或 ogg 参考音频（至少 3 秒），填写参考文本和表达控制，即可克隆音色并朗读新的文本。

### 音乐：歌曲与纯音乐

支持歌曲（有人声）和纯音乐（无人声）两种模式。歌词编辑器支持段落标签和流行歌曲结构模板；音乐描述可包含风格、情绪、人声、配器、BPM 等信息。

可调参数包括音频时长（15~360 秒）、降噪步数和种子。固定正整数种子可复现相近结果，`0` 表示随机。

### 视频：三种生成模式

| 模式 | 用途 |
| --- | --- |
| 文生视频 | 输入画面描述，可用画面风格、运镜方式和声音景观预设辅助提示 |
| 图生视频 | 提供首帧，可选尾帧，画布比例默认跟随首帧 |
| 全能参考 | 添加图片、视频和音频等多模态素材，拖动顺序决定模型阅读顺序 |

通用参数包括 5~15 秒时长、去噪步数、宽高比、768p/544p 分辨率和种子。Turbo 加速使用 4 步蒸馏 LoRA，仅支持文生视频和图生视频，适合预览级快速生成。

### 任务与输出

任务列表统一管理后台生成任务，可查看排队、生成、完成、失败和取消状态；进行中的任务支持取消，已完成任务可直接打开输出目录。

## 硬件要求

**通用要求：** Windows 10/11 x64，支持 CUDA 12.6 的 NVIDIA 驱动，建议使用 SSD 存放模型权重。

| 引擎 | 用途 | 显卡 / 显存 | 主机内存 | 磁盘占用 |
| --- | --- | --- | --- | --- |
| **VoxCPM2** | 语音设计 / 声音克隆 | NVIDIA 显卡即可；权重约 4.7 GB，无独显时回退 CPU | 16 GB+ | 约 10 GB |
| **MiniMax-Music3** | 音乐创作 | 峰值约 8 GB；RTX 3090/4090 更稳定 | 32 GB+ | 约 30 GB |
| **MiniMax-H3** | 视频生成 | 24 GB 显存；int8 实测峰值 16~18 GB | 约 75 GB，建议 96 GB+ | 约 85~115 GB |

> 视频引擎的 int8 权重会常驻主机内存约 75 GB。内存不足可能导致任务失败；请优先确认内存和磁盘空间。

## 技术架构

```mermaid
flowchart LR
    GUI[MetaSoundGUI<br/>PySide6 桌面客户端]
    TASK[TaskManager<br/>任务队列与进度]
    API[本地 HTTP API<br/>127.0.0.1/api/v1]
    VOICE[VoxCPM2<br/>语音引擎]
    MUSIC[MiniMax-Music3<br/>音乐引擎]
    VIDEO[MiniMax-H3<br/>视频引擎]
    OUT[本地输出目录]
    GUI --> TASK --> API
    API --> VOICE
    API --> MUSIC
    API --> VIDEO
    VOICE --> OUT
    MUSIC --> OUT
    VIDEO --> OUT
```

GUI 与模型引擎完全分离：界面不直接加载模型，通过独立进程托管引擎服务，提交任务并轮询进度。用户设置保存在 `%APPDATA%\AI 元声造影\settings.json`，引擎日志位于各引擎目录的 `logs\backend.log`。

### 项目结构

```text
MetaSound/
├── MetaSoundGUI/            # PySide6 前端与打包脚本
│   ├── app/interface/       # 语音、音乐、视频、任务、设置、关于
│   ├── app/core/            # TaskManager
│   ├── app/services/        # BackendProcessManager
│   ├── app/thread/          # 异步生成 Worker
│   ├── app/config/          # 配置与提示词预设
│   └── app/resources/       # 样式、图标与 Qt 资源
├── Backend VoxCPM2/         # 语音引擎
├── Backend Minimax-Music3/  # 音乐引擎
├── Backend Minimax-H3/      # 视频引擎
├── Backend Build/           # 引擎发行版
└── Frontend Build/          # GUI 打包产物
```

## 常见问题

**引擎显示「未安装」怎么办？**  
确认引擎程序和模型权重均已就位；在模型管理页重新选择引擎目录，页面会提示缺少的具体组件。

**引擎启动失败或超时怎么办？**  
检查 CUDA 12.6 驱动、显存和内存是否满足要求，并在模型管理页点击「打开日志」查看 `backend.log`。

**为什么不能同时运行多个引擎？**  
消费级显卡由于显存限制，通常无法同时容纳多个大模型。请先停止当前引擎，再启动另一个引擎。

**生成结果保存在哪里？**  
查看「偏好设置 → 输出设置」中的音频和视频目录，也可以在任务列表中点击「打开目录」。

**软件退出后引擎还在运行吗？**  
会。GUI 退出不会关闭引擎进程；重新打开软件后会自动探测并接管。需要释放资源时，请在模型管理页显式停止引擎。

## 技术栈

- **前端：** Python、PySide6、Nuitka
- **后端：** Python 3.10+、PyTorch、CUDA 12.6+
- **模型：** VoxCPM2、MiniMax-Music3、MiniMax-H3
- **通信：** 本地 HTTP 服务，监听 `127.0.0.1`
- **能力：** 进程托管、异步任务线程、本地配置持久化、深浅色主题

## 开源现状与后续规划

当前软件安装包和模型权重免费公开，但项目暂未确定全量开源范围。主要原因包括个人项目维护成本、第三方模型权重的版权梳理，以及避免不成熟源码被恶意篡改或付费倒卖。

针对二次开发需求，技术用户可联系作者获取后端源码、环境配置脚本和接口文档。后续将优先评估开放前端 GUI，待引擎代码、模型版权和版本稳定性完成梳理后，再评估全量开源。

## 关于作者

- 作者：聆曦
- 官网、下载与版本更新：[aizzx.top/2109.html](https://www.aizzx.top/2109.html)
- 赞助支持：[aizzx.top/sponsor](https://www.aizzx.top/sponsor)
- Bug 反馈：可在博客、B 站或抖音评论区以及github的issues提交
- 商用提示：软件生成内容可免费商用，但须遵循各底层模型自身的开源商用协议

<div align="center"><strong>MetaSound · 让本地 AI 成为你的创作工作台</strong></div>
