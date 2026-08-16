---
layout: default
title: "Horizon Summary: 2026-08-16 (ZH)"
date: 2026-08-16
lang: zh
---

> 从 32 条内容中筛选出 7 条重要资讯。

---

**科技新闻**
1. [Anthropic 发布 Claude 官方系统提示词](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8 27B：开源视觉模型能力出色，但默认过度思考](#item-tech-news-2) ⭐️ 8.0/10
3. [SSOG-Attention：可分离高斯和实现亚二次复杂度注意力](#item-tech-news-3) ⭐️ 8.0/10
4. [Cloudflare 切换域名服务器后静默注入分析脚本](#item-tech-news-4) ⭐️ 7.0/10
5. [PJM 建模失误浪费 120 亿美元，且可能重演](#item-tech-news-5) ⭐️ 7.0/10
6. [重新审视 ECA 论文：跨通道交互并非关键](#item-tech-news-6) ⭐️ 7.0/10

**财经新闻**
1. [Anthropic 第二季初步营收超 115 亿美元，同比增长逾 14 倍](#item-finance-news-1) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Anthropic 发布 Claude 官方系统提示词](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic 在 Claude 平台文档中正式发布了 Claude 模型的官方系统提示词，首次让开发者和研究者能直接查看并追踪这些提示词的变化。该发布为提示工程和模型可解释性提供了罕见的透明性，外界已开始用版本控制工具逐次对比不同模型版本间的差异；例如 Simon Willison 将提示词重建为 Git 提交历史，并指出 Opus 4.8 与 Opus 5 之间的差异片段。官方文档还披露了若干行为准则，包括危机对话优先考虑用户福祉、以及模型会自行检查是否真的存在图片而非仅凭提示词推断。这一举措并非范式转移，但属于高价值的透明度更新，有助于理解 Anthropic 对未来模型行为的规划。

hackernews · tosh · 8月16日 12:48 · [社区讨论](https://news.ycombinator.com/item?id=49319556)

**「背景」** 系统提示词（system prompt）是在每次对话开始时附加给 Claude 的一组指令和上下文信息，用于提供当前日期等最新数据并引导模型行为。Anthropic 会在官方文档中随每次模型发布更新并公开这些系统提示词，使开发者能够查看和追踪其变化。例如，Claude Opus 4 和 Claude 的新版模型提示词均已以这种方式公布。

**「影响」** 开发者现在可以直接依据官方系统提示词开展提示工程实验，并借助社区维护的版本历史比较不同模型版本之间的行为设定差异，从而减少对逆向工程或二手信息的依赖。

**「社区讨论」** 社区讨论中，Simon Willison 提供了将提示词转换为 Git 提交历史的工具，方便对比模型版本差异；有人评论称某些系统提示是在用明文规定替代模型本应具备的常识判断，也有人提醒这些提示词只是塑造行为的层次化系统中的一部分，不能单独解读为模型能力或路线图的全部。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/release-notes/system-prompts">System Prompts - Claude Platform Docs</a></li>
<li><a href="https://tactiq.io/learn/claude-system-prompt">Claude System Prompt Explained: What&#x27;s Inside and Why It Matters</a></li>
<li><a href="https://simonwillison.net/2025/May/25/claude-4-system-prompt/">Highlights from the Claude 4 system prompt</a></li>

</ul>
</details>

**标签**: `#claude`, `#system-prompts`, `#prompt-engineering`, `#anthropic`, `#ai-transparency`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B：开源视觉模型能力出色，但默认过度思考](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

阿里巴巴 Qwen 实验室于 8 月 16 日发布 Apache 2.0 许可的 Qwen 3.8 27B，这是一款 27B 参数的视觉理解 LLM，尺寸适合在配置较好的笔记本上本地运行。Qwen 自报的基准显示该模型同时超越前代 Qwen 3.6 27B 和此前最强的闭源模型 Qwen 3.7-Plus，但尚待独立基准验证。Simon Willison 在 M5 Max MacBook Pro 和 NVIDIA DGX Spark 上通过 LM Studio 的 17GB Q4\_K\_M 量化版及 llama-server 进行了测试。模型默认的 reasoning\_effort 为 xhigh，导致严重的“过度思考”：让他画一个 SVG 圆时消耗大量推理 token，产出了远超请求的动画圆；画鹈鹕骑自行车的 SVG 用时 21 分钟，生成 22,276 个推理 token 和 3,223 个输出 token，而关闭推理后同样提示仅用约 137 秒生成 3,715 token。作者强烈建议在本地运行时先使用 low 或关闭推理级别，并指出该模型在图像边界框任务上表现出色。

rss · Simon Willison · 8月16日 22:00

**「背景」** Qwen 3.8 27B 是阿里 Qwen 实验室继 Qwen 3.6 27B 之后的新一代 27B 参数开源模型；27B 被社区视为本地部署的“甜点”规格，可在高性能笔记本上用量化方式运行。此次模型引入官方的 reasoning\_effort 参数，提供 xhigh、medium、low 三档，xhigh 被设为默认值，用于复杂任务，但会在简单请求上也产生大量内部推理。

**「影响」** 对本地部署用户来说，不改默认设置会使 8,192 token 的默认上下文在简单问题上被推理内容占满，单次生成可能需要数分钟到二十多分钟；在 LM Studio 中调低或关闭推理级别（并加大上下文长度）后，它在消费级硬件上依然能产出高质量的 SVG 和视觉结果。

**标签**: `#Qwen`, `#LLM`, `#open source`, `#AI`, `#benchmarks`

---

<a id="item-tech-news-3"></a>
### [SSOG-Attention：可分离高斯和实现亚二次复杂度注意力](https://www.reddit.com/r/MachineLearning/comments/1vpt6ay/ssogattention_sum_of_separable_gaussians_as_a/) ⭐️ 8.0/10

Reddit 用户 /u/4rtemi5 发布了 SSOG-Attention，一种基于可分离高斯和的注意力机制，旨在替代缩放点积注意力（SDPA）。它将复杂度从 SDPA 的 O\(N²·d\) 降低到 O\(N·√N·d\)，通过为每个注意力头学习少量高斯原子，并根据查询 token 以几何方式调整它们。实验表明，在 CIFAR-100 等小数据集上 SSOG 明显优于 SDPA，在 ImageNet-1k（IN1k）上性能相当且收敛更快，同时在更大规模上更省内存、更快。作者提供了博客文章和 GitHub 仓库，并说明代码与部分博客内容使用了 AI 辅助，但作者对项目内容负责。目前该方法尚未经过同行评审和大规模外部验证。

reddit · r/MachineLearning · /u/4rtemi5 · 8月16日 10:06

**「背景」** 缩放点积注意力（SDPA）会计算所有查询 token 与所有键/图像 token 之间的相似度分数，因此计算和内存复杂度为 O\(N²·d\)。SSOG 的思路是让每个注意力头学习若干个可分解（可分离）的高斯原子，并根据查询 token 对它们进行几何引导，从而避免显式构造完整的 N×N 注意力矩阵。

**「影响」** 对高分辨率视觉模型或长序列场景，SSOG 可在保持与 SDPA 相当性能的同时将注意力复杂度降至 O\(N·√N·d\)，从而减少训练和推理的显存占用与时间开销。

**标签**: `#attention mechanisms`, `#sub-quadratic complexity`, `#efficient transformers`, `#computer vision`, `#Gaussian kernels`

---

<a id="item-tech-news-4"></a>
### [Cloudflare 切换域名服务器后静默注入分析脚本](https://news.ycombinator.com/item?id=49322107) ⭐️ 7.0/10

用户 stagas 在 Hacker News 报告，约数小时前为在自有子域名上提供 R2 存储桶服务而把域名服务器切换到 Cloudflare 后，发现 Cloudflare 静默向其纯 HTML、无 JavaScript 的站点 textlog.cc 注入了 JS 分析脚本。用户必须进入 Analytics 仪表盘、添加站点并随后禁用该片段才能移除，因而认为这种默认为开启、需要手动退出的做法侵入性强。Cloudflare 官方博客也介绍了 Web Analytics 自动启用机制；社区成员 purpleidea 提供了被注入脚本的示例，指向 static.cloudflareinsights.com/beacon.min.js，并带有 data-cf-beacon 与版本 token。部分评论指出，若域名仅用于 DNS 且未开启 Cloudflare 代理，则不会观察到注入，因此触发条件可能与是否使用 Cloudflare 代理有关。该事件提醒站点所有者在切换域名服务器或启用代理后检查 Cloudflare Web Analytics 设置并主动关闭自动注入。

hackernews · stagas · 8月16日 17:49

**「背景」** Cloudflare 同时提供权威域名服务器、CDN 反向代理和 R2 对象存储等服务；当站点通过 Cloudflare 代理时，Cloudflare 可以改写经过的 HTML 响应。Cloudflare Web Analytics 通过向页面注入 beacon.min.js 脚本来收集访问统计，官方曾默认对部分站点启用该功能，用户可以手动在仪表盘中关闭。HTML-only 或重视隐私的站点尤其容易受到这种注入的影响，因为它改变了原始响应内容并引入外部请求。

**「影响」** 对于通过 Cloudflare 代理且未主动启用分析的站点，切换域名服务器后可能被静默注入 Web Analytics 脚本，用户需手动在仪表盘关闭。仅将 Cloudflare 用于 DNS 且不启用代理的域名通常不会出现该注入。

**「社区讨论」** 评论中，okzgn 建议通过 CSP meta 标签限制 script-src，只允许加载自托管或指定来源的脚本；dchest 引用了 Cloudflare 官方博客介绍自动启用 Web Analytics 的文章；purpleidea 提供了被注入脚本的完整示例。还有评论者询问用户是否使用 Cloudflare 代理，并提到仅 DNS-only 的域名没有启用 Web Analytics，表明触发条件可能与代理模式相关。

**标签**: `#Cloudflare`, `#privacy`, `#web analytics`, `#DNS`, `#site owners`

---

<a id="item-tech-news-5"></a>
### [PJM 建模失误浪费 120 亿美元，且可能重演](https://newsletter.semianalysis.com/p/12b-of-us-ratepayers-money-wasted) ⭐️ 7.0/10

SemiAnalysis 的分析指出，美国电网运营商 PJM 因建模失误浪费了高达 120 亿美元的费率人资金，而该机构正面临再次犯下类似错误的风险。文章标题称，“美国最伟大的电网”把数十亿美元和缴费者置于风险之中，问题在于使用了错误的模型——不是人工智能模型，而是电网建模模型。这一事件暴露了关键基础设施中模型验证的严重缺陷；若 PJM 在新流程中继续沿用同类做法，用户可能承受进一步损失。

rss · Semianalysis · 8月16日 22:27

**「背景信息」** PJM 互联是美国最大的电网运营商，负责通过容量拍卖来确保未来电力供应，相关成本最终由用户电费承担。据外部资料，数据中心需求的激增已导致 PJM 容量拍卖成本大幅上升（例如被称为“164 亿美元可靠性税”的事件），并引发“结构性稀缺”的警告，监管机构 FERC 也被批评未能充分保护用户。在此背景下，文章指出的建模错误造成了 120 亿美元浪费，并担忧 PJM 可能重蹈覆辙。

**「影响」** PJM 的建模失误正使整个区域的用户承担数十亿美元的额外容量成本，而 PJM 提出的可靠性后备采购和可靠性必须运行（RMR）协议（如为 Talen Energy 的 Brandon Shores 和 H.A. Wagner 发电机组支付费用）可能让马里兰州等地的用户进一步增加支出。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.utilitydive.com/news/ferc-data-center-pjm-transmission-costs/825760/">FERC fails to shield PJM consumers from data center transmission costs: ratepayer advocates | Utility Dive</a></li>
<li><a href="https://avanzaenergy.substack.com/p/the-164-billion-reliability-tax-how?action=share">The $16.4 Billion Reliability Tax: How Data Centers Broke PJM&#x27;s Capacity Auction</a></li>
<li><a href="https://www.capitalgazette.com/2026/05/11/pjm-warns-maryland-energy-bills/">Maryland ratepayers could pay billions as PJM issues grid warning</a></li>
<li><a href="https://www.rtoinsider.com/138882-maryland-fears-pjm-backstop-effort-could-raise-ratepayer-costs/">Maryland Ratepayers at Risk from PJM Backstop, Advocate Says</a></li>
<li><a href="https://rtowww.com/85586-maryland-report-details-pjm-cost-increases-for-ratepayers/">Maryland Report Details PJM Cost Increases for Ratepayers</a></li>

</ul>
</details>

**标签**: `#modeling`, `#energy grid`, `#software error`, `#infrastructure`, `#analysis`

---

<a id="item-tech-news-6"></a>
### [重新审视 ECA 论文：跨通道交互并非关键](https://www.reddit.com/r/MachineLearning/comments/1vptaw9/revisiting_the_efficient_channel_attention_paper/) ⭐️ 7.0/10

Reddit 用户 arkuto 发文批评高效通道注意力（ECA）的核心设计，认为在通道均值上做一维卷积缺乏通道拓扑支撑，类似在表格数据上使用 CNN。作者用国际象棋 6 子残局表数据进行实验，发现 k=1、即完全没有跨通道交互的 ECA（平均测试准确率 96.61%）仍明显优于 Squeeze-and-Excitation（SE，96.17%）并接近 k=3 的 ECA（96.68%）。这表明原文“跨通道交互是关键”的假设可能不成立，且官方与常用复现库（timm 等）几乎都没有做纯 k=1 消融。作者建议除了真实数据集外，也应使用可完整采样、无过拟合风险的人造数据集来区分架构效率和隐式正则化效果。

reddit · r/MachineLearning · /u/arkuto · 8月16日 10:13

**「背景」** ECA 是 SE 的后续改进，SE 先把通道均值压到小隐藏层再恢复，ECA 则直接用一维卷积在通道均值上滑动，以避免降维并实现跨通道交互。但卷积假设数据有空间或时间那样的拓扑和局部性，而通道之间没有这种固定顺序，因此该设计在概念上存疑。作者在完整可采样的象棋残局数据上做实验，希望把架构效果与数据偏置或隐式正则化分开。

**「影响」** 对使用或复现 ECA 的研究者，这一结果提示需要测试 k=1 这一“退化”设置，否则可能高估跨通道交互的作用；同时也说明，在不完整数据集上的性能提升可能来自隐式正则化而非核心架构机制，需要更严谨的消融与合成数据验证。

**标签**: `#Efficient Channel Attention`, `#deep learning`, `#attention mechanisms`, `#computer vision`, `#critical analysis`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Anthropic 第二季初步营收超 115 亿美元，同比增长逾 14 倍](https://www.cnbc.com/2026/08/15/anthropic-revenue-jumps-to-over-11point5-billion-in-q2-report.html) ⭐️ 8.0/10

彭博社援引文件称，Anthropic 今年第二季初步营收超过 115 亿美元，较去年同期的 7.87 亿美元增长逾 14 倍，也高于今年第一季的 47.3 亿美元；当季调整后营业利润转正。以上为初步数据，仍可能调整。公司正筹备可能在今秋启动的大型 IPO。

telegram · zaihuapd · 8月16日 07:26

**「背景」** Anthropic 是一家开发和运营生成式 AI 助手 Claude 的 AI 安全与研究公司；本季营收为初步数据，最终财报可能调整。

**「影响」** 若最终数据确认，这组数字将成为市场评估 Anthropic 估值以及潜在 IPO 定价的重要参考，但最终结果仍可能有变动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://forgeglobal.com/insights/how-to-invest-in-anthropic-pre-ipo/">Insights: How to Invest in Anthropic Pre-IPO - Forge</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#earnings`, `#AI industry`, `#IPO`, `#revenue growth`

---