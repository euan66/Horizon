---
layout: default
title: "Horizon Summary: 2026-09-07 (ZH)"
date: 2026-09-07
lang: zh
---

> 从 34 条内容中筛选出 9 条重要资讯。

---

**科技新闻**
1. [LLM 引导程序进化刷新 Packomania csqv 10 个实例最优解](#item-tech-news-1) ⭐️ 8.0/10
2. [216M 台 LG 智能电视被曝窃听与窥探隐私](#item-tech-news-2) ⭐️ 7.0/10
3. [TPU 推理外部化加速：InferenceX 声称性价比高 50%](#item-tech-news-3) ⭐️ 7.0/10
4. [Rustuna：高性能 Rust 版 Optuna 超参数优化库](#item-tech-news-4) ⭐️ 7.0/10
5. [KV 缓存作为智能体运行时的研究](#item-tech-news-5) ⭐️ 7.0/10
6. [华为时隔六年再发旗舰芯片：麒麟 9050 Pro 亮相](#item-tech-news-6) ⭐️ 7.0/10
7. [最高法 AI 纠纷司法解释明确换脸杀熟责任](#item-tech-news-7) ⭐️ 7.0/10

**科技博客**
1. [vLLM TT 插件：非 GPU 网格架构的接入实践](#item-tech-blog-1) ⭐️ 8.0/10

**财经新闻**
1. [中国宣布约 540 亿美元注资国有银行和保险商，规模低于预期](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [LLM 引导程序进化刷新 Packomania csqv 10 个实例最优解](https://www.reddit.com/r/MachineLearning/comments/1w9xlyi/llmguided_program_evolution_improves_10_bestknown/) ⭐️ 8.0/10

一项新研究使用 LLM 引导的程序进化方法迭代改进优化算法，而非直接求解圆填充问题。在 Packomania csqv 基准上，该方法在 15 次迭代内改善了 N=101 至 114 中 10 个实例的最佳已知半径和，提升幅度为 2.4% 到 5.4%。每个候选算法都通过独立验证器评分，成功保留、失败丢弃，累计 LLM 成本仅 27.72 美元。Packomania 已独立接受这些结果，论文与代码分别发布于 arXiv:2609.05093 和 GitHub 上的 discovery-loop 仓库。

reddit · r/MachineLearning · /u/SIGH\_I\_CALL · 9月7日 16:54

**「背景」** 圆填充（circle packing）是经典几何优化问题。Packomania 的 csqv 基准要求将 N 个半径可变的圆放入单位正方形，并使半径之和最大化；此类问题在多圆情况下极难精确求解，通常以数值寻优刷新纪录。LLM 引导的程序进化并不直接让大模型给出圆的坐标，而是从简单种子求解器出发，由 LLM 根据得分板和尝试历史提出算法改动，再经独立验证器评估后保留改进。工具资料确认，该方法在 N=101 到 114 的 10 个实例上刷新了 Packomania 的最优纪录，并经过独立验证和接受。

**「影响」** 对于使用 Packomania csqv 基准的优化研究者，N=101–114 中 10 个实例的已知最优半径和值已被更新，且由基准维护方独立确认。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.05093">[2609.05093] LLM - Guided Program Evolution for Circle Packing ...</a></li>
<li><a href="https://arxiv.org/html/2609.05093">LLM - Guided Program Evolution for Circle Packing :Breaking 10...</a></li>

</ul>
</details>

**标签**: `#LLM`, `#program evolution`, `#optimization`, `#circle-packing`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [216M 台 LG 智能电视被曝窃听与窥探隐私](https://www.youtube.com/watch?v=6IFVTcM28KA) ⭐️ 7.0/10

YouTube 视频和 Notebookcheck 报道指出，LG 智能电视存在大量侵犯隐私的行为：即使用户关闭屏幕也会记录音频，并扫描本地网络中的其他设备；涉及约 2.16 亿台电视。LG 的条款还要求用户自行负责告知并征得家中或附近所有可能被收音的第三方同意，否则可能违约。评论区的用户反映，实际应对手段包括禁用电视的全部网络功能，或在退货期后拆开后盖拔掉 Wi‑Fi/蓝牙模块。该问题因规模巨大和合同条款苛刻而引发广泛关注，但在法律上是否触犯窃听法规仍无定论。

hackernews · treve · 9月7日 00:22 · [社区讨论](https://news.ycombinator.com/item?id=49592375)

**「背景」** 智能电视通常内置麦克风和网络模块，用于语音助手、内容推荐和远程控制等功能。这项调查由 Gamers Nexus 进行，测试发现 LG 智能电视会在屏幕关闭时捕捉麦克风音频，并在联网后上传数据；同时还会扫描本地网络以绘制手机和其他设备的信息。LG 的条款也要求用户自行负责取得第三方同意，提示其声音可能被捕捉和处理。此类事件反映出智能设备厂商数据收集行为所引发的隐私担忧。

**「影响」** 对 LG 智能电视用户而言，最直接的影响是安装使用这些设备即可能同时承担隐私泄露和向所有在场者告知并获得同意的合同义务；部分用户选择永久断开电视的网络/蓝牙硬件来规避。不过，其是否构成违法窃听仍未获法律裁定。

**「社区讨论」** 评论普遍批评 LG 的做法，称其服务条款“糟糕”，并指出除了指纹识别，电视还会主动嗅探周边设备；用户则分享了自己禁用网络或拆掉 Wi‑Fi/蓝牙芯片的实际做法。也有人提出疑问：即使机主通过条款同意，未同意的家庭成员和客人可能使 LG 或机主面临窃听责任，希望看到相关诉讼。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.notebookcheck.net/LG-smart-TVs-caught-logging-audio-with-screen-off-and-snooping-on-local-devices.1391214.0.html">LG smart TVs caught logging audio with screen off and snooping ...</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2laeXVqNEVSRUJZTzNfVVdzblZDZ0FQAQ?hl=en-IN&amp;gl=IN&amp;ceid=IN:en">See the latest updates, context and perspectives about this story.</a></li>

</ul>
</details>

**标签**: `#privacy`, `#smart-tv`, `#security`, `#IoT`, `#LG`

---

<a id="item-tech-news-3"></a>
### [TPU 推理外部化加速：InferenceX 声称性价比高 50%](https://newsletter.semianalysis.com/p/tpu-inferencex-full-steam) ⭐️ 7.0/10

SemiAnalysis 报道称，谷歌正在快速推进 TPU 推理栈的外部化，相关项目名为 InferenceX。该分析指出，InferenceX 在每美元性能上可比现有方案高出最多 50%，并且客户群正在扩大。报道还提及 Ironwood 与 TPUv8i 的进展，认为这正在削弱英伟达 CUDA 生态的护城河。目前关于具体部署条件、硬件规格和定价的细节仍然有限。

rss · Semianalysis · 9月7日 20:00

**「背景」** TPU 是谷歌自研的 AI 加速器芯片，过去主要供内部使用，近年来通过 Google Cloud 逐步开放给外部客户。据 SemiAnalysis 报道，谷歌正在加速将 TPU 推理栈“外部化”（externalization），并提到其性能每美元最高可提升 50%，同时涉及 Ironwood/TPUv8i 等新品。外部化的深化正在削弱 NVIDIA CUDA 生态的软件护城河。

**「影响」** 对使用或评估云 AI 推理算力的企业与开发者而言，Google TPU（含 Ironwood/TPUv8i）推理能力加速外化并宣称性能/美元最高提升 50%，将提供比肩 NVIDIA GPU 的新成本与选型选项；同时，这一外化进程有助于削弱 NVIDIA 的 CUDA 生态壁垒。不过，Google 自身也面临供应约束，实际可用性和大规模性能仍需检验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://newsletter.semianalysis.com/p/tpu-inferencex-full-steam">TPU Inference Externalization Full Steam Ahead - InferenceX</a></li>
<li><a href="https://www.techpowerup.com/343957/google-prepares-tpuv8ax-for-training-and-tpuv8x-for-inference">Google Prepares TPUv 8 ax for Training and... | TechPowerUp</a></li>
<li><a href="https://wccftech.com/google-splits-tpuv8-strategy-two-chips-broadcom-training-mediatek-inference-duties/">Google Splits TPUv 8 Strategy Into Two Chips, Handing Broadcom...</a></li>
<li><a href="https://newsletter.semianalysis.com/p/tpuv7-google-takes-a-swing-at-the">Google TPUv7: The 900lb Gorilla In the Room</a></li>
<li><a href="https://fourweekmba.com/ai-google-tpu-selling-renting-compute-alphabet-q2-2026/">Google Is Selling TPUs and Renting Outside... - FourWeekMBA</a></li>

</ul>
</details>

**标签**: `#TPU`, `#AI inference`, `#hardware`, `#Google Cloud`, `#CUDA`

---

<a id="item-tech-news-4"></a>
### [Rustuna：高性能 Rust 版 Optuna 超参数优化库](https://www.reddit.com/r/MachineLearning/comments/1w9nyhz/rustuna_a_highperformance_rust_implementation_of/) ⭐️ 7.0/10

Optuna 团队发布了 Rustuna，这是一个基于 Rust 编写的 Optuna 兼容实现，旨在提供高速度和低内存占用。它保持 Optuna 的熟悉 API 和概念，同时实现零 Python 依赖，以降低供应链攻击风险，并通过 Rust 原生内存管理提高效率。项目托管在 GitHub（optuna/rustuna），并附有 Medium 博客文章介绍详情。

reddit · r/MachineLearning · /u/c-bata · 9月7日 10:01

**「背景」** Optuna 是一个广泛使用的 Python 超参数优化框架，通常需要通过 Python 包管理安装并引入依赖。Rustuna 重新实现了兼容 Optuna 的 API，但不依赖 Python 运行时，从而减少了依赖链风险并优化了内存管理。

**「影响」** 现有 Optuna 用户可以在需要更低内存占用和更强依赖安全性的场景中评估迁移到 Rustuna，但需要注意其兼容性仍取决于 API 实现的完整性。

**标签**: `#rust`, `#optuna`, `#hyperparameter-optimization`, `#machine-learning`, `#performance`

---

<a id="item-tech-news-5"></a>
### [KV 缓存作为智能体运行时的研究](https://www.reddit.com/r/MachineLearning/comments/1w9myqc/kv_cache_as_an_agent_runtime_r/) ⭐️ 7.0/10

Yandex 研究团队提出一种替代思路：通过修改 LLM 的推理状态（KV 缓存），将 KV 缓存用作智能体运行时，以提升系统的交互性和响应能力。该思路已在其实验室此前的论文“Hogwild\! Inference”和“AsyncReasoning”中使用；博客文章还预览了未来工作：一个 Qwen3.8-27B 智能体利用类似技术交互式地游玩 DOOM 环境。Reddit 帖子试图探讨模型推理/运行时设计本身是否是被忽视的智能体能力维度，与模型和 harness 并列，并提出了“harness 过于抽象、修改模型成本过高，是否需要介于两者之间的层次”的问题。该提交本身缺少详细技术内容和独立评估，属于有价值的研究方向而非突破性成果。

reddit · r/MachineLearning · /u/\_puhsu · 9月7日 09:03

**「背景」** KV 缓存（Key-Value cache）是 Transformer 模型推理时存储注意力键和值的中间状态，传统上被视为提高生成速度的临时缓存。Yandex 研究团队提出将其视为“代理运行时”（agent runtime），即通过直接修改模型的推理状态（KV 缓存）来影响和操控模型行为，而不是仅仅更换模型提示词或外部编排框架。他们的想法建立在之前的工作如 Hogwild\! Inference 和 AsyncReasoning 之上，这些工作探索了在模型推理过程中进行更灵活的状态修改，以提升 LLM 的交互性和响应能力；AsyncReasoning 的代码已公开在 GitHub 上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/yandex-research/AsyncReasoning">GitHub - yandex-research/AsyncReasoning · GitHub</a></li>

</ul>
</details>

**标签**: `#kv-cache`, `#llm-agents`, `#inference`, `#machine-learning`, `#interactive-ai`

---

<a id="item-tech-news-6"></a>
### [华为时隔六年再发旗舰芯片：麒麟 9050 Pro 亮相](https://www.news.cn/20260907/adf46c5c003240d28cc3cf6de54f9b5f/c.html) ⭐️ 7.0/10

华为 7 日在广州发布 Mate XT 2 三折叠手机，搭载全新麒麟 9050 Pro 芯片。这是继 Mate40 全球发布会之后，华为时隔六年再次在旗舰发布会上推出全新麒麟芯片。按新华社介绍，麒麟 9050 Pro 被称为首款采用逻辑折叠技术的高性能芯片：它在单芯片内将逻辑单元分层排布，并增设垂直互联通道，从而缩短信号传输路径、降低时延并改善性能。简讯未说明制程、主频、功耗、跑分和供货量等关键参数。

telegram · zaihuapd · 9月7日 08:20

**「背景」** 麒麟是华为自研的移动处理器系列，此前 Mate 40 系列搭载的麒麟 9000 等芯片广为人知，但受制裁等因素影响，华为旗舰机型多年未再推出全新麒麟平台。此次发布的麒麟 9050 Pro 是时隔约六年后再次在旗舰发布会上亮相的全新麒麟芯片，采用所谓“逻辑折叠”技术，将逻辑单元在单芯片内分层排布，并借助垂直互联通道连接，以缩短信号传输路径、降低时延。该芯片随 Mate XT 2 三折叠手机在广州发布。

**「影响」** 对于 Mate XT 2 用户和关注麒麟芯片路线的开发者，这是华为时隔六年后再次将全新旗舰级麒麟芯片投入量产机型，信号路径缩短与低时延的宣称若得到实测验证，将直接影响整机的性能与能效表现。具体竞争优势仍需等待更详细的芯片参数和第三方测试数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/0/999/300.htm">华为继 Mate 40 后时隔六年再次发布高性能芯片，麒麟 9050 Pro 首发逻辑折叠技术 - IT之家</a></li>
<li><a href="https://www.sina.cn/news/detail/5340531733564063.html">华为麒麟 9050 Pro 芯片性能参数|华为|麒麟 9050 pro|mate xt 2_新浪新闻</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#hardware`, `#Huawei`, `#chip-design`, `#mobile`

---

<a id="item-tech-news-7"></a>
### [最高法 AI 纠纷司法解释明确换脸杀熟责任](https://www.cnr.cn/news/20260907/t20260907_527806795.shtml) ⭐️ 7.0/10

最高人民法院于 9 月 7 日发布人工智能纠纷案件司法解释，全文共 5 部分 24 条，聚焦 AI 换脸、算法杀熟、冒充他人代言、自动驾驶和知识产权等问题。解释明确，未经同意使用 AI 制作可识别的人脸、声音等可能构成人格权侵权；算法价格歧视侵害消费者权益的应承担责任；AI 冒充他人代言诱导消费的，可依法支持惩罚性赔偿请求。解释还规制利用人工智能实施“网络开盒”“人肉搜索”等侵害自然人隐私权的行为。这是我国在 AI 民事侵权责任领域出台的专项司法解释，为相关纠纷提供了更明确的法律依据。

telegram · zaihuapd · 9月7日 09:32

**「背景」** 随着生成式人工智能和算法推荐技术的普及，AI 换脸、算法差异化定价以及 AI 冒充他人代言等应用引发越来越多民事权益纠纷，但原有法律在责任认定上存在模糊地带。最高人民法院此次发布司法解释，是对民法典等现行法律在 AI 场景下的适用细化，有助于统一裁判尺度。

**「影响」** 对在中国开发和应用 AI 换脸、智能推荐、虚拟代言等技术的企业和平台而言，该解释将直接提高相关场景下的合规与风控要求，尤其是未经同意的肖像、声音处理和算法价格歧视行为。

**标签**: `#AI regulation`, `#AI liability`, `#deepfake`, `#algorithmic pricing`, `#China law`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [vLLM TT 插件：非 GPU 网格架构的接入实践](https://vllm.ai/blog/2026-09-07-vllm-tt-plugin) ⭐️ 8.0/10

rss · vLLM Blog · 9月7日 00:00

**「背景」** vLLM 的 V1 调度器默认按 token 预算把 prefill 与 decode 混在同一批，并行度也以 TP/PP rank 表达；而 Tenstorrent 硬件把模型按整套网格编译并追踪成一次执行。作者认为，若为这种硬件去改动 vLLM 核心，支持就会困在落后上游的分叉上。

**「方案」** 插件以标准 out-of-tree 平台机制注册 TTPlatform，仅在 ttnn 可导入时生效；模型经 TT 前缀架构名解析到 TT-Metal 的 TTNN 实现，插件自身不携带模型代码。调度上每一步只能是 prefill-only、decode-only 或空，chunked prefill 会穿插 decode-only 步骤以保持 trace 形状稳定，连续性 batching 仍成立，但切换粒度为完整 step，且每次切换会排空异步 readback。对单执行体 Galaxy 模型，作者放弃多进程 DP，改为单进程内由 TTLaneCoordinator 管理多个独立 lane，并为每步选择一个共享模式、合并一次设备提交；若强制 prefill 未接纳 token 就重试为 decode，避免 KV 压力造成无进展循环。设备端采样在未请求 logprobs、惩罚等能力时直接返回 token，否则按 batch 回退到主机路径；“async decode”本质是异步主机 readback，通过深度 2 的队列与 ttnn event 同步，只在稳态生成时保持重叠。文章也明确列出当前边界：尚无 speculative decoding、LoRA、prompt logprobs 与多主机服务，TP/PP 由 mesh 形态决定。

**「启示」** 作者以此论证 vLLM 的插件与可插拔调度器接口足够通用，能让网格硬件以受限调度、单进程 lane DP 和设备端采样等方式接入而不必分叉核心；这也为其他非 GPU 后端提供了可借鉴的扩展路径。

**标签**: `#vLLM`, `#Tenstorrent`, `#LLM inference`, `#hardware plugin`, `#scheduler design`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国宣布约 540 亿美元注资国有银行和保险商，规模低于预期](https://www.cnbc.com/2026/09/07/china-state-banks-lenders-insurers-capital-solvency-bankrupt-nim-.html) ⭐️ 7.0/10

中国政府宣布向多家国有银行和保险商注资合计约 360 亿元人民币（合 540 亿美元），规模小于市场预期；财政部、中国烟草等将通过定向增发和直接注资等方式补充资本，农行和工行分别拟募资不超过 1600 亿元和 1000 亿元。消息公布后相关港股股价周一下跌，农行跌 2.7%，工行跌 2.3%。

rss · CNBC Finance · 9月7日 09:26

**「背景」** 此前北京去年已向四家国有大行注资 5000 亿元人民币，并计划今年发行 3000 亿元特别国债补充大型银行资本。这一轮注资是首次覆盖保险商，行业偿付能力充足率已从去年 204.5%降至第二季度末的 180.6%。

**「影响」** 分析师认为，资本补充能为银行处置坏账提供缓冲，但由于当前制约放贷的是疲弱的信贷需求而非资本不足，短期内对经济影响有限。

**标签**: `#China`, `#banking`, `#recapitalization`, `#financial policy`, `#insurers`

---