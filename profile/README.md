# AIJISHU

Build with AI, from knowledge to real hardware.

我们在做一组面向 AI 开发者的实用工具，让 AI 不只生成内容和阅读代码，也能管理知识、运行 Agent，并参与仿真与真实设备开发。

[官方网站](https://aijishu.com/) 
<!--[产品文档] · [公众号] · [联系我们]

[需要链接：统一产品文档]
[需要链接：公众号介绍页或二维码图片]
[需要链接：联系邮箱或反馈入口] 
-->

## Products

### JishuBuddy

JishuBuddy 是面向 AI 硬件开发的编程 Agent，覆盖模型调试、开发板、仿真和真机开发。

它可以通过 SSH 和串口读取真实设备返回的信息，根据证据继续分析，并在执行危险命令前请求用户确认。

JishuBuddy，玩 AI 的技术伙伴。

AI hardware development partner for model debugging, simulation, development boards, and real devices.

[了解 JishuBuddy](https://github.com/x-aijishu/jishubuddy) · [npm 安装](https://www.npmjs.com/package/jishubuddy) · [Agent Skills](https://github.com/x-aijishu/jishubuddy-skills)


### JishuDB

JishuDB 是一个面向个人和团队的知识库，让资料能够被整理、检索，并通过 MCP 等方式连接 AI Agent。

它支持关键词、向量和重排相结合的检索方式，可用于内部资料查询、研究分析和基于来源的内容生产。

A local-first knowledge base for humans and AI agents.

[了解 JishuDB] · [桌面版下载] · [Agent Skills] · [问题反馈]

[需要链接：JishuDB 对外产品页或公开文档；如果核心仓库保持私有，不要链接私有仓库]
[需要链接：https://github.com/x-aijishu/jishudb-desktop-releases]
[需要链接：https://github.com/x-aijishu/jishudb-skills]
[需要链接：JishuDB 公开反馈入口]

### JishuShell

JishuShell 是 AI Agent 的统一管理面板，用于管理 Agent 实例、模型服务、Skills、MCP、消息渠道和运行状态。

All your agents, one JishuShell.

[了解 JishuShell] · [npm 安装] · [问题反馈]

[需要链接：https://github.com/x-aijishu/jishushell]
[需要链接：https://www.npmjs.com/package/jishushell]
[需要链接：JishuShell Issues 或反馈入口]

### JishuBench

JishuBench 是面向边缘设备的模型与 Agent 评测工具。评测流程运行在 Host 上，目标设备只负责模型推理和硬件指标采集。

Host-target evaluation infrastructure for models and AI agents on edge devices.

[了解 JishuBench] · [使用文档] · [问题反馈]

[需要链接：https://github.com/x-aijishu/jishubench]
[需要链接：JishuBench 文档地址]
[需要链接：https://github.com/x-aijishu/jishubench/issues]

## JishuBuddy in 30 Seconds

[需要图片：JishuBuddy 20至30秒演示 GIF 或短视频封面。建议展示“提出任务—连接开发板—读取真实设备信息—返回结果—危险操作等待审核”的完整过程。]

大多数编程 Agent 只能看到代码、文件和电脑里的运行环境。

JishuBuddy 尝试继续向前一步：通过 SSH 和串口连接开发板、远程 Linux 设备和其他真实硬件，让 Agent 能够读取设备实际返回的信息，再根据证据继续调试。

它不是“自动接管硬件”，也不会承诺一键修复所有问题。危险命令需要用户审核，无法确认的结论需要明确说明。

目前可以从 Raspberry Pi 开始体验：

- 查看 SSH 设备的连接状态、CPU 和内存
- 保留并分类真实 OpenSSH 错误
- 通过远程 Bash 检查磁盘、温度、服务和进程
- 通过本机串口读取和发送 UTF-8 或 Hex 数据
- 在执行危险 Bash 命令前展示目标、命令和风险

[开始使用 JishuBuddy]

[需要链接：JishuBuddy 快速开始文档或 GitHub 产品仓库]

## Agent Skills

我们正在把具体问题做成 Agent 可以发现和使用的 Skills。

### JishuBuddy Skills

围绕 Raspberry Pi 的首次配置、SSH 排障、串口救援和设备健康检查，让 Agent 先识别问题；需要真实设备证据时，在用户明确同意后安装或复用 JishuBuddy。

[查看 JishuBuddy Skills]

[需要链接：https://github.com/x-aijishu/jishubuddy-skills]

### JishuDB Skills

覆盖知识库连接与检索、行业研究、数据核验、PPT、网站、公众号和小红书内容制作等任务。

[查看 JishuDB Skills]

[需要链接：https://github.com/x-aijishu/jishudb-skills]

## Featured Projects

### Raspberry Pi diagnostics with JishuBuddy

通过 SSH 或串口获取真实设备信息，判断连接失败、过热、卡顿、服务异常和启动问题。

[查看项目]

[需要链接：JishuBuddy 树莓派案例、文章或 Demo 页面]

### Knowledge workflows with JishuDB

把资料检索、行业研究、数据核验和内容生产连接成可追溯的 Agent 工作流。

[查看项目]

[需要链接：JishuDB 案例或 Demo 页面]

### Edge AI evaluation with JishuBench

在 Host 上运行评测流程，在开发板、Mac 或其他边缘设备上运行模型推理并采集指标。

[查看项目]

[需要链接：https://github.com/x-aijishu/jishubench]

## Get Started

### Install JishuBuddy

前置条件：

- Node.js 22 或更高版本
- Linux x64、Linux ARM64 或 Apple Silicon macOS
- 当前不支持原生 Windows

安装：

npm install -g jishubuddy

启动：

jishubuddy

[查看完整安装说明]

[需要链接：JishuBuddy 完整安装文档]

### Install JishuShell

前置条件：

- Node.js 22 或更高版本
- Linux 或 macOS

安装：

npm install -g jishushell

[查看完整安装说明]

[需要链接：https://github.com/x-aijishu/jishushell]

## Community

欢迎关注产品进展、真实测试和开发记录。

- 官方网站：[需要链接：AIJISHU 官网]
- 公众号：[需要图片或链接：公众号二维码/公众号介绍页]
- 小红书：[需要链接：AIJISHU 小红书官方号]
- npm：[需要链接：AIJISHU 或各产品 npm 页面]
- 问题反馈：[需要链接：统一反馈入口]
- 商务与合作：[需要信息：公开邮箱]

## About AIJISHU

我们关注的不是让 AI 看起来无所不能，而是让它在真实任务里获得更可靠的工具、数据和反馈。

从知识库、Agent 管理，到模型评测和 AI 硬件开发，我们希望把复杂能力做成更容易使用、验证和组合的产品。

Build useful tools. Test with real evidence. Keep the human in control.
