---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> 从 42 条内容中筛选出 14 条重要资讯。

---

**科技新闻**
1. [Qwen3.8-2.4T 发布：2.4T 参数 MoE 开源模型](#item-tech-news-1) ⭐️ 9.0/10
2. [DeepSeek V4 Pro 0813 发布与社区初测](#item-tech-news-2) ⭐️ 8.0/10
3. [追踪 16 年之久的 SQLite WAL-reset 漏洞](#item-tech-news-3) ⭐️ 8.0/10
4. [Zed 推出 Delta：AI 智能体对话成为编辑器文档](#item-tech-news-4) ⭐️ 8.0/10
5. [xAI 发布 Grok 4.6，社区质疑基准可信度](#item-tech-news-5) ⭐️ 8.0/10
6. [uBlock Origin 停止过滤 Facebook 广告](#item-tech-news-6) ⭐️ 7.0/10
7. [Adam 的逐坐标缩放破坏隐式低秩偏置](#item-tech-news-7) ⭐️ 7.0/10
8. [白宫拟将开源模型纳入发布前安全测试](#item-tech-news-8) ⭐️ 7.0/10
9. [苹果拟为 Siri AI 购买新闻内容，按使用量付费](#item-tech-news-9) ⭐️ 7.0/10
10. [特朗普签署备忘录允许私企开展海外监控与网络攻击](#item-tech-news-10) ⭐️ 7.0/10

**财经新闻**
1. [中国车市：电动车占比升至 65.1%，吉利星愿居畅销榜首位](#item-finance-news-1) ⭐️ 8.0/10
2. [中国 YMTC NAND 闪存出货量跻身全球第三](#item-finance-news-2) ⭐️ 7.0/10
3. [CME 集团拟推出首批 AI 算力期货合约](#item-finance-news-3) ⭐️ 7.0/10
4. [中国零工劳动者增至超 5300 万，就业市场供过于求](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Qwen3.8-2.4T 发布：2.4T 参数 MoE 开源模型](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

通义千问发布了 Qwen3.8-2.4T-A95B，这是一款 2.4 万亿参数的混合专家（MoE）开源权重语言模型，推理时激活 95B 参数。BF16 无损版约 4.9TB，官方同时提供 FP8 版本；社区称 1-bit 量化版可压至约 397GB，并称模型卡显示其性能介于 Claude Opus 4.8 与 Fable 5 之间，是 Kimi k3 的竞品。许可协议与 k3 相似，内部使用或年收入低于 5000 万美元可免费，超过该门槛后对外提供服务受限。开源版缺少视觉输入、默认 1M 上下文和内置工具，这些是 Qwen3.8-Max 的增强功能。

hackernews · Philpax · 8月12日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=49273478)

**「背景」** Qwen3.8-2.4T-A95B 是阿里巴巴 Qwen 团队发布的开源权重稀疏混合专家（MoE）模型，也是 Qwen3.8-Max 的开源版本：总参数达 2.4 万亿，但每次推理只激活约 950 亿参数，因此能以相对较低的算力运行。该模型采用细粒度 MoE 架构，并混合了全注意力与线性注意力机制，支持较长上下文，定位为接近前沿闭源模型的开放权重模型。

**「影响」** 对 AI 工程师和自托管用户而言，模型虽巨大，但 1-bit 量化后可在约 397GB 显存或内存的消费级工作站运行，同时达到接近顶级闭源模型的性能；不过 BF16 和 FP8 原始版本在发布初期比 Kimi k3 更难部署，q4 量化需要大量校准数据。

**「社区讨论」** 评论者普遍认可其性能定位，认为 1-bit 量化让 Opus 4.5 级能力进入可购买硬件，但指出开源版本没有视觉支持和默认 1M 上下文是遗憾；也有用户对真正跑满性能所需硬件何时降到 1 万美元以下表示怀疑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/serve-qwen3-8-2-4t-a95b-a-2-4t-parameter-model-with-configurable-reasoning-on-nvidia-gb300-nvl72/">Serve Qwen3.8-2.4T-A95B, a 2.4T-Parameter Model, with Configurable ...</a></li>
<li><a href="https://benchable.ai/models/qwen/qwen3.8-2.4t-a95b-20260812">Qwen: Qwen3.8 2.4T A95B - AI Model Details &amp; Benchmarks</a></li>

</ul>
</details>

**标签**: `#large language models`, `#AI`, `#Qwen`, `#open source`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [DeepSeek V4 Pro 0813 发布与社区初测](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek V4 Pro 0813 是 DeepSeek 新发布的模型，现可通过 OpenRouter 直接调用，官方 API 文档已更新，Artificial Analysis 也建立了对应基准页。该发布延续 DeepSeek 系列的低成本策略，主要面向需要 API 接入的开发者。Hacker News 上的早期试用手记显示，实际效果依任务场景而异：有人在生成 docker-compose 的部署任务中遇到问题，也有人在仿真和分布式物理引擎任务中获得明显改进且没有引入新问题。此次发布之所以重要，是因为它为 AI/ML 社区提供了一个新的、可能更具性价比的模型选项，但其真实能力和稳定性仍需更多正式基准与大规模验证。

hackernews · explosion-s · 8月12日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=49274600)

**「背景」** DeepSeek V4 Pro 0813 是 DeepSeek 旗舰模型 V4 Pro 的生产版本，于 2026 年 8 月 12 日结束约四个月的预览期后正式发布，并可通过 OpenRouter 等平台调用。根据官方 API 文档，DeepSeek-V4-Pro 拥有 1.6T 总参数、49B 激活参数，并支持 1M 上下文长度；V4-Flash 则为 284B 总参数、13B 激活参数。该模型被定位为性能接近顶级闭源模型的开源可调用模型，社区早期测试侧重于与 GPT-5.6-terra-high 等竞品的实际任务对比。此次发布延续了 DeepSeek 以低成本提供长上下文与较强推理能力的路线。

**「影响」** DeepSeek V4 Pro 0813 通过 OpenRouter 提供 API，其定价远低于前沿竞品：输入约为 GPT-5.6 Sol 的 1/11、Claude Opus 5 的 1/36，输出约为后两者的 1/34 和 1/89，并支持 1M 上下文窗口，这让它在高 token 消耗的开发任务中成为高性价比选择。社区实测显示，一位开发者仅花费约 12.50 美元（2B token、50% 缓存命中）就完成了对交通模拟/分布式物理引擎的明显优化。

**「社区讨论」** 讨论中观点分歧明显：freakynit 在扫描现有仓库并生成 docker-compose 的实测中，认为该模型比 GPT-5.6-terra-high 问题更多，且与他对最新 Flash 版的既有观察一致；monster\_truck 则在流量模拟器/分布式物理引擎上跑了约 2B token（约 12.50 美元，50% 缓存命中），报告获得显著优化且没有引入新问题。alecsm 对上一代 Deepseek Flash 的低成本重型开发能力印象深刻，期待新版；book\_mike 更关心最低成本完成任务，目前使用 Kimi-K3、GLM-5.2 和 MiniMax，并认为 Sonnet 消耗 token 太快、Opus 5 虽更强但对多数任务而言并不必要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unite.ai/deepseek-ships-v4-pro-as-its-flagship-model-leaves-preview/">DeepSeek Ships V4 Pro as Its Flagship Model Leaves ...</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260424/">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>
<li><a href="https://codersera.com/blog/deepseek-v4-pro-review-benchmarks-pricing-2026/">DeepSeek V4-Pro Review: Pricing, Benchmarks &amp; Verdict</a></li>
<li><a href="https://benchlm.ai/models/deepseek-v4-pro">DeepSeek V4 Pro Benchmarks &amp; Pricing (August 2026)</a></li>

</ul>
</details>

**标签**: `#deepseek`, `#llm`, `#ai-models`, `#model-release`, `#openrouter`

---

<a id="item-tech-news-3"></a>
### [追踪 16 年之久的 SQLite WAL-reset 漏洞](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale 发布了对 SQLite WAL-reset 竞态条件缺陷的详细追踪报告，该缺陷已潜伏约 16 年。调查显示，此问题只在多个并发连接或进程同时参与 WAL 写入与检查点时出现，因此与 SQLite 常见的“单写者”用法不同。Tailscale 资助了一个开源 SQLite VFS shim 工具，用来快速隔离和复现该竞态，并计划用它排查类似缺陷。公司还与 SQLite 团队签订了商业支持合同，最终修复了问题，并为社区提供了可复用的调试手段。

hackernews · ropbear · 8月12日 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49272832)

**「背景」** SQLite 默认使用预写日志（WAL）模式来提升并发读写性能，其中 WAL 重置是日志文件轮转时的一个关键内部步骤。Tailscale 在排查数据库损坏问题时发现，这一重置过程存在一个数据竞争条件，且该问题据估计已存在至少 16 年，直到最近才被定位并修复。此背景解释了为何这一看似底层的 bug 会对依赖 SQLite 的应用程序造成严重影响。

**「影响」** SQLite 用户和 VFS 实现者获得了一个新的开源调试工具，可在隔离 WAL 相关竞态条件时复用；Tailscale 的控制面不再受该缺陷影响，也为此类并发问题的排查提供了可参考的案例。

**「社区讨论」** 评论普遍认可 Tailscale 的做法，认为公司资助开源调试工具并签订商业支持合同是重视正确性的表现。有读者澄清，该 bug 只会在多连接并发场景下触发，并不违背 SQLite 作为单写者数据库的预期用法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL - Reset bug</a></li>

</ul>
</details>

**标签**: `#sqlite`, `#bug`, `#database`, `#debugging`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [Zed 推出 Delta：AI 智能体对话成为编辑器文档](https://zed.dev/blog/introducing-delta) ⭐️ 8.0/10

Zed 编辑器发布了名为 Delta 的新功能，将协作式 AI 智能体对话作为文档嵌入编辑器。Delta 结合了实时多人协作与 AI 智能体线程，允许用户在对话中内联评论，将“对话即文档”的理念引入开发流程。该功能可能影响代码评审和新人指导等协作场景，但社区对其实际价值仍有分歧。目前没有公布具体版本号、日期或性能数据。

hackernews · khy · 8月12日 18:19 · [社区讨论](https://news.ycombinator.com/item?id=49276574)

**「背景」** Zed 是一款开源、注重速度的 AI 代码编辑器，原生支持代理式编辑和 Git 操作，并宣称能与人类开发者及 AI 模型流畅协作。此次发布的 Delta 是 Zed 推出的一种多人协作环境，旨在将代码与对话整合到统一工作区中，让人类开发者与 AI 代理能在实时协作的会话里共同工作。

**「社区讨论」** 社区反馈分歧明显：有用户认为 Zed 本身出色但多人编辑需求有限，质疑这项技术缺乏实际用途；也有人反感 AI 生成的代码摘要，担心其冗长或遗漏边界情况；还有人看到它在指导初级工程师和理解 PR 生成过程上的价值。另有评论抱怨 Zed 博客页面文字对比度低，影响阅读体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-13-zed-introduces-delta-a-new-multiplayer-environment-for-collaborative-coding-with-ai-agents-and-real">Zed Delta: Multiplayer Coding Environment for AI Agents</a></li>
<li><a href="https://zed.dev/">Zed — Your last next editor</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#collaborative editing`, `#code editor`, `#Zed`, `#software development tools`

---

<a id="item-tech-news-5"></a>
### [xAI 发布 Grok 4.6，社区质疑基准可信度](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI 发布了 Grok 4.6，这是其前沿模型家族的增量更新，并提供了 Artificial Analysis 的基准评测文章。社区讨论聚焦于模型性能、API 默认系统提示词行为以及基准测试的可信度。部分用户称 Grok 4.6 在多数基准测试上超过 GPT-5.6-Sol 和 Claude 4.8/5，但也有观点质疑这些成绩可能来自“调分”或蒸馏。此外，API 默认添加的系统提示词可能覆盖用户指令，导致模型拒绝讨论系统提示词相关话题。

hackernews · iLuddite · 8月12日 15:32 · [社区讨论](https://news.ycombinator.com/item?id=49274027)

**「背景」** Grok 是 SpaceXAI（xAI）开发的一系列大语言模型，最初于 2023 年 11 月由埃隆·马斯克推出。Grok 4.6 是继 Grok 4.5 之后的版本，官方称其重点增强长时间运行的代理任务以及更具雄心的交互式和视觉工作能力。此次发布被视为在基准测试中与 GPT-5.6 等前沿模型竞争的重要更新。

**「影响」** 使用 Grok 4.6 API 的开发者可能遇到默认系统提示词覆盖自定义指令的问题，从而使涉及系统提示词的对话被拒绝。若 Grok 4.6 的基准成绩可信，它将成为其他前沿模型的有力竞争者，但其品牌声誉仍可能限制部分用户采用。

**「社区讨论」** 讨论中既有正面体验，如 Grok 4.5/4.6 更简洁直接，也有人怀疑各实验室在短时间内涌现出同级模型是基准测试操纵或技术快速传播所致。API 的默认系统提示词行为被实际用户指出，并可能影响开发者的集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_%28chatbot%29">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://x.ai/news/grok-4-6">Introducing Grok 4 . 6 | SpaceXAI</a></li>

</ul>
</details>

**标签**: `#AI`, `#Grok`, `#model release`, `#benchmarks`, `#xAI`

---

<a id="item-tech-news-6"></a>
### [uBlock Origin 停止过滤 Facebook 广告](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 7.0/10

uBlock Origin 已停止过滤 Facebook 广告，原因是该平台让广告难以通过常规过滤规则拦截。这一决定意味着使用 uBlock Origin 的 Facebook 用户将看到更多广告，除非他们使用其他工具或方法。此举也反映了广告拦截器与社交平台之间持续的技术对抗。

hackernews · Markoff · 8月12日 11:28 · [社区讨论](https://news.ycombinator.com/item?id=49270726)

**「背景」** uBlock Origin 是一个流行的开源广告拦截浏览器扩展，依赖社区维护的过滤规则来隐藏网页广告。Facebook 通过不断改变广告的 HTML 结构、混入无意义标记等方式，使基于选择器的过滤规则难以稳定生效。据相关报道，这个小型志愿者团队已经决定停止针对 Facebook 专门更新规则，因为多年来平台持续调整代码，拦截变成了一场令人精疲力竭的“打地鼠”游戏；用户近期在 Facebook 上看到广告并非自身配置问题，而是项目主动退出了这场针对特定平台的对抗。

**「影响」** 依赖 uBlock Origin 过滤 Facebook 广告的用户将不再获得该保护，可能会在 Facebook 上看到更多广告。

**「社区讨论」** 社区评论普遍对 Facebook 的广告混淆表示不满，认为这是故意的技术对抗。有用户表示宁愿离开 Facebook 也不看广告，并担忧这种 div 嵌套会影响无障碍访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://piunikaweb.com/2026/08/10/ublock-origin-facebook-ads-not-blocking/">Seeing ads on Facebook even with uBlock Origin? Here&#x27;s why</a></li>
<li><a href="https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html">uBlock Origin Is Giving Up the Fight to Keep Ads Off Facebook</a></li>
<li><a href="https://www.neowin.net/news/facebook-ads-are-so-hard-to-block-that-ublock-origin-stopped-filtering-them/">Facebook ads are so hard to block that uBlock Origin stopped ...</a></li>

</ul>
</details>

**标签**: `#uBlock Origin`, `#Facebook`, `#ad blocking`, `#privacy`, `#open source`

---

<a id="item-tech-news-7"></a>
### [Adam 的逐坐标缩放破坏隐式低秩偏置](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 7.0/10

该研究帖子指出，在因子化模型 W=UV^T 中，损失对旋转保持不变，但 Adam 的逐坐标二阶矩依赖基方向，因此 Adam 会失去梯度下降（GD）的隐式低秩偏置，而 Muon 和 Shampoo 等旋转不变优化器则保留该偏置。作者在欠定矩阵感知任务上比较了九种更新规则，在训练损失匹配的条件下观察到了两个清晰聚类：GD、共享标量 Adam、Muon 和 Shampoo 保持低秩偏置，而 Adam、RMSProp、Lion、signum 和 Adafactor 则丢失该偏置。一个由逐坐标分母连续过渡到共享标量分母的单参数族单调改善恢复误差，表明破坏来自各向异性而非自适应本身。Muon 在真实低秩目标上表现精确，但随谱尾增加而快速退化，并在约 4% 尾能量处出现与 GD 的交叉。作者提前说明，对高光谱数据 43%–44% 的留出误差降低来自仅使用训练集的学习率规则，该规则恰好为 Adam 选择了其网格上最差的率；若让各方法自行选择最优率，差异会明显缩小。

reddit · r/MachineLearning · /u/EtherealGlyph · 8月12日 16:39

**「背景」** 隐式低秩偏置是指某些优化算法在不显式加入正则化时，倾向于找到低秩或结构更简单的解，这在矩阵感知和深度线性网络中被广泛研究。Adam 的逐坐标归一化使其对参数矩阵的旋转不敏感，而旋转不变性是许多因式分解模型自然具备的对称性，因而这种归一化可能破坏原本由梯度下降所依赖的几何结构。

**「影响」** 对使用 Adam 类优化器的研究者而言，该结果说明逐坐标归一化可能破坏隐式低秩正则化；作者报告将自身优化器中的逐坐标裁剪改为全局范数裁剪后，恢复误差由 0.347 降至 0.220，表明这一机制可被直接用于改进优化器设计。

**标签**: `#optimization`, `#Adam`, `#low-rank bias`, `#matrix sensing`, `#machine learning`

---

<a id="item-tech-news-8"></a>
### [白宫拟将开源模型纳入发布前安全测试](https://www.wired.com/story/the-white-house-is-going-to-expand-its-ai-policy/) ⭐️ 7.0/10

白宫据报计划扩大其人工智能政策框架，将开源模型纳入监管范围。目前该框架仅覆盖 Anthropic、OpenAI 等闭源模型，未来数月内，开源模型一旦达到“前沿”能力，也须接受发布前安全测试。由于特朗普政府认为正式监管只会帮助中国追赶美国，该框架仍属自愿性质。部分官员担忧，可能要求的 30 天测试期限会抑制美国企业发展。相关报道来自 WIRED，但具体政策细节和生效时间尚未确认。

telegram · zaihuapd · 8月13日 00:43

**「背景信息」** 2026 年 8 月 4 日，美国白宫敲定了一项自愿性 AI 安全测试框架，要求美国实验室开发的、能力最强的&quot;前沿&quot;模型在公开发布前先由联邦政府进行安全测试。然而，该框架目前仅覆盖 Anthropic、OpenAI 等闭源模型开发商，明确排除了开放权重模型，且政策细则不会公开，测试标准只与少数科技公司共享。白宫据报计划扩大该框架，未来数月内将开源模型纳入监管，一旦其达到&quot;前沿&quot;能力门槛，也须接受发布前安全测试。

**「影响」** 美国开源模型开发者一旦其模型达到“前沿”能力，预计将被纳入白宫扩展后的 AI 政策框架，须接受发布前安全测试；不过该框架目前仍属自愿，且部分官员担心约 30 天的测试要求可能抑制美国企业发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wired.com/story/the-white-house-is-going-to-expand-its-ai-policy/">The White House Is Going to Expand Its AI Policy | WIRED</a></li>
<li><a href="https://www.theguardian.com/technology/2026/aug/07/white-house-ai">The White House’s plan to vet potentially dangerous AI is cloaked in secrecy | AI (artificial intelligence) | The Guardian</a></li>
<li><a href="https://www.yahoo.com/news/politics/articles/white-house-ai-framework-excludes-073920495.html">White House AI Framework Excludes Open-Weight Models From Federal Security Review, Creating Structural Competitive Asymmetry</a></li>
<li><a href="https://www.wired.com/story/the-white-house-is-going-to-expand-its-ai-policy/">The White House Is Going to Expand Its AI Policy | WIRED</a></li>
<li><a href="https://witho2.com/news/white-house-voluntary-ai-framework-frontier-models">White House Voluntary AI Rules: What the New Framework Means</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#open source`, `#regulation`, `#safety testing`, `#United States`

---

<a id="item-tech-news-9"></a>
### [苹果拟为 Siri AI 购买新闻内容，按使用量付费](https://9to5mac.com/2026/08/12/report-apple-seeks-publisher-deals-to-give-siri-ai-better-access-to-current-events/) ⭐️ 7.0/10

消息人士称，苹果正与出版商洽谈多年期内容协议，为计划于 2026 年晚些时候推出的 Siri AI 提供当前新闻和信息。苹果讨论了按内容使用量向合作方付款的方案，预算可能达到九位数（数亿美元），这与大型 AI 公司常见的预付固定授权费模式不同。苹果尚未宣布任何相关合作，公司也拒绝置评；该消息来自 9To5Mac、MacRumors 和《华尔街日报》的报道。

telegram · zaihuapd · 8月13日 04:40

**「背景」** 大型 AI 公司在训练模型或提供实时信息时，通常与新闻出版商签订固定费用的内容授权协议。苹果计划中的 Siri AI 需要访问最新新闻，可能为了避免与传统授权模式捆绑，探索按使用量计费的新方式。Siri AI 预计在 2026 年晚些时候亮相，但官方尚未公布具体功能或合作细节。

**「影响」** 如果该协议达成，按使用量计费可能成为 AI 新闻授权的替代模式，影响出版商与苹果及其他 AI 公司的谈判格局；Siri 用户也可能获得基于当前事件的回答。不过目前消息尚未得到官方确认，具体条款和预算仍存不确定性。

**标签**: `#Apple`, `#Siri`, `#AI`, `#news licensing`, `#artificial intelligence`

---

<a id="item-tech-news-10"></a>
### [特朗普签署备忘录允许私企开展海外监控与网络攻击](https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal) ⭐️ 7.0/10

美国总统特朗普签署备忘录，允许私营企业在联邦政府直接控制和监督下开展海外监控与网络攻击，目标是打击针对美国人的外国网络化跨国犯罪组织。国土安全部将负责运行该项目，并与司法部协调监督。参与企业须维持至少 100 万美元的保证金或托管款，若不遵守合同约定，该款项将被没收。此举使私营部门系统性参与美国背书的进攻性网络行动，对网络安全行业、隐私保护和国际安全产生广泛影响。

telegram · zaihuapd · 8月13日 05:10

**「背景」** 长期以来，针对境外跨国网络犯罪组织的监控和攻击性网络行动主要由美国联邦政府机构执行。2026 年 8 月，特朗普签署总统备忘录，启动一项新计划，允许经审查的美国私营企业在联邦政府直接指导与监督下，对境外的跨国网络犯罪组织实施网络监控和攻击性网络行动。国土安全部负责项目运行，并与司法部协调监督，参与企业须维持至少 100 万美元保证金或托管款，若不遵守合同将被没收。

**「影响」** 该政策将使符合条件的美国私营安全企业获得政府授权开展海外网络行动，可能重塑网络安全服务市场，并加剧围绕跨境监控和网络攻击的法律与隐私争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal">Trump Signs Memo Allowing Private Firms to Conduct Cyber Attacks ...</a></li>
<li><a href="https://news.slashdot.org/story/26/08/13/0052208/trump-administration-enlists-private-companies-to-hack-foreign-cybercrime-groups">Trump Administration Enlists Private Companies To Hack... - Slashdot</a></li>
<li><a href="https://www.whitehouse.gov/presidential-actions/2026/08/expanding-capabilities-to-combat-transnational-cyber-enabled-crime/">Expanding Capabilities to Combat Transnational Cyber -Enabled Crime</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#policy`, `#surveillance`, `#technology-industry`, `#private-sector`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国车市：电动车占比升至 65.1%，吉利星愿居畅销榜首位](https://www.cnbc.com/2026/08/12/china-car-sales-data-byd-tesla-geely-vw.html) ⭐️ 8.0/10

中国汽车销售最新数据显示电动车正主导市场：7 月新能源车占新乘用车销量的 65.1%，高于一年前的 54%；行业数据显示，上半年吉利星愿以近 19.75 万辆成为最畅销车型，而比亚迪乘用车销量下滑逾 10%。

rss · CNBC Finance · 8月13日 01:31

**「背景」** 新能源车包括纯电动和插电混动等车型；尽管市场份额扩大，今年前 7 个月新能源车销量仍同比下降 12.5%，整体乘用车销量下降 20.3%。

**标签**: `#China auto market`, `#electric vehicles`, `#BYD`, `#Tesla`, `#Geely`

---

<a id="item-finance-news-2"></a>
### [中国 YMTC NAND 闪存出货量跻身全球第三](https://www.cnbc.com/2026/08/13/chinese-firm-tops-micron-kioxia-shipments-nand-memory-chips.html) ⭐️ 7.0/10

Counterpoint 数据显示，中国长江存储（YMTC）今年第二季度 NAND 闪存芯片出货量跃居全球第三，份额约 14%，仅次于三星和 SK 海力士，超过美光和铠侠。

rss · CNBC Finance · 8月13日 02:59

**「背景」** NAND 闪存是断电后仍可保存数据的存储芯片；YMTC 正在准备在中国大陆上市，此前 DRAM 芯片厂商长鑫存储（CXMT）上月已上市。

**「影响」** 尽管出货量领先，YMTC 在 NAND 收入上仍落后于美光和铠侠，且更依赖消费应用；分析师认为 15%份额是存储厂商自我融资扩产的最低门槛。

**标签**: `#NAND memory`, `#YMTC`, `#semiconductor industry`, `#market share`, `#China tech`

---

<a id="item-finance-news-3"></a>
### [CME 集团拟推出首批 AI 算力期货合约](https://www.cnbc.com/2026/08/11/ai-computing-power-becomes-a-tradable-asset-class-as-cme-starts-futures.html) ⭐️ 7.0/10

CME 集团计划于 10 月 5 日推出首批与 AI 芯片租赁成本挂钩的期货合约，尚待监管批准，让投资者和企业可像交易石油或电力一样交易和对冲 AI 算力；每份合约代表一台 Nvidia H100 一个月的租金。

rss · CNBC Finance · 8月12日 14:14

**「背景」** 这些合约由 CME 与 Silicon Data 合作推出，基于 Silicon Data 追踪 GPU 小时租赁价格的指数，覆盖 Nvidia H100 和更新的 Blackwell B200。

**「影响」** 若获得批准，AI 开发者和数据中心运营商可用这些合约对冲成本或收入，投资者也可在不直接持有芯片或数据中心的情况下获得 AI 算力价格敞口。

**标签**: `#AI`, `#futures`, `#CME Group`, `#GPU pricing`, `#commodities`

---

<a id="item-finance-news-4"></a>
### [中国零工劳动者增至超 5300 万，就业市场供过于求](https://www.ft.com/content/a3803e70-cb4d-444f-a31e-05be2f2c44f6?accessToken=zwAAAZ_5xcXzkdOjgD5wy01ET9OjHgW-LyxE9g.MEUCIQCWTIny3JTJV8e-PGyK0XL2tg5g_7Ay-rpKkwGZCpp1-AIgbMgJQPlqWgqAsX4s1k4gYaC4b8k0JveZOs35OJQvbZ4&amp;amp;sharetype=gift&amp;amp;token=7e8483bb-395d-429e-afca-2f4ab5ad150b) ⭐️ 7.0/10

据英国《金融时报》报道，中国经济放缓加剧就业挤压：截至 2025 年，外卖和网约车司机等零工劳动者超过 5300 万人，两年增加 1000 万人，但岗位供过于求正压低收入、拉长工时。

telegram · zaihuapd · 8月13日 06:40

**「背景」** 房地产低迷、消费疲弱、制造业收缩及自动化使零工经济成为过剩劳动力出口；深圳今年 6 月已宣布网约车市场饱和。

**「影响」** 受影响的零工劳动者包括外卖和网约车司机，上海浦东、北京大兴和成都天府机场出租车司机排队等客最长分别达 7 小时、8 小时和 10 小时。

**标签**: `#China`, `#gig economy`, `#employment`, `#labor market`, `#economic slowdown`

---