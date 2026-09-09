---
layout: default
title: "Horizon Summary: 2026-09-09 (ZH)"
date: 2026-09-09
lang: zh
---

> 从 42 条内容中筛选出 13 条重要资讯。

---

**科技新闻**
1. [苹果发布折叠屏手机 iPhone Duo](#item-tech-news-1) ⭐️ 9.0/10
2. [OpenAI 称 AI 解决 Navier–Stokes 千禧年难题，但陷抢先争议](#item-tech-news-2) ⭐️ 9.0/10
3. [vLLM v0.29.0 发布：Model Runner V2 默认启用并扩展新模型支持](#item-tech-news-3) ⭐️ 8.0/10
4. [Shopify 收购 Tailwind CSS 团队与品牌](#item-tech-news-4) ⭐️ 8.0/10
5. [Google Ads 恶意广告规避审核的技术剖析](#item-tech-news-5) ⭐️ 8.0/10
6. [自动驾驶车降低死亡率的证据日益增多](#item-tech-news-6) ⭐️ 7.0/10
7. [GPT-6 Astra、循环 Transformer 与隐藏推理引发讨论](#item-tech-news-7) ⭐️ 7.0/10
8. [Anthropic 探讨 AI 重塑经济与工作的未来](#item-tech-news-8) ⭐️ 7.0/10
9. [陶哲轩：AI 竞相解题或让研究者不再公开想法](#item-tech-news-9) ⭐️ 7.0/10
10. [美国防部被曝要求 OpenAI 开发低拒绝率军用模型](#item-tech-news-10) ⭐️ 7.0/10
11. [OpenAI 将 AI 用于芯片设计，称成本低于开源模型](#item-tech-news-11) ⭐️ 7.0/10

**财经新闻**
1. [阿达尼企业机场子公司达成约 10 亿美元募资协议](#item-finance-news-1) ⭐️ 8.0/10
2. [中国电动车企转向人形机器人：小鹏完成 9 亿美元融资并计划今年量产](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [苹果发布折叠屏手机 iPhone Duo](https://www.apple.com/iphone-duo/) ⭐️ 9.0/10

苹果发布全新折叠屏手机 iPhone Duo，标志着苹果首次把可折叠设计引入 iPhone 产品线，也是公司硬件方向的一次重大变化。截至现有资料，苹果尚未公布完整规格、售价和发售日期，官方信息仍以产品页和发布会展示为主。该设备采用可折叠形态，使手机在收纳时更紧凑、展开后可提供更大的显示区域。凭借苹果的行业影响力，这一发布已成为消费电子和折叠屏市场的关注焦点。

hackernews · thecosmicfrog · 9月9日 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49630931)

**「背景」** iPhone Duo 是苹果在 2026 年 9 月活动中正式公布的可折叠 iPhone，展开后拥有一块连续 7.6 英寸屏幕，被视为近 20 年来 iPhone 外形上最大的改变。该产品采用两块屏幕与可折叠内屏，256GB 版本起售价 1999 美元，预购于 10 月 16 日开始，10 月 23 日正式开售。此前市场长期传闻苹果研发折叠屏手机，此次发布标志着苹果正式进入折叠屏手机市场。

**「影响」** 此次发布意味着苹果正式进入折叠屏手机赛道，给原有折叠屏市场格局带来新的竞争变量；不过由于定价、供货和实际体验细节尚未公布，对市场和用户的实际影响仍有待观察。

**「社区讨论」** 社区评价出现分歧：有用户根据早期上手视频认为该机折痕几乎不可见，并对 John Ternus 主导发布会带来的风格变化表示期待；另一部分用户则批评演示过程显得排练过度、缺乏自然交流，同时抱怨手机体积不断增大、希望有更小巧的选择。讨论中还出现了从纸张 ISO 216 比例标准延伸至屏幕宽高比的偏题内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnn.com/2026/09/09/business/live-news/apple-event-foldable-iphone-ternus">Apple event: CEO John Ternus reveals foldable iPhone Duo | CNN Business</a></li>
<li><a href="https://www.macrumors.com/2026/09/09/apple-announces-foldable-iphone-duo/">Apple Announces Foldable &#x27;iPhone Duo&#x27; - MacRumors</a></li>
<li><a href="https://www.ign.com/articles/apple-announces-foldable-iphone-duo">Apple&#x27;s Foldable iPhone Duo is Finally Real – Here&#x27;s Everything You Need to Know</a></li>

</ul>
</details>

**标签**: `#Apple`, `#iPhone Duo`, `#foldable phone`, `#consumer hardware`, `#product announcement`

---

<a id="item-tech-news-2"></a>
### [OpenAI 称 AI 解决 Navier–Stokes 千禧年难题，但陷抢先争议](https://simonwillison.net/2026/Sep/8/on-navier-stokes/) ⭐️ 9.0/10

OpenAI 发布文章称，在 9 月 1 日听到两个千禧年难题已被解决的传言后，它启动了用未发布内部模型驱动的智能体在悬赏问题上进行尝试；智能体在启动约 88 小时后的 9 月 5 日获得 Navier–Stokes 存在性与光滑性问题的解决，随后用 GPT-6 Astra 花费 17 小时完成 Lean 形式化验证。OpenAI 称，全部尝试共发送 490 万条消息、消耗约 3000 亿输出 token，其中 Navier–Stokes 部分约 270 万条消息、1300 亿输出 token；按 GPT-6 Astra 公开 API 价格估算，3000 亿 token 约合 1500 万美元。与此同时，NYU 教授 Tristan Buckmaster 与 Anthropic 数学家 Levent Alpöge 公开抗议，称两人近一年来使用 Claude 和 Codex（主要是 GPT-5.6 Sol）研究相关问题，并于 8 月 15 日取得突破；他们指控 OpenAI 在获知风声后抢先行动。Buckmaster 还说，OpenAI 团队曾表示不会邀请在 Anthropic 任职的 Levent 合著，理由是两家的竞争关系。OpenAI 否认在对方公开前查看过其工作，但承认无法完全排除“来自其产品使用的去标识化数据”帮助改进模型的可能性。博主 Simon Willison 认为，这起事件显示“存在未公开解”的传闻本身就可能促使 AI 实验室大规模投入抢先解题，并再次暴露了用户数据“用于改进模型”的含义并不透明。

rss · Simon Willison · 9月8日 23:55

**「背景」** Navier–Stokes 存在性与光滑性问题描述三维流体运动方程是否总存在不会产生奇性、始终保持光滑的全局解。它是克雷数学研究所 2000 年 5 月 24 日宣布的七个千禧年大奖难题之一，单题悬赏 100 万美元，至今没有公认证明。AI 模型如果真能产出可验证的数学证明，将同时冲击数学方法和 AI 能力两个领域，这也是此次争议影响较大的原因。

**标签**: `#AI research`, `#mathematical breakthrough`, `#OpenAI`, `#Navier-Stokes`, `#Millennium Prize`

---

<a id="item-tech-news-3"></a>
### [vLLM v0.29.0 发布：Model Runner V2 默认启用并扩展新模型支持](https://github.com/vllm-project/vllm/releases/tag/v0.29.0) ⭐️ 8.0/10

vLLM v0.29.0 正式发布，包含 277 位贡献者（其中 91 位新贡献者）提交的 594 个 commit。此次更新将 Model Runner V2 设为所有模型的默认执行路径，并为其补齐 CUDA graph 显存预留、batch-sharded sampling、prompt embeds、speculative decoding 隐藏状态提取等能力；MRV1 仍用于少量 ROCm 模型和不支持的特性。新模型支持包括 Hy4-preview、Qwen3.8-Flash-Next、GraniteSWA/GraniteMoeSWA、NemotronH\_Omni\_Reasoning\_V3 与 Kimi K3 NVFP4 检查点，并为 Kimi K3、DeepSeek V4 与 Mamba prefix caching 加入多项性能优化。默认行为也有变化：Tensor Parallel CUDA 组默认启用 FlashInfer all-reduce，分布式 KV cache 的 NONE\_HASH 前缀缓存改为确定性哈希，并新增 \`--max-num-queued-reqs\`/\`--max-num-queued-tokens\` 准入控制参数。破坏性变更包括移除十种已弃用模型架构、迁移 FlexOlmo/Olmo3/Hunyuan V1-VL 至 Transformers 后端、删除 PyAV 视频解码后端，以及弃用 \`python -m vllm.entrypoints.openai.api\_server\` 命令。

github · khluu · 9月9日 08:54

**「背景」** vLLM 是广泛使用的开源大语言模型推理与服务引擎，Model Runner 负责将模型配置、输入批次与 GPU 执行图调度整合。此前 V1 是默认模型执行路径，V2 从 pooling 模型开始逐步接管；本次发布后 V2 成为所有受支持模型的默认运行器，以提升内存效率、采样与解码等环节的性能，并降低长期维护成本。

**「影响」** 使用 vLLM 部署受支持模型的团队升级到 v0.29.0 后，默认执行路径会切换为 Model Runner V2，可受益于采样显存减少、KV cache 自动预留和新的并发控制参数；但需注意默认启用 FlashInfer all-reduce，且部分旧模型架构和 PyAV 视频解码后端已被移除，可能要求调整配置或升级部署方式。仍依赖 ROCm 原始模型路径或旧入口点的用户应保持使用 MRV1 兼容路径，或改用 \`vllm serve\` 命令。

**标签**: `#vLLM`, `#LLM inference`, `#Model Runner`, `#GPU serving`, `#open source`

---

<a id="item-tech-news-4"></a>
### [Shopify 收购 Tailwind CSS 团队与品牌](https://tailwindcss.com/blog/tailwind-is-joining-shopify) ⭐️ 8.0/10

Shopify 收购了 Tailwind CSS 背后的团队与品牌；Tailwind 是一款广泛使用的开源 CSS 框架。此次交易发生在该团队承认人工智能已对以 UI 模板和文档为主要收入来源的业务造成严重冲击之后。收购后，Tailwind 的维护模式、品牌归属与后续版本路线尚无细节公开。这一整合对众多 Web 开发者以及依赖 Tailwind 生态的电商项目将产生后续影响，也反映出在 AI 生成代码日益普及的环境下模板类产品的脆弱性。

hackernews · EdwinHoksberg · 9月9日 13:27 · [社区讨论](https://news.ycombinator.com/item?id=49626190)

**「背景」** Tailwind CSS 是一个开源的“工具类优先”CSS 框架，让开发者可以直接在 HTML 中组合原子类来构建界面，由加拿大公司 Tailwind Labs 开发。Shopify 是总部位于渥太华的电商平台。此次 Shopify 收购 Tailwind Labs，意在为 Tailwind CSS 提供“稳定、长期的归属”，并维持其 MIT 开源许可下的持续发展。

**「影响」** 对使用 Tailwind 的开发者与电商建站生态来说，这项收购最直接的影响是框架的商业与治理方向将转入 Shopify 手中，而社区最关心的项目持续维护承诺目前尚不明朗。

**「社区讨论」** 评论中有人讨论在新项目中是否仍有必要使用 Tailwind，认为现代原生 CSS 已可替代并能简化构建依赖；另有人将 Tailwind 归入“CSSSlop”生态，质疑其长期可移植性。还有不少用户对 Tailwind 团队表示感谢，并认为在 AI 时代出售模板业务是合理选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tradingview.com/news/seekingalpha:72d53b6e5094b:0-shopify-acquires-tailwind-labs/">Shopify acquires Tailwind Labs — TradingView News</a></li>
<li><a href="https://seekingalpha.com/news/4641301-shopify-acquires-tailwind-labs">Shopify acquires Tailwind Labs (SHOP:NASDAQ) | Seeking Alpha</a></li>
<li><a href="https://betakit.com/tailwind-finds-stable-long-term-home-with-shopify-acquisition/">Tailwind finds “stable, long-term home” with Shopify acquisition | BetaKit</a></li>

</ul>
</details>

**标签**: `#acquisition`, `#tailwind`, `#css`, `#open-source`, `#shopify`, `#web-development`

---

<a id="item-tech-news-5"></a>
### [Google Ads 恶意广告规避审核的技术剖析](https://xlii.space/eng/malicious-software-on-google-ads/) ⭐️ 8.0/10

作者 xlii 在一篇第一人称技术文章中详细介绍了如何让恶意软件广告绕过 Google Ads 的审核流程，并指出其自动化内容审核机制存在可利用的弱点。该文章由 Hacker News 社区传播后引发广泛关注，后续作者在评论区表示自己的账户曾被暂停，但在互联网曝光并引发讨论后已恢复。此事件暴露了 Google Ads 在广告安全审核方面可能被针对性绕过的现实风险，也可能影响平台信任度和用户安全。

hackernews · xlii · 9月9日 11:43 · [社区讨论](https://news.ycombinator.com/item?id=49624856)

**「背景」** 恶意广告（malvertising）是指通过在线广告系统投放恶意软件或欺诈页面的行为。Google Ads 等广告平台通常依赖自动化审核机制来过滤违规内容，攻击者会尝试绕过这些机制以投放恶意软件。本文作者“xlii”在 Hacker News 上分享了自己如何规避 Google Ads 审核的过程，随后表示其广告账户曾被暂停，但在社区关注和投诉后又被恢复。此事反映了广告平台在内容审核与用户申诉机制方面的长期争议。

**「影响」** 该文公开了可复现的绕过 Google Ads 审核的广告投放方法，可能使恶意广告投放者得以在正规广告系统中传播恶意软件，直接威胁点击广告的普通用户并损害广告生态的可信度。

**「社区讨论」** 社区评论普遍认为 Google 的自动化审核系统存在严重失灵，许多用户反映广告充斥着诈骗内容或被错误拒绝且难以获得人工申诉；原帖作者也承认，若不是在 Hacker News 上被放大关注，他的账户问题可能不会得到解决。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49624856">How I advertise malicious software on Google Ads | Hacker News</a></li>
<li><a href="https://news.ycombinator.com/item?id=49626346">I made an update, but I &#x27;ll post also here in comments. | Hacker News</a></li>
<li><a href="https://news.ycombinator.com/item?id=49627577">Another thing they apparently do is let business owners... | Hacker News</a></li>

</ul>
</details>

**标签**: `#google-ads`, `#security`, `#malvertising`, `#ad-review-bypass`, `#platform-integrity`

---

<a id="item-tech-news-6"></a>
### [自动驾驶车降低死亡率的证据日益增多](https://spectrum.ieee.org/are-self-driving-cars-safe) ⭐️ 7.0/10

IEEE Spectrum 的一篇报道汇集现有数据指出，越来越多证据表明自动驾驶汽车比人类驾驶员更安全、能够减少道路死亡；该进展被视为可信但属于增量而非突变。报道提到 Waymo 用自动驾驶事故率与“普通驾驶员”而非其替代的网约车驾驶员对比，这一比较基准受到质疑。此外，致死事故数据本身存在偏差，例如未系安全带、超速、酒驾以及行人/自行车死亡等占比较高。总体而言，数据虽支持自动驾驶救人的方向，但社会接受度、监管和替代方案仍制约落地。

hackernews · bookofjoe · 9月9日 17:14 · [社区讨论](https://news.ycombinator.com/item?id=49629886)

**「背景」** IEEE Spectrum 的文章指出，越来越多证据表明自动驾驶技术每年可防止约 58 万起死亡，但自动驾驶汽车的安全性仍是需要持续评估的问题。相关综合研究也显示，自动驾驶汽车在常规驾驶和减少追尾碰撞方面通常比人类驾驶员更安全，但也存在例外情况。此背景有助于理解围绕数据比较和统计口径的讨论。

**「社区讨论」** Hacker News 评论者没有一致否定自动驾驶的安全性，但批评其宣传性对比，例如与普通驾驶员而非网约车司机比较，并指出酒驾、超速、安全带和行人死亡等数据会显著影响基准。部分人主张把资源投入公共交通，也有人认为自动驾驶汽车要满足“零致死”或可追责的法律逻辑才能被接受。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spectrum.ieee.org/are-self-driving-cars-safe">Are Self Driving Cars Safe as Early Data Suggests? - IEEE Spectrum</a></li>
<li><a href="https://inspirega.bytes.news/78d7fc2-autonomous-vehicles-road-safety/">Self - Driving Cars Outperform Humans in Safety , with Some Exceptions</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#safety`, `#artificial intelligence`, `#transportation`, `#data analysis`

---

<a id="item-tech-news-7"></a>
### [GPT-6 Astra、循环 Transformer 与隐藏推理引发讨论](https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and) ⭐️ 7.0/10

一篇评论文章探讨了 GPT-6 Astra 与循环 Transformer（looped transformers）作为通往“隐藏推理”的路径，并引发社区对思维链计算权衡的讨论。文章称相关概念涉及将模型输出在推理时重新回馈给模型，而不是把完整推理痕迹展示出来；社区评论指出已有研究在关注哪些计算问题最少需要多少思维链步骤，以及循环 Transformer 能否改变这些结论。目前没有确认的 GPT-6 Astra 发布细节，相关讨论主要基于演示与传闻；用户对 Astra 效果变化和电脑使用演示也有不同反应。

hackernews · ModelForge · 9月9日 14:37 · [社区讨论](https://news.ycombinator.com/item?id=49627370)

**「背景」** GPT-6 Astra 被报道采用“循环深度”（looped transformers）技术，将输出在推理时重新输入模型，以提高效率，但同时会隐藏部分或全部“思维链”（chain of thought）。思维链让大语言模型先输出中间推理步骤再给出最终答案；William Merrill 与 Ashish Sabharwal 的论文（arXiv:2310.07923）探讨了这类推理步骤对 Transformer 表达能力的影响。这为理解社区关于隐藏推理的利弊以及计算效率与可解释性权衡的讨论提供了背景。

**「影响」** 面对尚处传闻阶段的 GPT-6 Astra，AI/ML 实践者与研究者应重新评估显式思维链（CoT）的必要性与可观测性：若其确如分析所称采用循环 transformer 的潜在推理，模型可在不输出可读推理轨迹的情况下以隐藏状态迭代完成多步计算，从而减少推理 token 与参数开销，并让部分任务在更少参数下达到更强推理表现，但这也意味着推理过程更难被外部验证。官方并未确认相关模型细节，且社区评论中对 Astra 实际体验变化的报告也提示影响尚不确定。

**「社区讨论」** 评论中，有研究者引用了 Will Merrill 等关于思维链计算复杂度的文献，认为循环或通用 Transformer 与隐藏推理的关系值得关注；另一些用户则报告 Astra 在某个时点后能力表现发生变化、对其实时操作演示感到惊讶。整体讨论体现了研究视角与使用体验之间的分歧，但缺少对 GPT-6 Astra 本身的共识性验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra - Wikipedia</a></li>
<li><a href="https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and">GPT-6 Astra, Looped Transformers, and Hidden Reasoning</a></li>
<li><a href="https://arxiv.org/abs/2310.07923">[2310.07923] The Expressive Power of Transformers with Chain of Thought</a></li>
<li><a href="https://tosea.ai/blog/looped-transformer-recurrent-depth-astra-guide">What Is a Looped Transformer ? Complete Guide to... | Tosea. ai</a></li>
<li><a href="https://www.alphaxiv.org/abs/2502.17416">Reasoning with Latent Thoughts : On the Power of Looped ... | alphaXiv</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#transformer-architecture`, `#chain-of-thought`, `#GPT`

---

<a id="item-tech-news-8"></a>
### [Anthropic 探讨 AI 重塑经济与工作的未来](https://www.anthropic.com/institute/econ-scenarios) ⭐️ 7.0/10

Anthropic 发布的经济情景文章，探讨人工智能可能如何改变工作方式、生产力与医疗护理等领域的未来。文章设想 AI 能提高护士等职业的产出，使人有更多时间与患者交流，同时指出有些任务仍只能由人类完成，并预测新技术会催生新的工作。社区评论普遍认为这些情景过于乐观，强调在成本驱动的现实系统中，效率提升更容易导致岗位减少而非工作质量提升。该分析还因未包含失业、不平等加剧、社会信任受损或经济危机等负面情景而受到批评。

hackernews · oumua\_don17 · 9月9日 13:38 · [社区讨论](https://news.ycombinator.com/item?id=49626373)

**「背景」** Anthropic 经济团队发布了一份题为《Economic Scenarios for Transformative AI》的工作论文（The Anthropic Institute Working Paper No. 2026-02），并配套推出一个交互式探索页面，对 2030 年人工智能对美国及全球经济可能产生的各种影响进行建模。该模型与报告由 Anton Korinek、Charles I. Jones、Szymon Sacher、Tess Cotter 和 Peter McCrory 共同撰写，页面标注为 2026 年 9 月发布的 1.0 版。这些内容试图系统化地呈现 AI 驱动经济增长、生产力变化以及不同情景下的不确定性。

**「社区讨论」** 多位评论者认为文章的经济推理颇为天真。用户 JacobiX 指出，如果 AI 能让一名护士完成过去两个人的工作，医院在成本压力下很可能会减少护士人数，而不是让护士花更多时间陪伴患者。其他评论还批评最不乐观的情景只是“LLM 没有产生重大影响”，却忽略了 AI 可能损害教育、注意力、社会信任、加剧贫富差距，以及数据中心过度建设导致经济危机或算力价格骤降等后果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/institute/econ-scenarios">Scenarios for our Economic Future \ Anthropic</a></li>
<li><a href="https://www-cdn.anthropic.com/files/4zrzovbb/website/cf58f84d46a4a76bf5a5b039ac695fba6b80041c.pdf">Economic Scenarios for Transformative AI</a></li>

</ul>
</details>

**标签**: `#economics`, `#artificial-intelligence`, `#future-of-work`, `#anthropic`, `#analysis`

---

<a id="item-tech-news-9"></a>
### [陶哲轩：AI 竞相解题或让研究者不再公开想法](https://simonwillison.net/2026/Sep/9/terence-tao/) ⭐️ 7.0/10

菲尔兹奖得主、数学家陶哲轩在 Mastodon 上警告说，好的、富有成效的开放问题正在被当作不可再生资源开采，可能变得稀缺。他指出，现在只要有人传言正在研究某个问题，就可能触发大量基于 AI 的努力去抢先“碾平”该问题，使原创研究来不及充分发挥潜力。这样的激励机制可能促使研究者不再向更广泛的社区分享任何有前景的研究方向，从而逆转数百年的开放科学传统，并对数学领域的长期未来造成严重损害。

rss · Simon Willison · 9月9日 00:20

**「背景：陶哲轩对 AI 开采开放数学问题的担忧」** 陶哲轩指出，识别有价值、有前景的开放数学问题正在变成一种稀缺资源，而 AI 驱动的大规模求解会对这些问题进行类似“非可再生”的开采。他进一步观察到，现在甚至只要出现某人正在研究某个问题的风声，就可能立刻引发大量 AI 辅助的尝试，赶在该原创研究项目成熟前将其“碾压”。这会导致研究者不愿再向更广泛的社群分享有前景的研究方向，从而可能逆转延续数百年的开放科学传统，并损害数学领域的长期发展。

**「影响」** 最直接的影响是数学研究者可能为避免想法被 AI 抢先破解而选择保密，减少公开开放问题的共享，长期或将拖慢数学领域的集体进步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Sep/9/terence-tao/">A quote from Terence Tao</a></li>
<li><a href="https://teorth.github.io/tao-web/ai-views.html">Terence Tao on AI — a living summary — Terence Tao</a></li>

</ul>
</details>

**标签**: `#ai-ethics`, `#open-science`, `#mathematics`, `#research`, `#ai-impact`

---

<a id="item-tech-news-10"></a>
### [美国防部被曝要求 OpenAI 开发低拒绝率军用模型](https://theintercept.com/2026/09/08/pentagon-openai-military-contract/) ⭐️ 7.0/10

据 The Intercept 泄露的文件显示，美国国防部在合同修订版“P00003”中要求 OpenAI 提供其人工智能技术的特殊军事版本，尽可能不频繁地拒绝军事指挥，即寻求“最低拒绝率”条款。该修订扩展了去年夏天国防部与 OpenAI 的原订交易。然而，OpenAI 和五角大楼均否认同意该语言，称泄露文件是草稿而非最终合同。OpenAI 发言人 Nate Evans 明确表示，公司从未同意要求“最低拒绝率”的合同语言，该内容未出现在已执行的合同中。此事引发对 OpenAI 与军方合作及 AI 安全伦理的广泛关注。

telegram · zaihuapd · 9月9日 09:02

**「背景」** OpenAI 与五角大楼的合作可以追溯到去年夏天签订的一份原型合同，其潜在价值据报最高可达 2 亿美元，合同期限为两年。此次泄露的 P00003 版更新文件据称是美国防部提出的草稿，其中包含寻求 OpenAI 模型“最低拒绝率”的语言，即模型尽可能少地拒绝军事指挥。OpenAI 发言人 Nate Evans 否认公司同意此类语言，表示最终执行的合同中并未出现该表述，但泄露文件与被否认内容之间的差异引发了对军方 AI 部署限制的疑问。

**「影响」** 若相关条款属实或未来被采纳，OpenAI 的技术在军事指挥中的人为监督和伦理约束可能被削弱，影响 AI 安全承诺的可信度；同时该事件警示科技公司与军方合作需警惕合同细节的透明度与公众信任风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://theintercept.com/2026/09/08/pentagon-openai-military-contract/">The Pentagon Asked OpenAI for Artificial Intelligence Designed to...</a></li>
<li><a href="https://www.unite.ai/openai-pentagon-contract-defines-mission-models-by-minimal-refusal-rates/">OpenAI Pentagon Contract Defines ‘Mission Models’ by Minimal ...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#OpenAI`, `#military AI`, `#contracts`, `#policy`

---

<a id="item-tech-news-11"></a>
### [OpenAI 将 AI 用于芯片设计，称成本低于开源模型](https://www.reuters.com/world/china/openai-offers-ai-chip-design-touts-cost-advantage-over-open-source-cfo-says-2026-09-09/) ⭐️ 7.0/10

OpenAI 首席财务官萨拉·弗里尔表示，公司正把 AI 拓展至芯片设计、生命科学和金融服务，并声称在云端部署降价后的 Luna 模型的成本低于中国开源替代方案。OpenAI 称，其自研 Jalapeno 芯片在 9 个月内完成设计定稿；Luna 降价 80% 后，使用量增加约 10 倍。这些说法目前仅来自公司单方面披露，尚缺乏独立验证。

telegram · zaihuapd · 9月9日 13:06

**「背景」** OpenAI 首席财务官萨拉·弗里尔在高盛 Communacopia 会议上表示，OpenAI 使用自家 AI 模型设计了自研 Jalapeño 芯片，并在不到 9 个月内完成了“流片”（tape-out），即芯片设计锁定并交付制造厂生产的阶段。与此同时，OpenAI 称其 Luna 云模型降价 80% 后使用量增长约 10 倍，且部署成本低于中国开源替代方案；不过这些说法目前主要基于公司自身声明，尚缺乏独立的公开验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/openai-cfo-sarah-friar-says-123936035.html">OpenAI CFO Sarah Friar says Luna undercuts Chinese AI on price</a></li>
<li><a href="https://insideai.news/news/ai-in-business/openai-chip-design-ai/9951/">OpenAI Offers AI for Chip Design, Undercuts Open-Source Costs</a></li>
<li><a href="https://forkast.news/openai-used-its-own-ai-models-to-design-the-jalapeno-chip-the-compute-landlord-thesis-just-went-recursive/">OpenAI Used Its Own AI Models to Design the Jalapeno Chip – The Compute Landlord Thesis Just Went Recursive</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Chip Design`, `#AI Models`, `#Cost Optimization`, `#Open Source`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [阿达尼企业机场子公司达成约 10 亿美元募资协议](https://www.cnbc.com/2026/09/09/adani-enterprises-airport-fundraise-shares.html) ⭐️ 8.0/10

阿达尼企业的机场子公司宣布，已与 Alpha Wave Global、Premji Invest、淡马锡和贝莱德管理的基金等投资者达成协议，以注资前估值约 180 亿美元募集约 981 亿卢比（10 亿美元）。投资者将分三批认购新股，最终合计持股约 5.54%，交易尚待常规条件和监管批准。

rss · CNBC Finance · 9月9日 06:26

**「背景」** 阿达尼机场控股目前在印度运营 8 座机场，占该国航空客运量逾 23%；此前母公司阿达尼企业已在 7 月完成一笔 1500 亿卢比的合格机构配售（面向大型机构投资者发行新股）。

**「影响」** 筹得资金将用于扩建和现代化机场设施、推进阿达尼机场城市项目，并扩大地勤等非航空业务，目标是把年客运能力提高到约 2 亿人次。

**标签**: `#Adani Enterprises`, `#airport infrastructure`, `#fundraising`, `#India`, `#Temasek`

---

<a id="item-finance-news-2"></a>
### [中国电动车企转向人形机器人：小鹏完成 9 亿美元融资并计划今年量产](https://www.cnbc.com/2026/09/09/chinas-ev-makers-shift-gears-to-focus-on-humanoids-as-car-market-slows.html) ⭐️ 7.0/10

在电动车市场增长放缓之际，小鹏汽车上月完成中国“具身智能”（硬件连接人工智能）行业规模最大的 9 亿美元融资；据花旗估计，该机器人业务估值超过 63 亿美元，与其电动车业务估值大致相当。小鹏表示，计划今年底开始量产机器人，首先用于自家门店和营业场所。

rss · CNBC Finance · 9月9日 04:12

**「背景」** 中国电动车销量正走向 2021 年以来最差的一年，汽车制造业 2026 年上半年平均利润率仅 1.5%，促使多家车企把机器人视为新的增长方向。

**标签**: `#China EV`, `#Humanoid robots`, `#Xpeng`, `#Robotics financing`, `#Auto industry`

---