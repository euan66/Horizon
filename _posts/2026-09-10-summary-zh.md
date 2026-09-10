---
layout: default
title: "Horizon Summary: 2026-09-10 (ZH)"
date: 2026-09-10
lang: zh
---

> 从 41 条内容中筛选出 10 条重要资讯。

---

**科技新闻**
1. [Calif Research 称用 AI 两天写出微信通话零点击蠕虫](#item-tech-news-1) ⭐️ 9.0/10
2. [Shopify 从 React Native 回归 Swift 与 Kotlin](#item-tech-news-2) ⭐️ 8.0/10
3. [微软将 Rust 列为一级语言](#item-tech-news-3) ⭐️ 8.0/10
4. [蚂蚁国际联合 Visa 与 Mastercard 制定 AI 代理支付标准](#item-tech-news-4) ⭐️ 8.0/10
5. [DeepSeek 发布 V4.1 Flash：552B 参数多模态模型上线 API](#item-tech-news-5) ⭐️ 7.0/10
6. [腾讯混元发布开源音频编辑模型 AuK](#item-tech-news-6) ⭐️ 7.0/10

**科技博客**
1. [跟随瓶颈：在 AMD MI355X 上优化 MiniMax M3](#item-tech-blog-1) ⭐️ 9.0/10
2. [vLLM 分层 KV 缓存卸载：以主机内存为中心的设计](#item-tech-blog-2) ⭐️ 8.0/10

**财经新闻**
1. [Kalshi launches ‘perps’ for gold and silver following CFTC approval, expanding futures offerings](#item-finance-news-1) ⭐️ 7.0/10
2. [中国 AI 芯片厂商因 HBM 短缺上调价格](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Calif Research 称用 AI 两天写出微信通话零点击蠕虫](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

安全研究机构 Calif Research 发布了一段 WeWorm 演示，声称这是首个通过微信通话在 iOS 和 Android 上传播的零点击蠕虫。按其描述，受害者无需接听电话、也无需对手机做任何操作；即使接听，也听不到任何声音，漏洞利用依然成功。该团队表示，他们借助 AI 在大约两天内找到漏洞并写出首个远程代码执行（RCE）利用程序，随后又用一周时间构建出蠕虫，并称过去这种规模的蠕虫通常需要更大团队花费数月，人类只负责选择目标与安全测试的判断。Simon Willison 引用了这一发布内容。需要注意，上述说法目前仅来自该研究团队的自行发布，除被引用的内容外尚无独立验证。

rss · Simon Willison · 9月10日 00:56

**「背景」** 零点击（zero-click）漏洞指攻击者无需受害者进行任何交互就能完成利用，而蠕虫（worm）是能自我复制、借助受害者通讯录等渠道自动向外传播的恶意软件，两者结合意味着仅一通来电就可能让恶意代码自行扩散并劫持账户。WeChat 是用户规模以亿计的即时通讯应用，其语音通话与联系人列表横跨 iOS 和 Android，正是 WeWorm 声称利用的传播面。Calif Research 此次公开的是 WeWorm 的演示，相关说法来自其自行发布的研究页面与博客，目前尚无第三方独立验证。

**「影响」** 若该演示所述成立，iOS 与 Android 上的微信用户只需接到一通来电，账号就可能在数秒内被接管，并被用于向通讯录好友继续传播。但上述后果目前仅基于 Calif Research 的演示发布，尚未获得独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://calif.io/research/weworm">WeWorm | Calif</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">&quot;Zero-click&quot; WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>
<li><a href="https://blog.calif.io/p/weworm">WeWorm</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">&quot;Zero-click&quot; WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>
<li><a href="https://cybersecuritynews.com/weworm-first-0-click-worm/">WeWorm - First 0-Click Worm Spreading Through WeChat Calls Across iOS and Android</a></li>
<li><a href="https://www.theregister.com/security/2026/09/09/wechat-worm-could-pwn-a-friend-before-they-even-answered-the-call/5295234">WeChat worm could pwn a friend before they even answered the call</a></li>

</ul>
</details>

**标签**: `#AI security`, `#zero-click exploit`, `#WeChat`, `#remote code execution`, `#mobile worm`

---

<a id="item-tech-news-2"></a>
### [Shopify 从 React Native 回归 Swift 与 Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify 工程团队发布文章，讲述其移动应用从 React Native 迁回原生 Swift 和 Kotlin 的历程。这一迁移值得关注，因为一家大型商业公司公开复盘了跨平台方案与原生移动开发之间的权衡。文章在 Hacker News 上引发大量讨论，焦点包括团队资源、Web 开发者转移动端以及是否继续使用 React Native 等工程决策。目前可见的一手内容有限，具体迁移原因、版本、时间和性能数据尚不清楚。

hackernews · fnthawar2 · 9月10日 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49643982)

**「背景」** React Native 是 Meta 推出的跨平台移动框架，允许用 JavaScript/React 编写一套代码同时运行在 iOS 和 Android 上；Shopify 在 2020 年宣布将其作为移动端未来，以避免为两个平台重复开发功能。该团队在 2025 年 1 月还发布《Five years of React Native at Shopify》，称框架前景光明并计划继续投入。如今 Shopify 决定将全部移动应用迁回独立的 Swift 与 Kotlin 原生代码库，官方将这一转向归因于编码智能体大幅降低了同时构建和维护两个原生平台的成本。

**「影响」** 对正在评估跨平台与原生路线的移动团队来说，这一案例会被用来讨论 React Native 的适用边界，但社区评论强调它更像是取决于资源、产品阶段与团队构成的工程权衡，而非普适结论。

**「社区讨论」** 评论者从不同角度讨论此事：有人将其视为取决于公司资源与问题的普通工程取舍；有人认为 AI 生成代码削弱了 React Native 复用 Web 开发者的优势，并分享用 Codex 和 Maestro 将约 15–20 个屏幕的 RN 应用快速转成 Android/iOS 原生的实践。另有用户批评 Shopify 的 Shop 应用、结账入口和包裹追踪体验，表示因此会避免购买。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>
<li><a href="https://dev.to/jamilxt/shopify-is-moving-its-mobile-apps-back-to-native-coding-agents-made-it-cheaper-to-build-twice-than-4bf9">Shopify Is Moving Its Mobile Apps Back to Native. Coding ...</a></li>
<li><a href="https://picx.dev/news/LsT33N">Shopify moves from React Native back to native Swift and ...</a></li>

</ul>
</details>

**标签**: `#React Native`, `#Swift`, `#Kotlin`, `#mobile development`, `#cross-platform engineering`

---

<a id="item-tech-news-3"></a>
### [微软将 Rust 列为一级语言](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

根据 Rust 基金会发布的客座文章，微软已将 Rust 定为一级（tier-1）语言，这意味着 Rust 在其系统编程生态中获得一等支持。这一举措被视为主要操作系统与工具链厂商对 Rust 成熟度的正式认可，并可能影响微软系统级开发以及 C/C++ 代码迁移。社区讨论特别关注 MSVC 后端整合的传闻，以及用 Rust 改善内存安全、减少相关 CVE 的潜力。现有材料未提供该决定的具体适用范围、生效时间或配套路线图。

hackernews · mmastrac · 9月10日 13:39 · [社区讨论](https://news.ycombinator.com/item?id=49643546)

**「背景」** 在微软这类平台厂商内部，编程语言通常按官方支持等级划分，“Tier-1（一线）”意味着该语言在生产环境的开发中获得完整的官方支持，覆盖工具链、构建流程以及安全与质量审查环节。Rust 目前已被列为这一等级，但据相关报道，经过数十年积累的 C++ 仍在微软的系统中占据主导地位。这一调整也与业界近年倾向于用内存安全语言减少缺陷（尤其是内存安全类漏洞）的方向相符，因此 Rust 与 C++、C\# 等既有语言之间的定位对比成为讨论焦点。

**「影响」** 对 Windows 平台与 MSVC 工具链上的开发者而言，Rust 被列为 Microsoft 一级语言意味着编译器后端、工具链与库支持将从试验性支持转为与 C/C++ 并列的长期投入，现有构建、调试与依赖流程可能随之调整。需要注意的是，微软内部「2030 年前消除 C/C++」的目标目前主要来自公开招聘与公开表态，实际落地范围与时间表仍不确定。

**「社区讨论」** 评论总体积极，认为这表明 Rust 已从新兴语言走向能与 C++/C\# 竞争的成熟系统语言，且主要操作系统厂商都在为系统编程语言多元化。讨论中有人引用微软到 2030 年转换 10 亿行代码、DARPA 自动化 C 到 Rust 等项目，并强调 MSVC 后端取代 LLVM 是重要看点；也有评论关注大规模迁移与内存安全 CVE 治理的实际挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://qatrial.com/developer-open-source/rust-is-tier-1-language-at-microsoft/">Rust Is Tier-1 Language At Microsoft - QAtrial</a></li>
<li><a href="https://lobste.rs/s/eerwba/rust_is_tier_1_language_at_microsoft">Rust Is Tier-1 Language at Microsoft | Lobsters</a></li>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://windowsforum.com/news/microsoft-aims-2030-rust-migration-for-c-and-c-with-ai-tools.394765/">Microsoft Aims 2030 Rust Migration for C and C++ with AI Tools</a></li>
<li><a href="https://www.theregister.com/software/2025/12/24/microsoft-wants-to-replace-its-entire-c-and-c-codebase/2339230">Microsoft wants to replace its entire C and C++ codebase</a></li>

</ul>
</details>

**标签**: `#Rust`, `#Microsoft`, `#systems programming`, `#memory safety`, `#programming languages`

---

<a id="item-tech-news-4"></a>
### [蚂蚁国际联合 Visa 与 Mastercard 制定 AI 代理支付标准](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html) ⭐️ 8.0/10

蚂蚁国际宣布与 Visa、Mastercard 合作，为 AI 代理支付制定通用标准，三方将建立“了解你的代理”机制，用于把代理关联到有效实体、评估其行为并监测风险，以提升不同支付系统之间的互操作性和安全性。三方援引麦肯锡的预测称，到 2030 年 AI 代理可能处理全球消费者商业交易中的 3 万亿至 5 万亿美元。这一跨行业合作涉及主要支付网络，被视为可能影响 AI 系统与金融基础设施的行业性动作。目前公开信息仅为简要新闻摘要，未披露标准的具体技术细节、时间表或独立验证情况。

telegram · zaihuapd · 9月10日 03:00

**「背景」** AI 代理支付指的是由自主运行的 AI 智能体代替用户发起并完成交易的场景，这类交易要求支付方能够确认“是谁在替我付钱”。此前各家支付网络对代理的身份核验、授权与责任归属缺乏通用规则，代理在一家支付机构完成注册后，往往还需要在其他机构重复注册，跨网络互操作因此受限。此次三方提出的“了解你的代理”（Know Your Agent）机制，目的正是把每个代理关联到有效实体、评估其行为并持续监测风险，从而让注册信息可在参与方之间互认。

**「影响」** 若该标准最终落地，开发面向消费者的 AI 代理的开发者与受理商户将需要接入统一的代理身份关联与风险评估机制，才能跨 Visa、Mastercard 等不同支付网络完成代理发起的交易。目前三方仅公布合作意向，“了解你的代理”机制的具体规则与实施时间表尚未披露，实际约束力仍待观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html">Ant International, Visa and Mastercard team up on AI payment standard</a></li>
<li><a href="https://crypto.news/ant-international-joins-visa-mastercard-to-build-ai-agent-payment-standards/">Ant International joins Visa, Mastercard to build AI agent payment standards</a></li>
<li><a href="https://bitcoinethereumnews.com/tech/ai-agent-payment-standards-set-by-visa-mastercard-ant/">AI Agent Payment Standards Set by Visa, Mastercard, Ant</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#payment standards`, `#fintech`, `#interoperability`, `#risk management`

---

<a id="item-tech-news-5"></a>
### [DeepSeek 发布 V4.1 Flash：552B 参数多模态模型上线 API](https://mp.weixin.qq.com/s/qg0NU3NNUbp1co2PdkAPAg) ⭐️ 7.0/10

DeepSeek 宣布正式发布 V4.1 Flash，称其为全新模型结构系列中尺寸最小的模型，采用 552B 参数的 Causal-Encoder-Decoder 结构，输入与输出激活分别为 8B 和 16B，并原生支持多模态视觉理解。该模型已上线 DeepSeek API，模型名为 deepseek-flash，新价格自 2026 年 9 月 10 日 12:00 起生效。自 9 月 14 日 12:00 之后，deepseek-v4-pro 的请求将被路由至 V4.1 Flash，并按其价格计费。需要说明的是，该消息为简短转发式公告，未附带基准测试数据、技术论文或独立与官方渠道的额外确认，因此上述架构与定价细节仍有待进一步核实。

telegram · zaihuapd · 9月10日 05:54

**「背景」** DeepSeek 此前的主力是 V4-Pro 等旗舰模型，而 V4.1 Flash 属于其全新推出的 Causal-Encoder-Decoder（因果编码器-解码器）架构系列，是该系列中尺寸最小的模型。该架构将输入与输出阶段的激活参数分别控制在 8B 和 16B，同时保留 552B 的骨干参数总量，属于以稀疏激活降低推理开销的路线（tool-1-1、tool-1-3）。据 DeepSeek 官方介绍，新的预训练方法配合更大规模的强化学习后训练，使其在部分基准上超过包括 DeepSeek-V4-Pro 在内的旗舰模型，并原生支持图文输入与 1M token 上下文；该模型也已出现在 Hugging Face 上（tool-1-1、tool-1-2、tool-1-3）。

**「影响」** 对使用 DeepSeek API 的开发者而言，自 2026 年 9 月 14 日 12:00（北京时间）起，deepseek-v4-pro 的请求将全部被路由至 V4.1 Flash 并按 Flash 价格计费，直至 V4.1 Pro 未来发布为止，现有依赖 v4-pro 的应用会在无需改动代码的情况下切换到不同架构与参数规模的模型。据第三方整理的信息，新价格在非高峰时段为缓存命中输入每百万 token 0.02 元、缓存未命中输入 1 元、输出 4 元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.deepseek.com/en/news/deepseek-v4-1-flash/">DeepSeek | Introducing DeepSeek-V4.1-Flash: smarter, faster, more efficient.</a></li>
<li><a href="https://www.progressiverobot.com/2026/09/10/deepseek-v4-1-flash-552b-moe-model-hugging-face/">DeepSeek V4.1 Flash: Powerful 552B MoE at a Surprising Price</a></li>
<li><a href="https://benchlm.ai/models/deepseek-v4-1-flash">DeepSeek V4.1 Flash Benchmarks &amp; Pricing (September 2026)</a></li>
<li><a href="https://api-docs.deepseek.com/quick_start/pricing/">Models &amp; Pricing | DeepSeek API Docs</a></li>
<li><a href="https://technode.com/2026/09/10/deepseek-formally-launches-v4-1-flash-routes-v4-pro-requests-to-flash/">DeepSeek formally launches V4.1 Flash, routes V4 Pro requests to Flash · TechNode</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#large language models`, `#multimodal AI`, `#model release`, `#API pricing`

---

<a id="item-tech-news-6"></a>
### [腾讯混元发布开源音频编辑模型 AuK](https://x.com/TencentHunyuan/status/2097996926876795197) ⭐️ 7.0/10

腾讯混元宣布正式发布开源音频编辑模型 AuK，可通过自然语言指令与参考音频统一完成语音生成和编辑。该模型支持零样本文本转语音、音色/风格/情绪编辑、去口音以及多人语音分离等功能。腾讯混元同时发布 AuK-Flash，采用 4 步推理，在匹配条件下速度约提升 4.5 倍。目前代码、模型权重和演示均已上线。官方公告未披露模型规模、基准测试细节与许可条款，这些信息仍待补充。

telegram · zaihuapd · 9月10日 11:56

**「背景」** 语音生成与语音编辑长期是两条技术路线：文本转语音（TTS）负责从文本合成语音，语音编辑则负责修改已有录音的音色、风格或情绪。其中“零样本”指只用一小段参考音频就能复现未见过的说话人音色，无需针对该说话人重新训练；而统一模型则试图用同一套权重、以自然语言指令同时完成生成与编辑。扩散与流匹配类音频模型通常需要数十步迭代推理，因此把步数压缩到个位数的少步推理方案，是当前降低音频生成延迟与算力成本的常见思路。

**「影响」** 对语音与音频应用开发者来说，AuK 以 1.5B 参数规模、MIT 许可开放代码与权重，可直接用于构建零样本 TTS、内容与音色编辑、语音增强及声源分离等自托管流程，而 AuK-Flash 的 4 步推理约 4.5 倍加速有助于压低实时场景的推理成本。由于官方未披露基准测试与更细的性能对比，实际效果仍需开发者自行验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/tencent/AuK-Flash">tencent/AuK-Flash · Hugging Face</a></li>
<li><a href="https://github.com/Tencent-Hunyuan/AuK">GitHub - Tencent-Hunyuan/AuK: AuK: An Open-Source ...</a></li>
<li><a href="https://ai-tldr.dev/models/auk/">AuK — Tencent&#x27;s Open Speech Generation Model | AI/TLDR</a></li>

</ul>
</details>

**标签**: `#open-source`, `#audio-editing`, `#text-to-speech`, `#speech-editing`, `#Tencent-Hunyuan`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [跟随瓶颈：在 AMD MI355X 上优化 MiniMax M3](https://vllm.ai/blog/2026-09-10-minimax-m3-mi355x) ⭐️ 9.0/10

rss · vLLM Blog · 9月10日 00:00

**「背景」** MiniMax M3 在 AMD Instinct MI355X 上的 day-0 vLLM 实现（MSA 稀疏注意力、多模态、MXFP8 权重、EAGLE3）已经能跑通，但真正的问题是：当瓶颈不断移动时，下一步该优化什么？作者以 SemiAnalysis InferenceX 基准和具体 PR 为主线，记录从局部形状、重复路径、稀疏元数据、分布式状态到工作负载队列的逐层追问。

**「方案」** 作者的核心方法是“跟随瓶颈”：先估计主导成本，再测量、批处理重复工作、预计算不变量，叶子 kernel 变平后把问题层级上移。本地形状上，TP 分片和头复制决定实际 M/N/K，按 prefill/decode 选择 tile 并重排 grouped-MoE，使 TP4 端到端提升 1.08×–1.46×。重复工作上，把共享专家并入路由专家表、复用 grouped GEMM，在并发 1 提升 30.2%、并发 128 提升 5.6%；跨层索引复用和 page-table 视图避免 KV 拷贝，在 TP4 并发 256 下使 MXFP4/MXFP8 输出吞吐提升 6.93%/5.56%。累积结果包括：MXFP8 标准服务并发 32 从 109.1 升至 342.4 输出 tok/s/GPU（3.14×），并发 128 从 297.8 升至 623.7（2.09×）；MXFP4 TP2 达 943.5，EAGLE3 达 682.4，P/D 解耦后在并发 512 达 6370.5 总 tok/s/GPU、1.32 秒中位 TTFT。作者也强调边界：公开曲线是累计检查点，固定 8K/1K 策略排除了跨层索引复用，并撤回无法证明执行的 INT4 QuickReduce 归因；正确性同样是性能合同，FP8 KV 修复让 GSM8K 从 0.0099 到 0.9575。P/D 最初虽达 2084.6 总 tok/s/GPU，但 223.20 秒中位 TTFT 说明队列才是真瓶颈；AgentX 首点前缀缓存实际命中率 92.1%，提示下一瓶颈可能是缓存对齐与调度。

**「启示」** 作者的结论是：MiniMax M3 变快靠的是不断改变瓶颈问题的层级——从 tile、重复路径、稀疏元数据、分布式状态到工作负载队列。优化因此应从追数字转向追瓶颈。

**标签**: `#LLM inference optimization`, `#AMD Instinct MI355X`, `#vLLM`, `#sparse attention/MoE`, `#performance profiling`

---

<a id="item-tech-blog-2"></a>
### [vLLM 分层 KV 缓存卸载：以主机内存为中心的设计](https://vllm.ai/blog/2026-09-10-tiered-kv-offloading) ⭐️ 8.0/10

rss · vLLM Blog · 9月10日 00:00

**「背景」** 长上下文模型与多轮对话会产生庞大的 KV cache。当 GPU 显存被占满时，先前算好的 KV 被驱逐，后续请求只能从头重算，既浪费算力又压低集群的有效服务容量；vLLM 自 v0.22 起提供的分层 KV 缓存卸载，就是把被驱逐的数据保留在主机内存、存储和远端节点上。

**「方案」** 其核心原则是让所有 KV 数据都流经主机内存：卸载时先用 PCIe 异步 DMA 从加速器拷到主机并立即释放显存，再由 tiering manager 并行级联到文件系统、对象存储等二级层；重载先查主机缓存，未命中则按配置顺序查询各二级层，命中的层异步把数据提升回主机，期间调度器收到 RETRY 并在下一轮重查。主机层是真正的 LRU/ARC 缓存而非暂存区。主机侧采用规范布局——每页存一层的一个 block，跨 TP rank 的 KV heads 聚成连续区域，与 GPU 布局、注意力后端和并行配置无关，因此 TP=2 与 TP=4 的节点可直接共享同一份 chunk。二级层是单进程组件，用 POSIX I/O、S3 SDK、RDMA verbs 传输，接口只有四个方法并直接读写主机区的 memoryview，支持 out-of-tree 扩展；P2P 层用 ZMQ 协调、RDMA 做主机到主机传输，由 llm-d 之类编排层决定向谁拉取。作者称整合 I/O 把大量小传输并为更少更大的 RDMA 操作，chunked prefill 让计算与数据传输重叠以降低首 token 延迟，混合模型（full attention、sliding window、MLA、Mamba）经统一字节缓冲归一化后透明处理，Prometheus 指标与 KV events 则支撑外部调度做缓存感知路由。在 Qwen3.6-35B-A3B、2×H100（TP=2）、本地 NVMe 文件系统层、12K 首轮加 4K/轮共 8 轮、并发 64 的测试中：约 64 个会话内 HBM 足够，64–128 时无卸载的吞吐骤降而 CPU 卸载仍能维持，超过 128 后 CPU 缓存也满、存储层仍保持高命中并把吞吐提高一倍以上；存储延迟更高故达不到峰值吞吐，但相比全量重算仍是明确胜出。

**「启示」** 作者的结论是，让 KV 数据统一经主机内存中转并采用配置无关的规范布局，能把多级缓存以极小的接口成本扩展到存储与远端节点，从而在长上下文多轮负载中以可接受的延迟换取明显更高的有效服务容量。

**标签**: `#KV cache offloading`, `#vLLM`, `#LLM inference serving`, `#memory tiering`, `#prefill-decode disaggregation`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Kalshi launches ‘perps’ for gold and silver following CFTC approval, expanding futures offerings](https://www.cnbc.com/2026/09/10/kalshi-launches-perps-for-gold-and-silver-following-cftc-approval-expanding-futures-offerings.html) ⭐️ 7.0/10

Kalshi won CFTC approval and launched perpetual futures on gold and silver, expanding its regulated derivatives offerings beyond crypto and prediction markets.

rss · CNBC Finance · 9月10日 14:00

**标签**: `#Kalshi`, `#perpetual futures`, `#CFTC`, `#gold and silver`, `#derivatives regulation`

---

<a id="item-finance-news-2"></a>
### [中国 AI 芯片厂商因 HBM 短缺上调价格](https://www.reuters.com/world/asia-pacific/chinas-ai-chipmakers-raise-prices-high-bandwidth-memory-shortage-bites-2026-09-10/) ⭐️ 7.0/10

受高带宽存储器（HBM，即用于 AI 芯片的高速内存）供应紧张影响，华为、寒武纪等中国 AI 芯片厂商已上调产品价格。据报道，华为升腾 950DT 报价较两个月前上涨约 20%—50%，部分老款芯片上涨约 30%；寒武纪新一代思元 690 价格预计上涨约 20%—30%。

telegram · zaihuapd · 9月10日 09:29

**「背景」** 美国出口管制限制中国获取英伟达最先进处理器后，本土 AI 芯片厂商曾受益于留下的市场空缺，但 HBM（高带宽存储器，AI 芯片的关键部件）主要由 SK 海力士、三星和美光供应，中国获取渠道又受出口限制影响，供应紧张因此成为国产 AI 芯片扩张的瓶颈。

**「影响」** 这一涨价直接推高了中国数据中心和 AI 企业的算力建设成本，并可能拖慢北京推动用国产芯片替代英伟达产品的进程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.msn.com/en-us/technology/hardware-and-devices/china-ai-chipmakers-raise-prices-amid-hbm-shortage/vi-AA2bXQwL">China AI chipmakers raise prices amid HBM shortage</a></li>
<li><a href="https://money.usnews.com/investing/news/articles/2026-09-10/exclusive-chinas-ai-chipmakers-raise-prices-as-high-bandwidth-memory-shortage-bites">Exclusive- China &#x27;s AI Chipmakers Raise Prices as High-Bandwidth...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/exclusive-chinas-ai-chipmakers-raise-050223278.html?fr=sycsrp_catchall">Exclusive-China&#x27;s AI chipmakers raise prices as high ...</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/chinas-ai-chipmakers-raise-prices-high-bandwidth-memory-shortage-bites-2026-09-10/">EXCLUSIVE: China&#x27;s AI chipmakers raise prices as high ...</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#HBM`, `#China semiconductors`, `#export controls`, `#pricing`

---