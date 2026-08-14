---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> 从 39 条内容中筛选出 17 条重要资讯。

---

**科技新闻**
1. [GLM-5.3：涌现网络能力的自主编码模型](#item-tech-news-1) ⭐️ 9.0/10
2. [Qwen 3.8 27B：本地推理与显式思考的显著进步](#item-tech-news-2) ⭐️ 8.0/10
3. [无训练将 Doom 渲染器编译为 21B 参数 Transformer](#item-tech-news-3) ⭐️ 8.0/10
4. [小红书开源 dots3-note：280B MoE 仅激活 16B](#item-tech-news-4) ⭐️ 8.0/10
5. [PostgreSQL 修复高危 to\_char 堆溢出漏洞，可执行任意代码](#item-tech-news-5) ⭐️ 8.0/10
6. [为什么 Opus 5 用起来更差？讨论聚焦于为智能体优化的沟通风格](#item-tech-news-6) ⭐️ 7.0/10
7. [RustDesk 在 Wayland 下支持真正的无人值守远程访问](#item-tech-news-7) ⭐️ 7.0/10
8. [Firefox 成为唯一支持 uBlock Origin 的主流浏览器](#item-tech-news-8) ⭐️ 7.0/10
9. [PyTorch 新 linter：torch-preflight 可捕获训练错误并估算显存](#item-tech-news-9) ⭐️ 7.0/10
10. [美国法官令谷歌一周内移除第三方应用商店安装障碍](#item-tech-news-10) ⭐️ 7.0/10
11. [苹果联手阿里为中国市场训练专属 AI 大模型](#item-tech-news-11) ⭐️ 7.0/10

**科技博客**
1. [vLLM 自适应验证：DSpark 置信度调度](#item-tech-blog-1) ⭐️ 9.0/10

**财经新闻**
1. [苹果提交美国 App Store 外部购买抽成方案，费率最高 15%](#item-finance-news-1) ⭐️ 8.0/10
2. [伯克希尔二季度大举增持 Alphabet 等股票，终结连续 14 季净卖出](#item-finance-news-2) ⭐️ 7.0/10
3. [高盛从 AI 基建融资热潮中获利](#item-finance-news-3) ⭐️ 7.0/10
4. [Reddit、Applied Materials 等个股盘前大幅波动](#item-finance-news-4) ⭐️ 7.0/10
5. [中信旗下基金接近收购阿里游戏部门，估值或超 15 亿美元](#item-finance-news-5) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [GLM-5.3：涌现网络能力的自主编码模型](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.ai 发布了 GLM-5.3，一款具备涌现网络安全能力的前沿编码模型，能在真实红队场景中自主执行安全研究、发现漏洞并大规模披露。社区用户报告称，通过 Claude Code harness 使用该模型时，它能够完成 WordPress 插件 0-day 发现、RCE 以及 6.8 内核漏洞利用迁移等任务。另一名用户指出，Z.ai 正在扫描开源与流行软件并在 cvd.z.ai 上披露漏洞，许多 CVE 处于保密期且被评为关键或高危。该模型展现了从编码到自主攻击研究的持续能力扩展，但多数漏洞披露细节尚未公开，实际影响仍有待验证。

hackernews · pella · 8月14日 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**「背景」** GLM-5.3 是智谱（Z.ai）于 2026 年 8 月 14 日发布的开放权重模型，与 GLM-5.2 共用同一基础模型，所有提升均来自规模化后训练。其编码能力在 Z.ai Code Bench 上比 GLM-5.2 提升约 50%，并在 Terminal-Bench 3.0 等基准上取得开源模型最优结果；同时展现出“涌现”的网络安全能力，在 CyberGym 漏洞发现基准上达到 SOTA，并在利用类基准上较 GLM-5.2 提升一倍以上。该发布引发关于开源前沿模型安全影响与大规模漏洞披露机制的讨论。

**「影响」** 对依赖 WordPress 插件和 Linux 内核等流行软件的组织，GLM-5.3 的社区演示已经展示出可被自动化发现的真实漏洞路径，可能加剧修复压力；但由于多数披露的 CVE 仍处于保密期，实际影响范围尚不清楚。

**「社区讨论」** 评论中既有正面测试报告，也有保留意见。有用户称 GLM-5.3 是首个接受红队任务并顺利执行（包括 WP 插件 0-day 和内核利用适配）的模型，而另一位用户则指出其大规模扫描并披露 CVE 的做法涉及保密期和成本下降问题。还有人认为它仍略逊于 Sol 和 Fable，本质上是 GLM 5.2 加后训练，并质疑是否有必要从 OpenAI 迁移。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.devdiscourse.com/article/technology/3963858-zais-open-source-model-glm-53-challenges-cybersecurity-norms">Z.ai&#x27;s Open-Source Model GLM-5.3 Challenges Cybersecurity Norms | Technology</a></li>
<li><a href="https://www.unite.ai/z-ai-launches-glm-5-3-with-frontier-coding-and-a-cyber-capability-that-outgrew-its-training/">Z.ai Launches GLM-5.3 With Frontier Coding and a Cyber Capability That Outgrew Its Training – Unite.AI</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**标签**: `#artificial intelligence`, `#cybersecurity`, `#code generation`, `#GLM`, `#open source`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B：本地推理与显式思考的显著进步](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B（Hugging Face 上的 Qwen3.8-27B-FP8）是新一代开源权重模型，在本地推理和推理能力上获得社区好评。一位用户称它是继 Gemma 4 之后第二个能通过其私有基准的本地模型，比 Gemma 4 多花约 5 倍 token，并在开启 MTP 下用 12 分 30 秒完成；另一位在 RTX 5090 上使用 ninfer 推理引擎获得约 138 tokens/秒，约为朴素 llama.cpp 设置的两倍。此外，有用户比较 3.6 版后指出其思考轨迹更接近笔记体，会省略“to/we”等词，也有人观察到 VRAM 使用效率不如 Gemma 4 或 Glimmer。模型还能画出结构正确的自行车上的鹈鹕，尽管缺少链条。

hackernews · erdaltoprak · 8月14日 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**「背景」** Qwen 是阿里巴巴推出的开源大模型系列，此前的 Qwen3.5 与 Qwen3.6 已在社区中被广泛采用。Qwen3.8-27B 是该系列最新一代中面向本地部署的 27B 规模开放权重模型，并以 FP8 量化版等形式发布，旨在降低显存占用、使其更适合在消费级硬件上运行。该模型于 2026 年 8 月 3 日与更大的 Qwen 3.8-Max 一同宣布，但开放权重版本更侧重于让开发者能够自行托管和本地推理。

**「影响」** 对本地推理用户而言，Qwen 3.8 27B 使部分此前只有 Gemma 4 能完成的私有推理任务可在本地完成，并可通过 ninfer 等推理引擎在 RTX 5090 上达到约 138 tokens/秒的速度；但其较高的 VRAM 占用可能限制同样硬件上的并发或长上下文使用。

**「社区讨论」** 评论整体积极：用户称赞其推理和绘图质量，并展示了超过两倍的推理速度；同时也提出两点担忧：与 Gemma 4/Glimmer 相比 VRAM 效率偏低，以及独特的笔记式思考轨迹可能拖累 MTP 预测。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@rosgluk/qwen-3-8-27b-is-coming-and-it-could-be-the-most-important-local-ai-release-of-2026-c1cf381d5292">Qwen 3.8 27B Is Coming - and It Could Be the Most Important Local AI Release of 2026 | by Rost Glukhov | Aug, 2026 | Medium</a></li>
<li><a href="https://www.yottalabs.ai/post/qwen-3-8-27b-specs-hardware-requirements-how-to-run-2026">Qwen 3.8 27B: Specs, Hardware Requirements, and How to Run It (2026) | Yotta Labs</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>

</ul>
</details>

**标签**: `#Qwen`, `#language-model`, `#open-source`, `#local-inference`, `#AI-reasoning`

---

<a id="item-tech-news-3"></a>
### [无训练将 Doom 渲染器编译为 21B 参数 Transformer](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

作者用自研编译器把 Doom 渲染算法转换为计算图，再映射为 21B 参数 Transformer 权重，整个过程未做任何训练。生成的检查点是标准 Hugging Face 格式，可直接用 43 行 Python 宿主程序加载、生成并解析出 E1M1 帧画面。模型通过输入 3614 个场景 token，输出 53747 个绘制指令 token（移动光标、画像素等），机械执行这些指令即可得到渲染帧。在 B200 上生成单帧约需 40 分钟，作者对比原版 Doom 在 486 上可达 35 FPS，而此方案仅为 35 FPD（帧/天）。这展示了用权重编程算法化 Transformer 的可行性，但更偏向概念验证，性能远不及传统渲染。

reddit · r/MachineLearning · /u/notforrob · 8月14日 15:50

**「背景」** 传统的 Transformer 模型需要通过大量训练数据来学习权重，但近期的实验表明，如果已经有一个明确的计算图以及每个中间变量的调度顺序，就可以直接构造模型权重，而无需任何训练。此前已有将计算器或微型计算机编译进 Transformer 的尝试，而这次的工作进一步把 Doom 的渲染算法也编译成了 Transformer 的权重，从而在无需训练的情况下让模型执行像素级渲染任务。

**「影响」** 对研究算法化 Transformer 和权重编程的开发者而言，这提供了一个无需训练、可直接用标准 Hugging Face 库加载的 21B 参数算法模型实例；但当前速度使其仅适用于概念验证，无法替代传统渲染。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://towardsdatascience.com/i-built-a-tiny-computer-inside-a-transformer/">I Built a Tiny Computer Inside a Transformer | Towards Data Science</a></li>
<li><a href="https://ood.dev/posts/calculator/">A calculator, compiled into a transformer — Out of Distribution</a></li>
<li><a href="https://medium.com/data-science-collective/i-built-a-tiny-computer-inside-a-transformer-e3000a0019b3">I Built a Tiny Computer Inside a Transformer | by Sean Moran | Data Science Collective | Medium</a></li>

</ul>
</details>

**标签**: `#transformers`, `#compilers`, `#computation graphs`, `#Doom`, `#neural rendering`

---

<a id="item-tech-news-4"></a>
### [小红书开源 dots3-note：280B MoE 仅激活 16B](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

小红书 dots 实验室开源了 dots3-note preview，这是 dots3 系列首个开放权重模型。模型总参数达 280B，但每次推理仅激活 16B 参数，支持 512K 上下文，并可处理文字、图片、视频和音频。该模型引入了名为 TEMPO 的新强化学习方法，通过自批判和测试时价值估计来训练长程智能体，并已在 Hugging Face 上开源权重。与此同时，团队还发布了 VibeSearchBench 和 VibeLifeBench 两个面向真实场景的智能体基准。此次开源为研究者和开发者提供了大型 MoE 模型的新选择，同时降低了实际部署所需的算力门槛。

telegram · zaihuapd · 8月14日 08:27

**「背景」** MoE（混合专家）模型将总参数量分散到多个“专家”中，推理时只激活其中一部分，从而在保持大量参数能力的同时降低计算成本；这里的 280B 总参数、16B 激活参数即指这一特性。TEMPO 是 dots 实验室提出的一种强化学习方法，强调通过自批判和测试时价值估计来训练模型完成长程任务。VibeSearchBench 与 VibeLifeBench 是同步发布的两个面向真实场景的智能体基准，用于评估模型在搜索、生活规划等长期任务上的表现。

**「影响」** 模型权重开放后，开发者可以直接在 Hugging Face 获取并部署这个 16B 激活参数的 280B MoE 模型，从而以较低推理成本体验大规模模型能力；两个新基准也为智能体评估提供了可复用的测试标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.besthub.dev/articles/open-source-dots3-note-from-imo-full-score-math-to-real-world-long-term-tasks-0b606f67d951">Open‑Source Dots3‑Note: From IMO Full‑Score Math to Re… | BestHub</a></li>
<li><a href="https://github.com/studio-dots-ai/dots3-note-prev">GitHub - studio-dots-ai/dots3-note-prev: dots3 note preview</a></li>
<li><a href="https://huggingface.co/dots-studio/dots3-note-prev">dots-studio/dots3-note-prev · Hugging Face</a></li>

</ul>
</details>

**标签**: `#open-source`, `#MoE`, `#large language models`, `#reinforcement learning`, `#benchmarks`

---

<a id="item-tech-news-5"></a>
### [PostgreSQL 修复高危 to\_char 堆溢出漏洞，可执行任意代码](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL 项目披露并修复高危漏洞 CVE-2026-14669，该漏洞存在于 to\_char\(timestamptz\) 函数处理超长 POSIX 时区缩写的过程中，可引发堆缓冲区溢出。漏洞 CVSS 评分为 8.8，低权限数据库用户可借此以 PostgreSQL 服务进程的操作系统权限执行任意代码，但并非无需认证即可利用。受影响版本包括 PostgreSQL 18.5、17.11、16.15、15.19 和 14.24 之前的版本；由于 18.5 因回归问题未正式发布，18 系列用户应直接升级至 18.6，其他版本用户应分别升级至 17.11、16.15、15.19 或 14.24。此次小版本更新不需要转储数据库或运行 pg\_upgrade，只需更新程序文件并重启服务即可。

telegram · zaihuapd · 8月14日 14:35

**「背景」** to\_char 是 PostgreSQL 中将时间戳等值格式化为字符串的常用函数，timestamptz 表示带时区的时间戳。该漏洞源于解析超长 POSIX 时区缩写时缺少边界检查，导致堆缓冲区溢出，从而可能被低权限用户利用，在数据库服务进程中执行任意代码。了解这个背景有助于理解该漏洞影响的是数据库的时间格式化功能，而非认证机制。

**「影响」** 运行受影响版本且允许非特权用户设置时区的 PostgreSQL 部署面临被低权限账户攻击者以服务进程权限执行任意代码的风险，因此相关用户应优先升级至修复版本。

**标签**: `#postgresql`, `#security`, `#CVE`, `#database`, `#vulnerability`

---

<a id="item-tech-news-6"></a>
### [为什么 Opus 5 用起来更差？讨论聚焦于为智能体优化的沟通风格](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 7.0/10

一篇博客文章及 Hacker News 讨论认为，Opus 5 的沟通风格让人类用户感觉更差，核心推测是模型的后训练重点已从面向人类转向面向智能体（agent）协同。讨论中的用户抱怨其行文过于省略、抽象，常用无生命名词作主语，并频繁“承认错误”或解释，导致阅读疲惫；一名用户称已转向 OpenAI Sol，另一名用户则退回 4.8。该分析属于对模型可用性的观察，而非突破性新闻，但有助于 AI 从业者理解模型沟通取向的变化。

hackernews · numeri · 8月14日 10:12 · [社区讨论](https://news.ycombinator.com/item?id=49296740)

**「背景」** Claude Opus 5 是 Anthropic 于 2026 年 7 月发布的旗舰模型，官方定位为面向长期、多步骤智能体（agentic）编码任务构建，强调对代码库的深入理解与复杂任务中的上下文保持能力。其发布材料显示，Opus 5 在编程和知识工作评测（如 Frontier-Bench 和 GDPval-AA）上达到新的最先进水平，价格仅为同系列前沿模型 Claude Fable 5 的一半。本次讨论的背景正是这一模型在从“面向人类对话”转向“面向智能体协作”的优化过程中，其沟通风格引发的用户体验争议。

**「影响」** 在评论所涉及的工作负载下，Opus 5 的用户会感到沟通成本上升，需要更严格指令以避免发散；已有重度用户改为使用 OpenAI Sol 或退回 4.8。

**「社区讨论」** 社区共识与作者推测一致：后训练可能已转向“智能体语言”。barrkel 批评 Opus 5 行文过分省略和抽象；zmmmmm 认为人类不再是后训练的主要受众；D13Fd 表示在耗尽额度后觉得 OpenAI Sol 更易用；Paradigma11 贴出示例句子，MyFirstSass 则因 5 会偏离指令而退回 4.8。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/claude/opus">Claude Opus \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI`, `#language models`, `#user experience`, `#LLM communication`

---

<a id="item-tech-news-7"></a>
### [RustDesk 在 Wayland 下支持真正的无人值守远程访问](https://rustdesk.com/blog/unattended-remote-access-wayland/) ⭐️ 7.0/10

RustDesk 宣布其开源远程桌面软件现已支持在 Wayland 会话中进行真正的无人值守远程访问，填补了 Linux 远程管理场景中长期存在的缺口。Wayland 的会话和输入模型此前让远程桌面工具难以在无人工介入的情况下控制目标机器，此次更新使系统管理员和 Linux 用户能够更直接地远控无人值守的 Wayland 桌面。该功能是重要但属于增量的改进，而非全新突破；公告没有给出具体版本号或启用步骤，实际部署时仍需参考官方发布说明。

hackernews · rustdesk · 8月14日 16:12 · [社区讨论](https://news.ycombinator.com/item?id=49300759)

**「背景」** Wayland 是 Linux 上常见的显示服务器协议，但远程桌面支持一直是其难点，尤其是不希望有人在被控端每次手动确认连接时，很难实现无人值守访问。RustDesk 是一款开源远程桌面工具，此前在 Wayland 上要么需要每次人工批准，要么依赖启用显示管理器自动登录后立即锁屏等变通方案。现在 RustDesk 官方宣布支持真正的无人值守远程访问，无需远程机器上有人每次确认会话即可连接。

**「影响」** 对于使用 Wayland 的 Linux 远程桌面用户和系统管理员，这意味着无需人为在目标机器前操作即可完成远程登录和控制，简化了无人值守机器的维护流程。实际受影响程度取决于 RustDesk 各发行版的发布节奏和打包版本是否已包含该支持。

**「社区讨论」** 评论中有用户表示前两天刚遇到相关限制，很高兴看到该问题被解决；也有用户指出自托管 RustDesk 时仍不支持加密连接，并贴出 GitHub issue \#3714 作为关注点。另有用户询问 RustDesk 与 VNC、以及基于 SSH 和 Tailscale 的 Remmina 方案的差异和使用场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustdesk.com/blog/unattended-remote-access-wayland/">Unattended Remote Access on Wayland with RustDesk — RustDesk</a></li>
<li><a href="https://www.andotech.net/taming-rustdesk-on-wayland-how-to-fix-screensharing-and-input-issues/">Fix RustDesk on Wayland: Screen &amp; Input – AndoTech.net</a></li>

</ul>
</details>

**标签**: `#RustDesk`, `#Wayland`, `#remote desktop`, `#Linux`, `#open source`

---

<a id="item-tech-news-8"></a>
### [Firefox 成为唯一支持 uBlock Origin 的主流浏览器](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 7.0/10

Firefox 现在成为唯一仍支持 uBlock Origin 的主流浏览器，原因是谷歌推动的 Manifest V3 扩展规范限制了传统广告拦截扩展的能力。Chrome、Edge 和其他基于 Chromium 的浏览器不再支持完整的 uBlock Origin，用户只能使用功能受限的 uBlock Origin Lite 等 MV3 版本。Mozilla 的 Firefox 仍然支持 Manifest V2 扩展，因此保留了完整的广告拦截功能。这一变化凸显了扩展 API 限制对隐私工具和广告拦截能力的影响，也巩固了 Firefox 在注重隐私的用户群体中的地位。

hackernews · DemiGuru · 8月14日 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49303202)

**「背景」** 谷歌主导的 Manifest V3 扩展规范限制了扩展拦截网络请求的能力，导致 uBlock Origin 这类依赖 webRequest API 的扩展无法在 Chromium 系浏览器中继续完整运行。Chrome 从 139 版本开始逐步禁用 uBlock Origin，Microsoft Edge 等 Chromium 浏览器也相继跟进，而 Firefox 仍保持兼容并官方承诺继续支持。因此，Firefox 成为唯一仍能使用完整版 uBlock Origin 的主流浏览器。

**「影响」** 对于依赖完整广告拦截能力的用户，Firefox 成为唯一仍能使用 uBlock Origin 原版的主流浏览器；Chromium 系浏览器用户只能接受 uBlock Origin Lite 的功能限制，或寻找替代方案。

**「社区讨论」** 评论区中，有用户指出 Firefox 会审查 uBlock Origin 等热门扩展的代码更新，以防止恶意代码，但也有观点提醒不要轻易转向志愿者维护的浏览器分支，因为如果 Firefox 消失，这些分支也会消失。还有人批评 Google 通过 Manifest V3 削弱扩展能力，同时有用户表示目前使用 uBlock Origin Lite 并未发现明显问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html">Firefox is now the last major browser that still supports ...</a></li>
<li><a href="https://www.ofzenandcomputing.com/ublock-origin-is-no-longer-available-for-chrome-but-you-can-still-use-it-on-firefox/">uBlock Origin Chrome vs Firefox in 2026: Complete Migration Guide</a></li>

</ul>
</details>

**标签**: `#web browsers`, `#ad blocking`, `#privacy`, `#uBlock Origin`, `#Firefox`

---

<a id="item-tech-news-9"></a>
### [PyTorch 新 linter：torch-preflight 可捕获训练错误并估算显存](https://www.reddit.com/r/MachineLearning/comments/1vo8vv0/a_linter_for_pytorch_torchpreflight_p/) ⭐️ 7.0/10

torch-preflight 是一个针对 PyTorch 的新型 linter，能静态读取代码并捕获常见训练错误，如损失累加导致 autograd 图滞留、缺少 zero\_grad、梯度累积未除以损失、DDP 未使用 DistributedSampler 等，目前已实现 13 条规则。它不需要导入或执行用户代码，因此无需 GPU 和安装 torch；还能估算训练脚本在指定 GPU 上的显存使用是否足够，并给出可节省多少 GiB 的修改建议。开发者称其显存估算在 T4 上对四个模型的峰值测量误差在 4% 以内，但仍承认主要测试目标只有 PyTorch 源码树，存在误报风险。该项目已通过 pip install torch-preflight 发布，并开放贡献。

reddit · r/MachineLearning · /u/LeJanbandhu · 8月14日 14:30

**「背景」** PyTorch 训练脚本常见问题往往发生在运行时，例如忘记调用 optimizer.zero\_grad\(\) 会导致梯度累积，而把 loss 追加到列表会保留整张 autograd 计算图，造成显存膨胀；DDP 分布式训练中若不使用 DistributedSampler，则各 rank 会在相同批次上重复训练。torch-preflight 这类静态分析工具不执行代码，而是通过解析源码在运行前定位这些问题，并提供显存预估。

**「影响」** 对使用 PyTorch 训练且容易因这些常见错误浪费 GPU 时长的开发者来说，torch-preflight 可以在付费跑训练前发现潜在 bug 并判断显存是否足够。需要说明的是，其误报率和显存估算准确性仍有待更广泛的验证。

**标签**: `#PyTorch`, `#linter`, `#debugging`, `#machine-learning`, `#VRAM-estimation`

---

<a id="item-tech-news-10"></a>
### [美国法官令谷歌一周内移除第三方应用商店安装障碍](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 7.0/10

美国地区法官 James Donato 下令谷歌简化竞品安卓应用商店的安装流程，删除 Play Store 中安装第三方应用商店时的多余步骤与警告弹窗。法院认为这些需要用户先点击“查看”再出现“安装”按钮的多步操作，是谷歌蓄意制造的“反竞争摩擦”，意在吓退普通用户。谷歌须在一周内完成系统修改，使安装第三方应用商店像安装普通安卓应用一样直接。该指令源于 Epic 诉谷歌反垄断案，此前陪审团已裁定谷歌在安卓应用分发领域构成非法垄断。

telegram · zaihuapd · 8月14日 09:55

**「背景信息」** Epic 诉谷歌反垄断案源于 Epic Games 指控谷歌在安卓应用分发中非法垄断，陪审团裁定谷歌败诉，法院随后颁布多项补救措施，包括要求谷歌允许第三方应用商店入驻 Google Play 并开放其应用目录。谷歌随后开始在 Play 商店中提供第三方应用商店下载，但美国地区法官 James Donato 认为其额外警示步骤仍构成反竞争摩擦，因此下令一周内移除这些多余步骤，使安装第三方市场像安装普通安卓应用一样直接。

**「影响」** 该禁令将迫使谷歌在一周内移除 Play 商店针对第三方应用商店的警告与多余安装步骤，使 Aptoide 等竞争商店更易被普通用户安装和发现；不过目前 Play 商店新设的第三方应用商店页面仍只有 Aptoide 一家上线，实际生态影响仍较有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://www.theverge.com/policy/979852/that-is-not-acceptable-judge-orders-google-to-make-rival-app-store-installs-easier">&#x27;That is not acceptable&#x27;: Judge orders Google to make rival app store ...</a></li>
<li><a href="https://arstechnica.com/gadgets/2026/08/google-ordered-to-make-it-easier-to-download-alternative-android-app-stores/">Judge gives Google one week to fix &quot;anticompetitive&quot; app store download ...</a></li>
<li><a href="https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/">Google ordered to remove Android app store warning screens</a></li>
<li><a href="https://arstechnica.com/gadgets/2026/08/third-party-app-stores-are-rolling-out-in-google-play-but-theres-only-one-right-now/">Following Epic loss, Google has started hosting rival app stores in the...</a></li>

</ul>
</details>

**标签**: `#Android`, `#antitrust`, `#Google Play Store`, `#app distribution`, `#legal`

---

<a id="item-tech-news-11"></a>
### [苹果联手阿里为中国市场训练专属 AI 大模型](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 7.0/10

苹果正在为中国市场专门训练一款大语言模型，并获得了阿里巴巴的支持。此举改变了苹果此前依赖第三方模型的策略，使其能更好地掌控中国市场的 AI 体验。Apple Intelligence 预计将在未来数月内随 iOS 更新在华上线。中国网信办已于上月对苹果的生成式 AI 服务进行了备案。若顺利落地，苹果或成为首个获北京批准在华提供自有 AI 模型的外国公司。

telegram · zaihuapd · 8月14日 14:47

**「背景」** 中国对生成式 AI 服务实行备案与审批管理，外国公司须通过合规审查才能向境内用户提供服务。Apple Intelligence 因监管要求迟迟未在华上线，苹果过去依赖第三方模型，如今选择自研并与阿里巴巴合作，以便在符合规定的同时提供本地化体验。

**「影响」** 若顺利获批，苹果将成为首个在中国提供自有 AI 模型的外国公司，直接决定 iPhone 用户能否在合规前提下使用 Apple Intelligence，也可能促使其他跨国科技企业调整在华 AI 策略。

**标签**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Regulation`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [vLLM 自适应验证：DSpark 置信度调度](https://vllm.ai/blog/2026-08-14-dspark-adaptive-verification) ⭐️ 9.0/10

rss · vLLM Blog · 8月14日 00:00

**「背景」** 投机解码用额外算力换取更少的解码步。低并发时 GPU 显存受限、算力富余，草稿 token 近乎免费；但高并发时草稿与真实 token 争抢算力，被拒绝的草稿会浪费吞吐。因此固定的 num\_speculative\_tokens 无法同时适配不同并发。

**「方案」** DSpark 为每个草稿 token 输出置信度，调度器将其转为逐位置存活概率，再把预算 B 分配给存活分数最高的草稿槽位，槽位可跨请求竞争。B 通过最大化期望 token 数与每步成本之比得到，成本表在启动时用 dummy 步骤 profile 并强制单调；预算在 CPU 上用一步旧的置信度计算，具体分发则留在 GPU 上基于当前值执行。为支持可变长度验证，作者引入了 varlen decode CUDA graph，一次 capture 即可服务 1 到 k+1 个 token 的混合。并发 1 到 256 的扫描中，自适应验证始终处于 Pareto 前沿，低并发像长块、高并发像短块。限制是它需要完整的 varlen graph 支持，暂不支持 eager、LoRA 与 pipeline parallelism，也会拒绝输出 logprobs。

**「启示」** 作者认为，用置信度调度与成本模型驱动的自适应验证替代静态投机长度，能让投机解码在不同负载下都保持收益，减少用户调参负担，也使 DSpark 更接近“默认开启”的实用方案。

**标签**: `#speculative decoding`, `#vLLM`, `#adaptive verification`, `#CUDA graphs`, `#performance engineering`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [苹果提交美国 App Store 外部购买抽成方案，费率最高 15%](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 8.0/10

苹果在 Epic 反垄断案中向美国法院提交方案，拟对美国 App Store 外部购买收取抽成，标准应用费率 15%，视频、新闻等合作项目及订阅续费 10%，小型企业计划应用 5%。该方案为待审理的提议，并非最终政策。

telegram · zaihuapd · 8月14日 02:33

**「背景」** 此前美国最高法院驳回了苹果暂停下级法院审理相关费率的请求；Epic 将有机会回应，苹果预计需在 9 月 14 日前向最高法院提交书面意见。

**「影响」** 若该方案获法院批准，使用 App Store 进行数字内容外部购买的美国开发者可能适用新的抽成费率；小型企业计划开发者将对应 5% 的最低档。

**标签**: `#Apple`, `#App Store`, `#antitrust`, `#Epic Games`, `#regulation`

---

<a id="item-finance-news-2"></a>
### [伯克希尔二季度大举增持 Alphabet 等股票，终结连续 14 季净卖出](https://www.cnbc.com/2026/08/14/berkshire-hathaway-boosts-alphabet-to-a-top-three-holding-ups-delta-and-housing-bets.html) ⭐️ 7.0/10

伯克希尔-哈撒韦在第二季度大幅增持 Alphabet，持股增至约 1.06 亿股、市值 379 亿美元，环比上升 83%，使 Alphabet 成为其第三大美股持仓；同时将达美航空持仓提高 44%至 5730 万股，并增持 Lennar 等房屋建筑商。据监管文件，该公司当季净买入近 200 亿美元股票，结束了此前连续 14 个季度的净卖出。

rss · CNBC Finance · 8月14日 21:06

**「背景」** Alphabet 持股大增主要来自 6 月初宣布的 100 亿美元私募购买，当时 Alphabet 寻求为人工智能基础设施融资。伯克希尔现金储备从三个月前的创纪录 3974 亿美元降至 6 月底的 3655 亿美元。

**标签**: `#Berkshire Hathaway`, `#Alphabet`, `#Delta Air Lines`, `#Homebuilders`, `#Portfolio Management`

---

<a id="item-finance-news-3"></a>
### [高盛从 AI 基建融资热潮中获利](https://www.cnbc.com/2026/08/14/goldmans-latest-cash-cow-is-all-about-funding-the-ai-infrastructure-boom.html) ⭐️ 7.0/10

高盛正通过协助 AI 基础设施建设融资获利：它参与协助英伟达宣布的 5000 亿美元融资计划，并担任英特尔 200 亿美元和 Alphabet 850 亿美元股票发行的联席账簿管理人，赚取承销费等相关收入。

rss · CNBC Finance · 8月14日 20:05

**「背景」** 这轮融资的背景是，AI 基础设施开支巨大，科技公司需要从外部筹措大额资金，而华尔街大行则通过承销股票发行和为算力设施安排融资来赚取费用。例如，英伟达与高盛等六家机构计划为 AI 基础设施建设融资 5000 亿美元，并将数据中心等算力设施视为可产生现金流的抵押品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/08/14/goldmans-latest-cash-cow-is-all-about-funding-the-ai-infrastructure-boom.html">Goldman’s latest cash cow is all about funding the AI infrastructure boom</a></li>

</ul>
</details>

**标签**: `#Goldman Sachs`, `#AI infrastructure`, `#investment banking`, `#stock offering`, `#Nvidia`

---

<a id="item-finance-news-4"></a>
### [Reddit、Applied Materials 等个股盘前大幅波动](https://www.cnbc.com/2026/08/14/stocks-making-the-biggest-moves-premarket-rddt-amat-sndk-w.html) ⭐️ 7.0/10

盘前多只个股因指数调整、财报和收购传闻出现明显波动：Reddit 因将纳入标普 500 指数上涨 12%；Applied Materials 第二财季财报未能令投资者满意，股价下跌逾 5%；Workday 盘前上涨约 2%，前一日已因路透社报道银湖洽谈收购大涨近 18%；Wayfair、Fox 和 Sandisk 也因评级上调或并购消息走高。

rss · CNBC Finance · 8月14日 10:46

**「背景」** 标普道琼斯指数公司此前宣布，Reddit 将从 8 月 18 日起纳入标普 500 指数（美国大型上市公司股票指数），取代 AvalonBay Communities。

**「影响」** 由于 Reddit 将成为标普 500 指数成分股，跟踪该指数的指数基金通常会在生效前买入 Reddit、卖出 AvalonBay，从而带来相关资金流动。

**标签**: `#S&amp;P 500`, `#Earnings`, `#Mergers and Acquisitions`, `#Semiconductors`, `#Media`

---

<a id="item-finance-news-5"></a>
### [中信旗下基金接近收购阿里游戏部门，估值或超 15 亿美元](https://www.bloomberg.com/news/articles/2026-08-14/trustar-is-said-to-near-1-5-billion-deal-for-alibaba-gaming-arm) ⭐️ 7.0/10

据彭博社报道，中信集团旗下的亚洲私募机构信宸资本（Trustar Capital）正接近收购阿里巴巴旗下游戏业务灵犀互娱，交易估值可能超过 15 亿美元；目前磋商仍在进行，尚未作出最终决定。

telegram · zaihuapd · 8月14日 10:24

**「背景」** 此次交易是阿里巴巴在 CEO 吴泳铭推动下剥离非核心资产、聚焦人工智能与云计算的一部分。灵犀旗舰游戏《三国志·战略版》是与日本光荣特库摩合作开发的大型多人在线策略游戏。

**标签**: `#M&amp;A`, `#Alibaba`, `#Gaming`, `#Private Equity`, `#Divestiture`

---