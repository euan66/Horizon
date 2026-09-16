---
layout: default
title: "Horizon Summary: 2026-09-16 (ZH)"
date: 2026-09-16
lang: zh
---

> 从 36 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [Google 发布 Gemini 3.8 Live 与扩展思考版](#item-tech-news-1) ⭐️ 8.0/10
2. [SemiAnalysis：暂停令未实质性扼杀美国数据中心建设](#item-tech-news-2) ⭐️ 8.0/10
3. [Typesafe.ai 发布 System One 模型与 Jev](#item-tech-news-3) ⭐️ 7.0/10
4. [电子墨水相框：用 BirdNET 听鸟鸣并画出 19 世纪风格插画](#item-tech-news-4) ⭐️ 7.0/10
5. [互联网档案馆更新 Wayback Machine 访问状况](#item-tech-news-5) ⭐️ 7.0/10
6. [Show HN：20 美元 4G 热点改造成可发短信设备](#item-tech-news-6) ⭐️ 7.0/10
7. [美国首次确认已部署太空武器](#item-tech-news-7) ⭐️ 7.0/10
8. [Simon Willison 发布 Gemini Live 语音对话网页工具](#item-tech-news-8) ⭐️ 7.0/10
9. [SHADOW-50M：44M 三值 LLM，19.8MB 跑在 CPU 约 1900 tok/s](#item-tech-news-9) ⭐️ 7.0/10
10. [Prior Labs 发布 TabPFN-3.5 表格基础模型](#item-tech-news-10) ⭐️ 7.0/10
11. [工信部与发改委印发电子信息制造业“十五五”规划](#item-tech-news-11) ⭐️ 7.0/10
12. [谷歌向全员工程师开放 Claude Opus 5 用于内部开发](#item-tech-news-12) ⭐️ 7.0/10
13. [联发科发布天玑 9600 Pro：首款台积电 2nm 手机芯片](#item-tech-news-13) ⭐️ 7.0/10
14. [404 Media：OpenAI“Project Lily”由数百名合同工阅读 ChatGPT 对话](#item-tech-news-14) ⭐️ 7.0/10

**财经新闻**
1. [中国 8 月零售增长不及预期，投资降幅加深](#item-finance-news-1) ⭐️ 8.0/10
2. [报道称字节跳动 2026 上半年净利润降至约 200 亿美元](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Google 发布 Gemini 3.8 Live 与扩展思考版](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/) ⭐️ 8.0/10

Google 在官方博客宣布推出 Gemini 3.8 Live 和 Gemini 3.8 Live Extended Thinking，这是一次面向 AI 模型与语音交互的更新。该发布在 Hacker News 上获得了大量关注，相关讨论集中在实际使用体验上。不过，现有材料主要停留在发布公告和用户评论层面，缺少基准测试、详细技术说明或正式性能数据。因此，具体的模型能力提升幅度、可用账户类型、区域限制和定价等信息，在给定内容中尚未明确。

hackernews · leumon · 9月15日 17:38 · [社区讨论](https://news.ycombinator.com/item?id=49715947)

**「背景」** Gemini Live 是 Google 面向实时语音对话的产品形态，此次发布的 Gemini 3.8 Live 与 3.8 Live Extended Thinking 属于该系列的新一代语音模型，后者提供“扩展思考”能力，即在给出回应前进行更长的推理。据 Google 官方博客与第三方报道，这两款模型面向开发者与企业开放，其中 3.8 Live Extended Thinking 还进入 Gemini Live 及 Google Workspace 应用（Docs、Gmail、Keep）等消费级入口，面向 Google AI Pro 与 Ultra 订阅用户；有报道称它们在语音基准测试中领先，并可在一次通话中处理 97 种语言。与本次公告相关的页面还列出 Gemini 3.8 Flash 与 3.8 Flash Cyber，定位为面向智能体工作流与网络安全的新一代模型。

**「影响」** 对实时语音与多模态应用开发者而言，Gemini 3.8 Live 的接口规格——16 位、16 kHz PCM 音频输入，24 kHz 音频输出，以及最高每秒一帧的 JPEG 视觉输入——会直接约束其音频管线与视觉采样频率的设计选择。现有证据仍以官方定位说明和用户主观反馈为主，尚无基准数据可判断这些模型在生产负载下的实际表现差异。

**「社区讨论」** 多位评论者称赞 Gemini Live Mode 的语音表现，称其口音适应好、声音自然、延迟低，并能用于 Workspace 账户；有用户认为它虽不如对手“聪明”，但体验已优于 GPT Voice，也有南非荷兰语使用者表示用它进行即兴会话和语法练习效果惊人。与此同时，有人抱怨 Google AI Plus 用户尚未获得 Gemini 3.8，另有人质疑 Google 仍落后于竞争对手，并追问 Gemini 4 何时发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/">Introducing Gemini 3.8 Live and 3.8 Live Extended Thinking</a></li>
<li><a href="https://officechai.com/ai/google-releases-gemini-3-8-live-extended-conversational-model-claims-better-performance-than-gpt-live-1-astra-and-grok-voice-think-fast-2-0-at-lower-price/">Google Releases Gemini 3.8 Live-Extended Conversational Model, Claims Better Performance Than Rivals At Lower Price</a></li>
<li><a href="https://aivy.com.au/news/gemini-3-8-live-launch/">After ChatGPT and Claude comes Gemini 3.8 Live</a></li>
<li><a href="https://shattered.io/gemini-3-8-live-extended-thinking-launch-2026/">Gemini 3 . 8 Live &amp; Extended Thinking : Google Voice AI [2026]</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/">Gemini 3 . 8 Live &amp; Gemini 3 . 8 Live Extended Thinking</a></li>

</ul>
</details>

**标签**: `#Google Gemini`, `#LLM release`, `#voice AI`, `#extended thinking`, `#AI models`

---

<a id="item-tech-news-2"></a>
### [SemiAnalysis：暂停令未实质性扼杀美国数据中心建设](https://newsletter.semianalysis.com/p/everyone-says-datacenter-moratoriums) ⭐️ 8.0/10

SemiAnalysis 在一篇分析中反驳了“数据中心暂停令正在扼杀美国建设”的流行说法。该分析称，虽然约有 20GW 的数据中心容量位于受限制的地方边界内，但真正发生进度滑落的只有约 1,525MW；若把纽约州纳入，全国范围内实际滑落约为 2.3GW。据此，作者认为暂停令对全美数据中心建设的影响有限，并没有像外界普遍宣称的那样造成实质性破坏。对于关注 AI 基础设施与电力约束的读者而言，这一结论提供了不同于主流叙事的量化视角，但其具体测算方法在现有摘要中并未展开。

rss · Semianalysis · 9月15日 20:54

**「背景」** 美国多地已针对新建数据中心推出暂停或限制性措施（moratorium），围绕这些措施是否正在实质性拖慢美国 AI 基础设施扩张，近期出现明显争论。SemiAnalysis 指出，若把受限区域内的规划容量简单相加，会高估实际影响，因为“位于受限边界内”并不等于项目真正延期。本文以纽约为例说明这种计算差异，而此前金融和社交媒体还广泛流传“2026 年美国近半数据中心容量将被取消或延期”的说法。

**「影响」** 对美国 AI 数据中心开发商和电网规划者来说，最具体的后果是：地方暂停令更像局部选址风险——SemiAnalysis 量化出受限边界内约 1,525 MW 滑期、含纽约全国约 2.3 GW 受影响——而不是全国建设停摆，但个别遭社区反对的项目仍可能被直接叫停。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/everyone-says-datacenter-moratoriums">Everyone Says Datacenter Moratoriums Are Killing the US Buildout. We ...</a></li>
<li><a href="https://newsletter.semianalysis.com/p/stop-saying-half-of-2026-us-datacenter">Stop Saying Half of 2026 US Datacenter Capacity Is Canceled</a></li>
<li><a href="https://www.datacenterknowledge.com/regulations/ai-data-center-moratorium-balancing-energy-community-and-growth-risks">AI Data Center Moratoriums: Balancing Energy, Community, and ...</a></li>
<li><a href="https://newsletter.semianalysis.com/p/everyone-says-datacenter-moratoriums">Everyone Says Datacenter Moratoriums Are Killing the US ...</a></li>

</ul>
</details>

**标签**: `#datacenter moratoriums`, `#AI infrastructure`, `#power constraints`, `#US datacenter buildout`, `#policy analysis`

---

<a id="item-tech-news-3"></a>
### [Typesafe.ai 发布 System One 模型与 Jev](https://typesafe.ai/blog/introducing-system-one-models-and-jev) ⭐️ 7.0/10

Typesafe.ai 在其博客发布文章，介绍 System One Models 与 Jev，将其定位为结构化、类型化推理的替代方案，而非通用生成。Hacker News 上的讨论集中在其适用范围以及与 LLM token 生成的对比，部分评论认为发布文章中的速度对比具有误导性。评论者 jacobgold 指出，Jev 似乎只能生成结构化输出，而一个能输出图灵完备代码的生成模型理论上可以完成计算机能做的任何事，因此 Jev 的优势更可能体现在分类等特定任务上。另有评论者称官方文档比公告解释得更清楚：模型接收状态输入与问题（如 yes/no、多选或评分），在毫秒级和低成本（$0.042/MTok）下输出选项、概率与置信度。不过这些细节来自评论者对文档的解读，公告本身未提供同等解释。

hackernews · albelfio · 9月15日 19:25 · [社区讨论](https://news.ycombinator.com/item?id=49717558)

**「背景」** System One Models 是 TypeSafe 推出的一类新模型，其代表 Jev 采用 System One 架构，并据称通过 RLCD 训练，旨在不逐 token 生成答案，从而以适合大规模生产的速度和成本进行推断。与通用生成模型不同，Jev 面向类型化/结构化推断：接收结构化输入（如文本或复杂 JSON）与问题，并直接返回类型化答案，而非自由生成文本。社区中已有项目（如 SIEGE）把 TypeSafe System One 用作“类型化动作门控”，以构建可靠的工作流。

**「影响」** 对需要用大模型做分类、打分或结构化决策的开发者，Jev 把这类任务从通用文本生成转向毫秒级、低成本的类型化推理，并以早期访问形式开放。但其“快两个数量级”和低成本优势目前来自厂商自测，社区也质疑与通用生成模型的速度对比是否公平，实际效果仍需独立验证。

**「社区讨论」** 评论总体认可这一思路的新意，但对速度对比是否公平存在分歧：jacobgold 认为 Jev 只能生成结构化输出，不能与能写图灵完备代码的通用模型直接比较。maltalex 和 big\_toast 等则批评公告解释不足、与 LLM token 的对比令人困惑，并建议以官方文档为准；还有评论者把它与契约式编程和 SymbolicAI 的实践联系起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://typesafe.ai/blog/introducing-system-one-models-and-jev">Introducing System One Models and Jev</a></li>
<li><a href="https://every.to/also-true-for-humans/mini-vibe-check-typesafe-s-jev-judged-everything-i-ve-written-in-0-7-seconds">Mini-Vibe Check: TypeSafe&#x27;s Jev Judged Everything I’ve Written in 0.7 Seconds</a></li>
<li><a href="https://github.com/vnmoorthy/siege">GitHub - vnmoorthy/siege: SIEGE: 200 people vs one agent. A typed action gate (TypeSafe System One) that learns from every breach, evaluated by W&amp;B Weave, hardened by a defender loop. Built at CoreWeave Hacks: Agent Loops 2026. · GitHub</a></li>
<li><a href="https://kamilstanuch.github.io/LLM-token-generation-simulator/">LLM Token Generation Speed Simulator &amp; Benchmark | Compare ... Introducing System One Models &amp; Jev - TypeSafe AI Blog LLM Leaderboard &amp; AI Model Benchmarks — September 2026 Fastest LLMs (September 2026): Tokens/sec and Latency ... LLM Speed Benchmark — Tokens Per Second Across 30 Models LLM Token Generation Speed: How Providers Compare in 2025 TypeSafe opens Jev early access for fast, typed AI decisions</a></li>
<li><a href="https://typesafe.ai/blog/introducing-system-one-models-and-jev">Introducing System One Models &amp; Jev - TypeSafe AI Blog</a></li>

</ul>
</details>

**标签**: `#AI models`, `#typed inference`, `#structured generation`, `#LLM tooling`, `#software engineering`

---

<a id="item-tech-news-4"></a>
### [电子墨水相框：用 BirdNET 听鸟鸣并画出 19 世纪风格插画](https://github.com/arnegiacomo/fugleramme) ⭐️ 7.0/10

开源项目 fugleramme 在 Hacker News 的 Show HN 板块亮相：它把电子墨水（e-ink）相框与 BirdNET 音频分类模型结合起来，识别周围鸟类的鸣叫，再把对应鸟类以 19 世纪插画风格绘制在屏幕上。代码托管在 GitHub，作者为 arnemunthekaas，作品属于嵌入式硬件、边缘端音频识别与复古视觉呈现的组合。评论者指出，其识别核心 BirdNET 是传统神经网络而非大语言模型，并给出了相应论文的 DOI 链接。这一项目并非重大技术突破或研究成果，但凭借创意与完成度在社区获得强烈反响。

hackernews · arnemunthekaas · 9月15日 12:31 · [社区讨论](https://news.ycombinator.com/item?id=49711544)

**「背景」** BirdNET 是一套用于鸟类声音识别的神经网络系统，其核心为卷积神经网络（CNN）：它把音频转成声谱图后，用训练好的权重匹配物种特征，可覆盖全球数千种鸟类；社区评论也特别指出，它是传统神经网络而非大语言模型。该项目 Fugleramme 运行在 Raspberry Pi 上，麦克风采集到的环境音频交给 BirdNET-Go，由后者调用 BirdNET 分类器并统一管理检测配置，全部推理均在本地完成，无需上传云端。显示端使用电子墨水屏——这类屏幕只在刷新时耗电，因此适合长期常驻、低频更新的展示场景；识别出的鸟种再以 19 世纪手工剪裁风格的鸟类插画呈现。此前 Hacker News 上还出现过同类项目「Avian Visitors」（2026 年 5 月，20 条评论），可见这一方向近期已有多次尝试。

**「影响」** 对已拥有树莓派和 Inky Impression 电子墨水屏的开发者与爱好者而言，Fugleramme 把 BirdNET-Go 的本地鸟类识别与既有硬件串成一条完全本地运行的展示链路，并提供管理页面来配置显示内容与自动更新；由于同一界面也能以网页形式在 HDMI 显示器或局域网内其他设备上呈现，实际部署并不强制要求电子墨水屏。

**「社区讨论」** Hacker News 评论几乎一致给予好评，称其是近期最令人兴奋的 HN 项目之一，认为它把多种想法融合成了带点“魔法感”的作品，并有人建议做成便于旅行携带的版本。讨论也补充了技术背景与实践经验：有人强调 BirdNET 是传统神经网络而非大语言模型并附上论文链接，有人分享用 ESP32 或 BTLE 驱动电子墨水屏、以 2000mAh 电池实现多年续航显示 KOReader 高亮摘录的经验，还有人指出近期鸟类识别项目明显增多，并提到 birdnet-go 等相关项目。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/birdnet">BIRDNet : Multifaceted Neural Network Systems</a></li>
<li><a href="https://birdnet.cornell.edu/">BirdNET – AI-Powered Sound ID</a></li>
<li><a href="https://github.com/arnegiacomo/fugleramme">GitHub - arnegiacomo/fugleramme: E-ink bird frame for ...</a></li>
<li><a href="https://arnegiacomo.dev/fugleramme/">Fugleramme - arnegiacomo.dev</a></li>
<li><a href="https://www.hackster.io/news/this-smart-picture-frame-shows-you-which-birds-are-outside-92a9b10bfddb">This Smart Picture Frame Shows You Which Birds Are Outside - Hackster.io</a></li>
<li><a href="https://github.com/vibragiel/fugleramme">GitHub - vibragiel/fugleramme: E-ink bird frame for Raspberry Pi - real-time bird detection by audio using BirdNET-Go · GitHub</a></li>
<li><a href="https://github.com/arnegiacomo/fugleramme">GitHub - arnegiacomo/fugleramme: E-ink bird frame for Raspberry Pi - real-time bird detection by audio, fully local AI, rendered as real, hand-cut 1800s bird illustrations. · GitHub</a></li>

</ul>
</details>

**标签**: `#e-ink displays`, `#BirdNET`, `#edge AI`, `#embedded systems`, `#open source`

---

<a id="item-tech-news-5"></a>
### [互联网档案馆更新 Wayback Machine 访问状况](https://blog.archive.org/2026/09/15/an-update-on-wayback-machine-access/) ⭐️ 7.0/10

互联网档案馆（Internet Archive）在官方博客发布了一篇关于 Wayback Machine 访问状况的更新，说明该服务近期遭遇多轮高流量自动化访问，并已部署防护措施以维持服务运行。社区评论中引述的内容显示，这些流量被怀疑来自试图绕过对原始网站封锁、转而抓取 Wayback Machine 存档副本的爬虫，讨论中还提到已有部分网站因此选择退出存档。现有材料没有给出具体限流机制、受影响范围或恢复正常的时间等细节。Wayback Machine 是提供免费历史网页存档的重要公共网络基础设施，因此其可用性变化受到关注。

hackernews · ChrisArchitect · 9月15日 17:52 · [社区讨论](https://news.ycombinator.com/item?id=49716176)

**「背景」** Wayback Machine 是 Internet Archive 运营的网页存档服务，用于回访已消失或发生变更的网页。Internet Archive 表示，该服务近期遭遇多波高流量自动化访问，因此部署了保护措施以维持运行。PCMag 报道称，这些旨在阻止自动化与滥用机器人的新防护也误伤了部分真实用户。

**「影响」** 对依赖 Wayback Machine 的研究者、记者和普通用户来说，这轮防护措施意味着访问可能继续出现间歇性失败或限流，而自动化抓取方会受到更强的访问约束；现有材料未说明服务何时恢复到稳定状态。

**「社区讨论」** Hacker News 讨论中，用户赞赏互联网档案馆在多方压力下仍维持开放访问（有人表示仍可经 Tor 匿名访问、不经中心化网关拦截），并呼吁捐款支持；同时有用户反映在工作网络中持续遇到 429 错误、而在其他网络访问正常，怀疑与自动化流量防护有关。也有评论谴责抓取存档以规避封锁的行为，并有人主张 AI 公司应为访问 Wayback Machine 付费。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.archive.org/2026/09/15/an-update-on-wayback-machine-access/">An Update on Wayback Machine Access | Internet Archive Blogs</a></li>
<li><a href="https://www.pcmag.com/news/why-is-the-internet-archive-blocking-users-blame-the-bots">Why Is the Internet Archive Blocking Users? Blame the Bots</a></li>

</ul>
</details>

**标签**: `#Internet Archive`, `#Wayback Machine`, `#web archiving`, `#open access`, `#web scraping`

---

<a id="item-tech-news-6"></a>
### [Show HN：20 美元 4G 热点改造成可发短信设备](https://bkovac.github.io/modem-thing/) ⭐️ 7.0/10

Show HN 上出现一个硬件改造项目，把约 20 美元的 4G 无线热点变成能发短信的 dumbphone，核心做法是复用 Clicks 键盘并运行 OpenStick 构建与开源固件。该项目的意义在于用低成本现成硬件和开源软件实现蜂窝短信能力，面向 maker 与嵌入式 Linux 爱好者。评论者迅速联想到类似设备：有人刚买了 10 美元 4G dongle，有人指出部分基于 MSM8916 的 dongle 虽无屏幕却运行 Android UI。讨论还延伸到把 18650 电池并联以延长数周续航，以及用热点设备查看短信和 OTP 的实际需求。由于未提供完整源码或实测数据，具体兼容性、功耗和稳定性仍待验证。

hackernews · bobili1234 · 9月15日 13:20 · [社区讨论](https://news.ycombinator.com/item?id=49712102)

**「背景」** 这类改造的技术底座是高通的 MSM8916 芯片，它被大量用于廉价的 4G USB 上网卡与热点设备，而 OpenStick 社区项目正是为这些 MSM8916 基带设备提供主线 Linux 支持；此外还有基于 postmarketOS 预编译内核的镜像构建工具，可生成 Debian 或 Alpine 系统。原厂设备通常运行 Android，但开箱即可通过 adb 访问，并能从 adb 直接进入 EDL 模式重新刷写固件，因此动手前需要先备份重要分区。项目还复用了 Clicks 物理键盘（原本是面向 iPhone 的实体按键配件）和 Sharp 记忆液晶屏，把热点变成可打字发短信的设备。

**「影响」** 对 maker 和嵌入式开发者来说，该项目提供了一个可复现的低成本思路：用约 20 美元 4G 热点、Clicks 键盘和 OpenStick 固件自制能发短信的极简设备。

**「社区讨论」** 评论普遍赞赏该改造，认为复用 Clicks 键盘是巧妙做法，并把它看作实用的迷你 cyberdeck 或 dumbphone。实际经验方面，有人提到自己常带热点而非手机上网，但查看短信和 OTP 仍需把 SIM 插回手机或打开笔记本 Web 界面；也有人提出并联两节高质量 18650 电池可把续航延长到数周，并好奇 OpenStick 的 RAM 与存储是否足以跑 Hermes Agent 等代理系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bkovac.github.io/modem-thing/">Converting a $20 4 G wireless hotspot into a texting device</a></li>
<li><a href="https://blog.adafruit.com/2026/09/15/converting-a-20-4g-wireless-hotspot-into-a-texting-device/">Converting a $20 4 G wireless hotspot into a texting device</a></li>
<li><a href="https://github.com/OpenStick">OpenStick Project · GitHub</a></li>
<li><a href="https://github.com/kinsamanka/OpenStick-Builder">GitHub - kinsamanka/OpenStick-Builder: Debian image builder for MSM8916 based 4G modem dongles · GitHub</a></li>
<li><a href="https://clicks.tech/">Clicks Keyboard case: transform your phone with buttons</a></li>

</ul>
</details>

**标签**: `#hardware hacking`, `#embedded Linux`, `#4G modems`, `#open source firmware`, `#DIY mobile devices`

---

<a id="item-tech-news-7"></a>
### [美国首次确认已部署太空武器](https://www.bbc.com/news/articles/ck790xg41ygro) ⭐️ 7.0/10

BBC 报道称，美国首次确认已部署太空武器，相关消息在 Hacker News 上引发讨论。由于提供的来源正文不可用，现有材料未给出具体武器类型、部署时间、数量或运行细节，缺乏超出标题和评论的技术深度。分析摘要指出，讨论集中在太空中立、轨道碎片风险以及军事航天技术。

hackernews · harporoeder · 9月15日 03:47 · [社区讨论](https://news.ycombinator.com/item?id=49707473)

**「背景」** 太空武器包括反卫星系统和定向能装置，1967 年《外层空间条约》禁止在轨道部署大规模毁灭性武器，但并未禁止其他类型的太空武器。美国现已首次确认其在地球轨道部署了一种进攻性太空武器，空军部长特洛伊·梅因克表示，这一“在轨”武器对于保护美国部队免受敌方敌对行动是必要的。太空碎片碰撞可能引发“凯斯勒效应”，即碎片连锁反应导致近地轨道在未来很长一段时间内无法使用，这也是此类部署引发担忧的原因之一。

**「影响」** 美国太空军正式确认在轨运行武器，意味着其对手与盟友都无法再假定轨道上不存在已部署的对抗系统。由于具体载荷、轨道位置和数量仍属机密，外部只能按最不利情形评估自身卫星与太空资产的安全性，这可能推动太空军备竞赛并加大凯斯勒综合征式的碎片风险。

**「社区讨论」** 评论者担忧太空军事化，认为太空应像南极一样保持中立，并警告轨道碎片可能触发凯斯勒效应、危及人类未来进入低轨的能力；也有人引用美国空军定向能局历史资料、激光试验设施以及航天飞机或迷你航天飞机的潜在反卫星能力来讨论相关技术渊源。另一些评论则嘲讽要求美国停止外空军备的官方表态，并提及里根与戈尔巴乔夫曾接近废除核武器，但美国不愿放弃太空武器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/ck790xg41ygro">US confirms for first time it has deployed space weapons</a></li>
<li><a href="https://www.youtube.com/watch?v=9N6YEUOv-dA">China and Russia warn of new arms race as US confirms it... - YouTube</a></li>
<li><a href="https://contentbuffer.com/news/us-space-force-deploys-space-control-weapons-into-orbit-ecae9886">US Space Force Deploys &#x27; Space Control Weapons &#x27; into Orbit</a></li>
<li><a href="https://www.firstpost.com/explainers/us-space-force-has-deployed-on-orbit-weapons-does-law-allow-it-14046059.html">US has deployed space weapons . Does law allow it?</a></li>

</ul>
</details>

**标签**: `#space weapons`, `#military technology`, `#space policy`, `#Kessler syndrome`, `#directed energy`

---

<a id="item-tech-news-8"></a>
### [Simon Willison 发布 Gemini Live 语音对话网页工具](https://simonwillison.net/2026/Sep/15/gemini-live/) ⭐️ 7.0/10

Simon Willison 发布了一个可在浏览器中试用 Google 当天推出的 Gemini 3.8 Live 与 3.8 Live Extended Thinking 语音到语音模型的网页工具，这两个模型在形态上与 OpenAI 的 GPT-Live 系列相似。据其说明，他把文档交给 GPT-6 Astra Extra High，由后者生成了这个 Web UI。界面支持选择模型与语音预设、填写可选的系统提示词，然后通过浏览器进行语音对话，并且可以在模型说话时打断它。该实现不依赖任何库，直接连接 wss://generativelanguage.googleapis.com/ws/google.ai.generativelanguage.v1alpha.GenerativeService.BidiGenerateContent?key=... 这个 WebSocket 端点，并用 Web Audio API 的 AudioContext 同时完成音频采集与播放。工具还提供转录文本的下载与清除、文本输入框（发送消息会打断当前回复），并提示转录内容可能包含播放前已被打断的语音。

rss · Simon Willison · 9月15日 22:47

**「背景」** Gemini Live 是 Google 面向实时语音对话的模型与 API 系列，开发者可通过 WebSocket 的 BidiGenerateContent 端点进行双向流式音频交互，并在浏览器中用 Web Audio API 完成采集与播放。Google 此次发布的 Gemini 3.8 Live 与 3.8 Live Extended Thinking 是新一代实时对话模型，前者面向低延迟、成本敏感的近实时对话并提供视觉基础能力，后者面向高复杂度的多步推理，整体形态与 OpenAI 的 GPT-Live 系列相似。

**「影响」** 对于构建实时语音代理的开发者来说，这意味着他们现在可以直接通过 Gemini API 和 Google AI Studio 接入 Gemini 3.8 Live 与 3.8 Live Extended Thinking，在维持对话的同时执行任务与工具调用。不过现有第三方基准仅公布了评测范围与指标，实际性能仍需独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-3-8-live-gemini-3-8-live-extended-thinking/">Gemini 3 . 8 Live &amp; Gemini 3 . 8 Live Extended Thinking</a></li>
<li><a href="https://zerohour.day/item/2f92a8ca47fb31cce7ea14f80f46a6a31b87d29e">Introducing Gemini 3 . 8 Live and 3 . 8 Live Extended Thinking</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/build-real-time-voice-applications-gemini-audio/">New Gemini Audio models for developers - The Keyword</a></li>
<li><a href="https://www.marktechpost.com/2026/09/15/google-releases-gemini-3-8-live-and-3-8-live-extended-thinking-for-production-grade-voice-agents/">Google Releases Gemini 3.8 Live and 3.8 Live Extended ...</a></li>
<li><a href="https://benchlm.ai/voice-benchmarks/gemini-3-8-audio-evaluation">Gemini 3.8 Audio model evaluation: Voice Benchmark Results ...</a></li>

</ul>
</details>

**标签**: `#Gemini Live`, `#speech-to-speech`, `#Google AI`, `#web UI`, `#developer tools`

---

<a id="item-tech-news-9"></a>
### [SHADOW-50M：44M 三值 LLM，19.8MB 跑在 CPU 约 1900 tok/s](https://www.reddit.com/r/MachineLearning/comments/1wgzpli/i_trained_a_44m_parameter_quantized_llm_from/) ⭐️ 7.0/10

r/MachineLearning 用户 /u/Final-Data-1410 发布了 SHADOW-50M：一个实际 44M 参数、在 45B tokens 上从零训练的三值权重 LLM，完整模型仅 19.8 MB，在笔记本 CPU 上约 1,900 tok/s、约 41 MB RAM，73,880 个 token 的词表由固定 512 位指纹而非训练嵌入表示，配 159 KB 编译内核，可完全离线运行，同一内核编译为 WebAssembly 后在浏览器中约 500 tok/s。该模型把计算与持久记忆单独处理：需要计算时输出形如 \[calc\]347\*86\[eq\] 的标记，由读出端的固定电路在同一 token 流中填入结果，覆盖算术、百分比、日期、星期、单位、计数、排序、比较和小型程序机；存储记忆时以每 token 288 字节（1 bit）把注意力状态写入磁盘，索引为 22 字节/token，不使用向量数据库或嵌入模型，100M token 的归档约 28.8 GB 加 2.2 GB 索引，而进程只占约 28 MB RAM（内存映射）。首个版本缺少约 8,600 个英文词片，作者未经训练直接把新行加入冻结指纹表，34/34 条此前公布答案保持不变，该表与人类词相似度评分的 Spearman 相关系数为 0.594（随机编码为 -0.057）。作者公开了与 51.8M 参数、bf16 的 Supra-50M-Reasoning 的对比：SHADOW 在所有测试的标准基准上更弱（ARC-Easy 0.307 对 0.435、PIQA 0.570 对 0.600、WikiText-2 困惑度 186 对 165），但在 11 个并排测试的算术、日期与检索问题上表现更好；其他实验包括用 Gemma 3 4B 生成的 298 条影片片段描述作为磁盘记忆答对 55-56/60、1,600 条记录清单得 159/160、作为 Qwen3-32B 草稿模型把 llama.cpp 从 19.7 提升到 28.5 tok/s，以及让 Qwen3-14B 经 MCP 记忆服务器 5/5 检索成功。作者强调这是概念验证而非产品，局限包括常识薄弱、创意写作不佳、七位数操作数偶尔复制错误、大归档偶尔拉入无关记录；代码为 MIT 许可，权重与微调/导出工具包公开，另有一个约 11,000 行、含 CUDA 引擎和内置 SHADOW 玩偶的 PR 尚待其验证后合并。

reddit · r/MachineLearning · /u/Final-Data-1410 · 9月15日 12:59

**「背景」** SHADOW-50M 是作者此前 SHADOW-250M 的延续：后者为 250M 参数、约 60 MB 部署、在笔记本 CPU 上约 400 tok/s 的离线模型，本次把规模压缩到 44M 参数，用于试验检索之后的推理与算术计算。所谓 ternary（三值）量化，是把权重限制在 \{-1, 0, +1\} 三个取值上，从而可用加法式稀疏 GEMM 等更廉价的计算替代乘法，降低边缘设备上的推理开销。与依靠训练得到的词嵌入不同，该模型用一张固定的 512 位指纹表表示 73,880 个词元，因此能在不重新训练的情况下直接向表中增补缺失词元；文中作为对照的 Supra-50M-Reasoning 则是 SupraLabs 的 51.8M 参数、Llama 式 bf16 推理模型。

**「对边缘与 CPU 推理开发者的影响」** 对边缘推理与量化实践者而言，SHADOW-50M 以 MIT 许可公开权重，展示了一条将三元权重、冻结的 512 位指纹词表和确定性读出电路结合、把算术与磁盘持久记忆检索压缩进约 20 MB 完全离线模型的可行路径。但作者自述的对比显示其在标准基准上低于 51.8M 的 bf16 基线（ARC-Easy 0.307 对 0.435、PIQA 0.570 对 0.600、WikiText-2 困惑度 186 对 165），且全部结果均为自报、尚无独立验证，因此应视为概念验证而非可广泛替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/QLNI/SHADOW-250M-Instruct">GitHub - QLNI/SHADOW-250M-Instruct: 250M parameter language model. 100M-token offline context. 60 MB deployment, 400 tok/s on a laptop CPU. · GitHub</a></li>
<li><a href="https://github.com/fpgasystems/ternaryLLM">GitHub - fpgasystems/ternaryLLM: Code for Fast Ternary Large Language Model Inference with Addition-Based Sparse GEMM on Edge Devices · GitHub</a></li>
<li><a href="https://huggingface.co/SupraLabs/Supra-50M-Reasoning">SupraLabs/Supra-50M-Reasoning · Hugging Face</a></li>

</ul>
</details>

**标签**: `#llm-efficiency`, `#quantization`, `#cpu-inference`, `#model-compression`, `#edge-ai`

---

<a id="item-tech-news-10"></a>
### [Prior Labs 发布 TabPFN-3.5 表格基础模型](https://www.reddit.com/r/MachineLearning/comments/1wh4xhy/tabpfn35_is_released_as_the_next_sota_tabular/) ⭐️ 7.0/10

Prior Labs 发布了新的表格基础模型 TabPFN-3.5，并称其在 TabArena 与 BeyondArena 两个基准上均排名第一，在 100 万行、最多 2 万个特征的数据规模上达到 SOTA。该版本包含三个变体：处于 alpha 阶段的 TabPFN-3.5-Fast 比基础模型快 6 倍，通过 API 提供的 TabPFN-3.5-Thinking 用更多算力换取更高精度，以及 TabPFN-3.5-Plus。在 BeyondArena 上，TabPFN-3.5 在文本密集、高基数和高维数据上领先，比此前最强基线高 250 Elo 分，比此前的总榜领先者高 150 Elo 分；Thinking 版本在 BeyondArena 上比基础模型高 20 Elo，在 TabArena 上高 44 Elo。上述排名与 Elo 数据目前仅来自 Reddit 发布帖，没有提供技术细节、论文或独立验证，应视为未经核实的作者自述结果。

reddit · r/MachineLearning · /u/tuanacelik · 9月15日 16:18

**「背景」** TabPFN 是 Prior Labs 开发的表格数据基础模型，其思路是用大量合成数据集进行预训练，使模型在推理时通过上下文学习直接完成表格预测，从而减少逐任务的特征工程与调参；它支持 Python 3.10+，并建议使用 GPU（约 8GB 显存即可，部分大数据集需要 16GB）。本条消息提到的 TabArena 与 BeyondArena 是用于比较表格模型的两个基准，其中 BeyondArena 更侧重文本丰富、高基数以及包含时间或分组切分的非独立同分布数据等实际场景。TabPFN-3.5 是继 TabPFN-3 之后的新旗舰版本，官方技术报告称其在上述更难的表格数据场景中提升最为明显。

**「影响」** 对处理表格数据的机器学习从业者而言，TabPFN-3.5 提供了一个在 TabArena 与 BeyondArena 上领先、并宣称覆盖 100 万行、最多 2 万特征规模的新默认候选，其 Thinking 变体通过 API 以算力换精度，Fast（alpha）据称比基础模型快 6 倍，直接影响模型选型与算力预算的权衡。不过 TabArena 的公开评测数据集规模约为 10 万行以内，百万行级的结论及 Elo 领先幅度目前仍缺乏独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://priorlabs.ai/technical-reports/tabpfn-3-5">TabPFN-3.5: Technical Report - Prior Labs</a></li>
<li><a href="https://github.com/PriorLabs/TabPFN">GitHub - PriorLabs/TabPFN: ⚡ TabPFN: Foundation Model for ...</a></li>
<li><a href="https://storage.googleapis.com/prior-labs-tabpfn-public/reports/tabpfn-v3.5-report.pdf">TabPFN-3.5: Technical Report - storage.googleapis.com</a></li>
<li><a href="https://www.emergentmind.com/topics/tabpfn-3">TabPFN - 3 : Scalable Transformer for Tabular Data</a></li>

</ul>
</details>

**标签**: `#tabular-data`, `#foundation-models`, `#machine-learning`, `#benchmarking`, `#TabPFN`

---

<a id="item-tech-news-11"></a>
### [工信部与发改委印发电子信息制造业“十五五”规划](https://www.secrss.com/articles/93961) ⭐️ 7.0/10

工业和信息化部、国家发展改革委联合印发《电子信息制造业发展“十五五”规划》，部署 17 项重点任务。规划提出提高先进制程能力，突破高端手机核心芯片和 PC 高性能芯片，并加强开源鸿蒙等国产操作系统搭载。到 2030 年，规模以上企业营业收入目标突破 30 万亿元，产业研发投入强度达到 3.5%。规划还明确推进 RISC-V、人工智能芯片和终端、北斗等领域发展；目前公开摘要未披露具体实施细节，实际推进节奏和达标条件仍待后续文件明确。

telegram · zaihuapd · 9月15日 03:10

**「背景」** 《电子信息制造业发展“十五五”规划》由工业和信息化部、国家发展改革委联合印发，属于中国以五年为周期部署重点产业方向的专项规划，覆盖“十五五”时期并设定了到 2030 年的产业发展目标。此前“十四五”期间，中国电子信息制造业营业收入连续 13 年在 41 个工业大类中位居第一，集成电路、服务器、新型显示、人工智能终端和北斗规模应用等已有新进展，这构成了此次规划提出提高先进制程能力、突破高端手机核心芯片和 PC 高性能芯片、加强开源鸿蒙等国产操作系统搭载等任务的产业背景。规划同时提出到 2030 年规模以上企业营业收入突破 30 万亿元等量化目标，以承载上述方向。

**「影响」** 该规划为国内先进制程、高端手机与 PC 芯片、开源鸿蒙及 RISC-V 生态的相关厂商和开发者设定了到 2030 年的政策目标（规上企业营收超 30 万亿元、研发投入强度 3.5%），并将高带宽内存池、全光交换、液冷散热、CLink 互连总线等列为关键技术方向，可能影响其技术路线与产品规划。不过规划未公开具体实施路径与资金安排，实际落地节奏仍待观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260915/herald/0c88d9f6e17390cede0285f9f02903ed.html">电子信息制造业发展“十五五”规划出炉！两部门：推动集成电路全链条攻关 - 21经济网</a></li>
<li><a href="https://k.sina.cn/article_1652484947_627eeb530200208ds.html">电子信息制造业发展“十五五”规划发布|国家发展改革委|工业和信息化部|信息化部|消费电子|工信部_新浪新闻</a></li>
<li><a href="https://cn.investing.com/news/stock-market-news/article-3566265">电子信息制造业发展“十五五”规划发布：到2030年规上企业营收将突破30万亿元 提供者 智通财经</a></li>
<li><a href="http://3g.cnfol.com/sc_stock/gushijujiao/20260915/32370146.shtml">30万亿蓝图出炉！ AI...</a></li>
<li><a href="https://fund.eastmoney.com/a/202609153874514129.html">30万亿蓝图出炉！ AI...</a></li>

</ul>
</details>

**标签**: `#China tech policy`, `#semiconductors`, `#open-source OS`, `#RISC-V`, `#AI chips`

---

<a id="item-tech-news-12"></a>
### [谷歌向全员工程师开放 Claude Opus 5 用于内部开发](https://www.businessinsider.com/google-finally-lets-all-engineers-use-anthropics-claude-2026-9) ⭐️ 7.0/10

据 Business Insider 报道，谷歌已向全公司工程师开放 Anthropic 最强的编程模型 Claude Opus 5，用于内部开发，但只能通过其内部开发平台 Antigravity 使用。此前谷歌通常禁止大多数员工使用 Claude Code、OpenAI Codex 等外部编程工具，要求他们改用自家 Gemini。谷歌发言人表示，Gemini 仍是内部开发的主要模型，Claude 按每位员工配额提供，作为补充。此举被视为对 AI 编码竞争压力的回应；谷歌是 Anthropic 的投资者，并曾于今年早些时候宣布计划向该公司投入最多 400 亿美元。

telegram · zaihuapd · 9月15日 05:31

**「背景」** 谷歌此前通常禁止大多数员工使用 Claude Code、OpenAI Codex 等外部编程工具，要求内部开发以自研的 Gemini 为主要模型，这构成了此次政策调整的背景。谷歌同时是 Anthropic 的投资者，今年早些时候宣布计划向该公司投入最多 400 亿美元，而 Claude 此次只通过谷歌内部开发平台 Antigravity 开放，并按每位员工配额提供，定位为 Gemini 之外的补充。

**「影响」** 对谷歌内部工程师而言，最直接的变化是他们可以在 Antigravity 平台内按个人配额调用 Claude Opus 5 处理编码任务，而不再像过去那样被要求只使用自家工具，但 Gemini 仍被官方定位为内部开发的主力模型，Claude 只是补充。这一安排也表明，在 AI 编码工具的竞争压力下，谷歌已承认外部模型值得引入内部流程，不过是否会扩展到 Claude Code、Codex 等其他外部工具，目前尚无证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digg.com/tech/04cff254-0da4-4396-8105-4c12e0f47c90">Google grants broader internal access to Anthropic &#x27;s Claude amid...</a></li>
<li><a href="https://promtime.net/p/en/post/claude-got-into-google-but-only-through-antigravity">Claude got into Google , but only through Antigravity · News</a></li>
<li><a href="https://trak.in/stories/google-finally-allows-all-engineers-to-use-anthropics-claude-for-coding/">Google Finally Allows All Engineers to Use Anthropic ’s Claude for...</a></li>
<li><a href="https://www.businessinsider.com/google-finally-lets-all-engineers-use-anthropics-claude-2026-9">Google finally lets all engineers use Anthropic&#x27;s Claude</a></li>
<li><a href="https://docs.cloud.google.com/gemini-enterprise-agent-platform/models/partner-models/claude/opus-5">Claude Opus 5 on Google Cloud | Gemini Enterprise Agent ...</a></li>

</ul>
</details>

**标签**: `#AI coding assistants`, `#Google`, `#Anthropic`, `#enterprise AI adoption`, `#developer tools`

---

<a id="item-tech-news-13"></a>
### [联发科发布天玑 9600 Pro：首款台积电 2nm 手机芯片](https://www.reuters.com/business/media-telecom/mediatek-launches-new-mobile-chip-using-tsmcs-most-advanced-technology-2026-09-15/) ⭐️ 7.0/10

联发科于 9 月 15 日发布旗舰手机芯片天玑 9600 Pro，采用台积电 2 纳米制程，成为该公司首款使用这一制程的手机处理器；同日发布的还有采用 3 纳米制程的天玑 9600M。联发科表示，搭载这两款芯片的首批手机将很快上市。天玑 9600 Pro 配备专用 AI 处理器，联发科称其处理用户提示词、启动模型生成前的性能较上一代提升 51%。上述性能提升目前为联发科公布的数据，缺乏独立测试验证。

telegram · zaihuapd · 9月15日 08:57

**「背景」** 纳米（nm）数是半导体制造工艺节点的代称，数值越小通常意味着晶体管密度更高、同性能下功耗更低，2nm 被视为继 3nm 之后的下一代先进制程，目前由台积电等代工厂推进量产。联发科长期与台积电在移动芯片制程上合作，其天玑系列此前主要基于 3nm 及更早节点，此次天玑 9600 Pro 是其首款 2nm 手机处理器，同期发布的天玑 9600M 则仍采用 3nm；按联发科说法，该公司是首家宣布跨入这一节点的厂商。随着手机端本地运行大模型成为卖点，芯片厂商开始在 SoC 中集成专用 AI 处理单元，用于加速提示词处理等推理环节，这也是本次发布强调 51% 提示词处理性能提升的背景。

**「影响」** 天玑 9600 Pro 让联发科首次以台积电 2nm 旗舰平台参与高端手机竞争，为其手机厂商合作伙伴提供了新的顶级芯片选择，并加大了对高通在高端机型市场份额的压力。其 51% 的提示词处理提升目前为联发科自述数据，终端实际表现仍待产品上市后验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5google.com/2026/09/15/mediatek-dimensity-9600-pro-chip/">MediaTek Dimensity 9600 Pro debuts with 2nm, performance gains</a></li>
<li><a href="https://www.mediatek.com/press-room/mediatek-dimensity-9600-pro-sets-new-standard-for-flagship-smartphone-chips">MediaTek Dimensity 9600 Pro Sets New Standard for Flagship ...</a></li>
<li><a href="https://www.gizguide.com/2026/09/mediatek-dimensity-9600-pro-launched.html">MediaTek Dimensity 9600 Pro launched: 2nm process, Mali-G2 ...</a></li>
<li><a href="https://www.mediatek.com/press-room/mediatek-dimensity-9600-pro-sets-new-standard-for-flagship-smartphone-chips">MediaTek Dimensity 9600 Pro Sets New Standard for Flagship ...</a></li>
<li><a href="https://www.taipeitimes.com/News/biz/archives/2026/09/16/2003864324">MediaTek releases Dimensity 9600 Pro mobile chip - Taipei Times</a></li>

</ul>
</details>

**标签**: `#MediaTek`, `#Dimensity 9600 Pro`, `#TSMC 2nm`, `#mobile SoC`, `#AI processor`

---

<a id="item-tech-news-14"></a>
### [404 Media：OpenAI“Project Lily”由数百名合同工阅读 ChatGPT 对话](https://www.404media.co/inside-project-lily-the-humans-reading-your-chatgpt-chats/) ⭐️ 7.0/10

404 Media 报道称，OpenAI 正通过名为“Project Lily”的项目雇用数百名合同工，阅读大量真实用户的 ChatGPT 提示词及完整对话，并为模型回复评分、提出修改意见，其中可能包含敏感个人信息。OpenAI 表示会在内容交给审核员前尽量删除个人信息，但承认敏感细节仍可能被看到。Anthropic 也确认使用人工审核来改进模型。该报道把大模型训练与回复评估中的人工数据审查实践及其隐私影响推到了公众视野中。

telegram · zaihuapd · 9月15日 11:56

**「背景」** ChatGPT 目前拥有超过 9 亿用户，而控制对话是否可用于模型改进的退出选项在 Free、Plus 和 Pro 账户中均默认开启，多数用户可能并不知道自己的对话会被人工查看。据 404 Media 报道，“Project Lily”是 OpenAI 内部的项目代号，其实施方式是由 Crossing Hurdles 招募合同工、通过 Mercor 支付报酬，把真实用户提示词分发给人工审核员，由后者总结用户意图并在 1 到 7 分的量表上为多个模型回复打分。用人工审核来改进模型在 AI 行业并非孤例，Anthropic 也确认采用类似做法。

**「对用户的影响」** 对日常使用 ChatGPT 的用户来说，这意味着看似私密的一对一对话内容可能在删除部分个人信息后仍被数百名外部合同工逐条阅读并评分，敏感细节存在被看到的实际风险；据相关报道，用户可通过关闭数据共享（opt out）来限制此类用途，但该选项对本已进行的审核是否有效尚不明确。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.404media.co/inside-project-lily-the-humans-reading-your-chatgpt-chats/">Inside ‘Project Lily’: The Humans Reading Your ChatGPT Chats</a></li>
<li><a href="https://aiweekly.co/alerts/404-media-openai-project-lily-hires-hundreds-of-contractors-to-read-real">404 Media: OpenAI &#x27;Project Lily&#x27; Hires Hundreds of ...</a></li>
<li><a href="https://tech.yahoo.com/ai/chatgpt/articles/chatgpt-chats-may-read-humans-154948211.html">Your ChatGPT Chats May Be Read by Humans. Meet Project Lily.</a></li>
<li><a href="https://theoutpost.ai/news-story/open-ai-contractors-read-real-chat-gpt-conversations-under-project-lily-raising-privacy-alarms-30851/">OpenAI &#x27;s Project Lily : Humans Reading ChatGPT Chats</a></li>
<li><a href="https://www.remio.ai/post/openai-project-lily-puts-human-review-behind-chatgpts-private-looking-conversati">OpenAI Project Lily Puts Human Review Behind...</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/chatgpt-transcripts-are-reportedly-read-by-humans-to-improve-responses-including-those-with-personal-information-project-lilly-has-seen-openai-hire-hundreds-of-contractors-to-manually-review-logs">ChatGPT transcripts are reportedly read by humans ... | Tom&#x27;s Hardware</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#data privacy`, `#AI labor`, `#human review`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国 8 月零售增长不及预期，投资降幅加深](https://www.cnbc.com/2026/09/15/china-august-retail-sales-industrial-output-investment-exports-.html) ⭐️ 8.0/10

中国 8 月社会消费品零售总额同比增长 0.4%，低于路透调查经济学家预期的 0.8%，也较 7 月的 0.6%放缓；1-8 月城镇固定资产投资同比收缩 7.2%，降幅比 1-7 月的 6.7%加深。同期工业增加值增长 5.2%，超过预期的 4.8%，但 8 月新增人民币贷款仅 600 亿元（约 89.5 亿美元），远低于约 4000 亿元的预期，信贷扩张明显不及预期。

rss · CNBC Finance · 9月15日 09:46

**「背景」** 中国二季度 GDP 增速已放缓至 4.3%，为三年多来最弱，而今年官方增长目标为 4.5%至 5%。国家统计局称国内“供给强、需求弱”的失衡突出，呼吁加大宏观政策调整、提振内需。

**「影响」** 家庭和企业借贷需求疲弱、投资收缩加深，可能进一步拖累依赖国内需求的行业。

**标签**: `#China economy`, `#retail sales`, `#fixed-asset investment`, `#credit growth`, `#macro policy`

---

<a id="item-finance-news-2"></a>
### [报道称字节跳动 2026 上半年净利润降至约 200 亿美元](https://finance.sina.com.cn/jjxw/2026-09-15/doc-inirxpiq6857286.shtml) ⭐️ 7.0/10

据外媒报道（新浪财经援引），字节跳动 2026 年上半年净利润降至约 200 亿美元，同比下降，净利润率约 16.7%，报道称主要原因是 AI 领域的大规模投入。同期营收同比增长 30%，字节跳动对上述数据未予置评。

telegram · zaihuapd · 9月15日 15:59

**「背景」** 字节跳动并非上市公司，通常不公开披露完整财报，因此其利润与营收数据多由媒体引述知情人士报道——此次约 200 亿美元净利润等数字来自 The Information 的报道，字节跳动未予置评。

**「影响」** 据媒体报道，字节跳动已将 2026 年 AI 资本开支提高至约 300 亿美元，并讨论把年度资本开支上限推高至 700 亿美元，用于数据中心等 AI 基础设施建设；若这些支出按计划落地，数据中心、服务器与芯片等 AI 基础设施供应商将持续获得订单。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eu.36kr.com/en/p/3968472279806210">$29.6B AI Investment: Major Industry Giant Places Massive Bet on...</a></li>
<li><a href="https://www.linkedin.com/posts/konekt-ai_bytedance-tiktok-aiinfrastructure-activity-7460335625519538176-xNTW">ByteDance Boosts AI Infrastructure Investment by 25% to... | LinkedIn</a></li>

</ul>
</details>

**标签**: `#ByteDance`, `#AI investment`, `#earnings`, `#TikTok`, `#tech industry`

---