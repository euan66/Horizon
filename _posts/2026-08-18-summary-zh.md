---
layout: default
title: "Horizon Summary: 2026-08-18 (ZH)"
date: 2026-08-18
lang: zh
---

> 从 38 条内容中筛选出 13 条重要资讯。

---

**科技新闻**
1. [Qwen 3.8 27B 在智能指数上获 52 分，追平更大规模的 GPT-5.6 Luna](#item-tech-news-1) ⭐️ 9.0/10
2. [Linux 7.3 改进显存耗尽时的 VRAM 过量分配性能](#item-tech-news-2) ⭐️ 8.0/10
3. [Mojo 开源：Apache 2.0 发布编译器与工具链](#item-tech-news-3) ⭐️ 8.0/10
4. [Turbovec：Rust 实现的 TurboQuant 向量搜索库](#item-tech-news-4) ⭐️ 7.0/10
5. [用 20 美元工具修复 Framework 13 的 BIOS 变砖](#item-tech-news-5) ⭐️ 7.0/10
6. [摄像头版 AirPods B790 现身，macOS 26.7 演示视觉智能](#item-tech-news-6) ⭐️ 7.0/10
7. [macOS 26.7 代码揭示中国大陆 Apple 智能写作工具审查机制](#item-tech-news-7) ⭐️ 7.0/10
8. [中国要求政府机构提前卸载定制版 Windows 10](#item-tech-news-8) ⭐️ 7.0/10
9. [国产 AI 芯片 2026 年将占中国近 90% 寒武纪华为受益](#item-tech-news-9) ⭐️ 7.0/10

**财经新闻**
1. [贵州茅台净利罕见下滑，折射中国经济与消费结构转变](#item-finance-news-1) ⭐️ 8.0/10
2. [债市压力挤压美国家庭：房贷与柴油成本上升](#item-finance-news-2) ⭐️ 8.0/10
3. [汇丰要求部分内地投资客户提交资金来源声明，逾期或终止服务](#item-finance-news-3) ⭐️ 7.0/10
4. [苹果美国 App Store 佣金收入降 18%，二季度用户消费额同比下降 6%](#item-finance-news-4) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Qwen 3.8 27B 在智能指数上获 52 分，追平更大规模的 GPT-5.6 Luna](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 9.0/10

据 Simon Willison 报道，Qwen 3.8 27B 在 Artificial Analysis Intelligence Index 上获得 52 分，与 GPT-5.6 Luna（最大值）持平，仅比 GLM-5.2（最大值，753B 参数）和 DeepSeek V4 Pro 0813（最大值，1.7T 参数）低 1 分；Luna 的规模未知，但很可能远大于 27B。Qwen 3.8 27B 是一个参数仅为 27B 的模型，却在该指数上达到与远大规模模型相近的分数，显示出模型效率上的显著进展。Simon Willison 称这是一个“真正令人惊讶的模型”，消息经由 Hacker News 传播。需要注意的是，该分数仅代表这一个指数上的表现，实际能力仍需更多评估。

rss · Simon Willison · 8月17日 23:58

**「背景信息」** Artificial Analysis Intelligence Index 是一个公开的模型智能评测指标，用于横向比较不同大语言模型的综合能力，例如 Qwen3.8 27B 在该指数上得到 52 分，明显高于同类模型的中位数 9 分。该模型是开源权重模型，支持文本和图像输入、文本输出，并拥有 256k tokens 的上下文窗口。此次成绩之所以受关注，是因为它以 27B 参数的小规模达到了与 GPT-5.6 Luna、GLM-5.2 和 DeepSeek V4 Pro 等更大模型相当或接近的分数，体现出模型效率的显著提升。

**「影响」** 对于关注本地部署或低推理成本的开发者而言，Qwen 3.8 27B 的这一成绩意味着在 Artificial Analysis Intelligence Index 这一项指标上，一个 27B 参数的开源模型可以接近甚至追平规模大得多的前沿模型，但这并不能直接证明它在所有实际任务中都有同等表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-8-27b">Qwen3.8 27B Intelligence , Performance &amp; Price Analysis</a></li>

</ul>
</details>

**标签**: `#ai`, `#llms`, `#qwen`, `#benchmarks`, `#model-efficiency`

---

<a id="item-tech-news-2"></a>
### [Linux 7.3 改进显存耗尽时的 VRAM 过量分配性能](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

Flaburgan 在 pixelcluster.dev 发表文章，介绍标题所称的 Linux 7.3 对 VRAM overcommit（显存过量分配）的改进，目标是在 GPU 显存耗尽时降低性能损失。文章本身的具体实现细节未随条目提供，但社区讨论认为这是显著改进，并期待其被上游合并；同时有评论指出 Nvidia 驱动目前不支持显存分页/换页，因此该改进可能暂时只惠及部分 GPU 用户。这项变化关系到 GPU 工作负载、内存管理和系统性能，尤其对显存受限场景有实际意义。需要说明的是，由于缺少源内容，具体机制、版本号和性能数据均无法核实。

hackernews · flaburgan · 8月18日 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49342719)

**「背景」** Linux 是一个开源操作系统内核，其内存管理子系统负责系统内存与显存（VRAM）等资源的分配和调度。显存超量分配（VRAM overcommit）指允许程序分配超过物理显存容量的显存空间，当显存不足时，内核如何处理换页与回收会直接影响性能。社区讨论还提到，不同显卡驱动（如 NVIDIA）对显存换页的支持程度不同，这会影响相关改进的实际效果。

**「影响」** 对显存容易耗尽的 Linux GPU 工作负载用户，这一改进有望在高显存占用时带来性能提升；但评论显示使用 Nvidia GPU 的用户可能无法立即受益，因为 Nvidia 当前不支持任何形式的显存分页。

**「社区讨论」** 社区整体持正面看法，认为文章写得清晰、改进令人期待，并赞赏内核开发者的投入；也有用户提出对系统内存耗尽时冻结问题的担忧，以及 Nvidia 不支持显存分页的例外情况，说明影响范围并非所有 GPU 用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Linux">Linux - Wikipedia</a></li>

</ul>
</details>

**标签**: `#linux`, `#kernel`, `#vram`, `#memory-management`, `#performance`

---

<a id="item-tech-news-3"></a>
### [Mojo 开源：Apache 2.0 发布编译器与工具链](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 8.0/10

Mojo 编程语言于 2026 年 8 月 18 日宣布开源，编译器与工具链以 Apache 2.0 许可证发布，距其 1.0 版本发布仅一周，也兑现了自 2023 年 5 月以来的开源承诺。Mojo 最初定位为 Python 的超集，但 2025 年 8 月的路线图已调整，承认它可能不会成为完整超集；如今它已成为一门独立的、语法受 Python 启发的语言，重点优化 GPU 编程体验。这一变化意味着开发者可以用类似 Python 的语法编写 GPU 代码，但现有 Python 代码并不保证 100% 兼容。开源的编译器与工具链为外部贡献、代码审计和更广泛生态建设提供了基础。

rss · Simon Willison · 8月18日 21:39

**「背景」** Mojo 由 Modular 公司开发，2023 年 5 月首次发布时宣称目标是成为 Python 的超集，以便利用现有 Python 代码和生态。2025 年 8 月，官方路线图改变，表示 Mojo 可能不会演变为完整 Python 超集，并认为 AI 辅助编码工具能帮助将 Python 迁移到 Mojo。

**「影响」** 对于使用或考虑采用 Mojo 的开发者，开源后可以在 Apache 2.0 许可证下自由使用、修改和分发编译器与工具链，并围绕这一面向 GPU 编程的新语言构建工具和生态；不过它与既有 Python 代码不保证兼容。

**标签**: `#mojo`, `#open-source`, `#programming-languages`, `#compiler`, `#ai`

---

<a id="item-tech-news-4"></a>
### [Turbovec：Rust 实现的 TurboQuant 向量搜索库](https://github.com/RyanCodrai/turbovec) ⭐️ 7.0/10

Turbovec 是一个用 Rust 编写的开源向量搜索库，实现了 Google 提出的 TurboQuant 量化技术，目标是在大规模文档索引中降低内存占用。项目资料显示，它声称仅用约 4GB 内存即可索引 1000 万篇文档，这对本地化、隐私优先的搜索场景具有吸引力。该库还受到效率对比的关注，但 TurboQuant 此前已由 Qdrant 等系统集成，因此 Turbovec 并非首创实现。当前项目仍处于早期阶段，社区希望补充更易读的 README，并期待 SQLite 绑定等后续能力。

hackernews · fittingopposite · 8月18日 18:07 · [社区讨论](https://news.ycombinator.com/item?id=49349898)

**「背景」** TurboQuant 是 Google Research 等机构在 2025 年提出的在线向量量化压缩方法，旨在大幅减小模型与向量索引的占用空间并保持近零精度损失，常被用于大语言模型推理、KV 缓存压缩和最近邻搜索。Turbovec 是该技术在 Rust 生态中的实现库，将 TurboQuant 应用于向量检索，其特点是不依赖数据集专属码本，并可通过 TQ+ 校准应对真实嵌入分布不理想的情况。这类量化方法为大规模或隐私优先的本地向量搜索提供了更高效的索引基础。

**「影响」** Turbovec 发布约三周后，据第三方博客统计已催生 14 个以上衍生仓库（如 pg\_turbovec 和基于 LangGraph 的 RAG 管道），并提供 Python 绑定，使 Rust 实现的 TurboQuant 向量索引能直接在常见开发流程中落地。

**「社区讨论」** 评论者既有肯定也有保留：有人称赞 4GB/1000 万文档的内存效率可能加速反向索引和开发调试流程，也有人认为既然 Qdrant 早已集成 TurboQuant，直接使用 Qdrant 更省事。另一些意见提到 FAISS 已不再是当前最优基线，并建议项目用更接近人类写作风格的 README 来促进采用，还有人询问能否编译为 WASM 在浏览器扩展中运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TurboQuant">TurboQuant - Wikipedia</a></li>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/turbovec-googles-turboquant-makes-vector-search-smaller-faster-and-simpler-fdea72674aad">turbovec : Google’s TurboQuant Makes Vector Search Smaller, Faster, and Simpler | by Mehul Gupta | Data Science in Your Pocket | Medium</a></li>
<li><a href="https://github.com/RyanCodrai/turbovec">GitHub - RyanCodrai/turbovec: A vector index built on TurboQuant, written in Rust with Python bindings · GitHub</a></li>
<li><a href="https://www.alphamatch.ai/blog/turbovec-rust-vector-index-rag-2026">TurboVec: The Rust-Powered Vector Index That&#x27;s Quietly Changing the RAG Game</a></li>

</ul>
</details>

**标签**: `#vector-search`, `#rust`, `#quantization`, `#machine-learning`, `#open-source`

---

<a id="item-tech-news-5"></a>
### [用 20 美元工具修复 Framework 13 的 BIOS 变砖](https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/) ⭐️ 7.0/10

一位用户在博客文章中记录了自己用约 20 美元的工具，修复了一台因 BIOS 更新而变砖的 Framework 13（AMD 7040 系列）笔记本。文章展示了这种“变砖”并非只能依赖官方售后或报废，借助低成本编程器和公开资料即可恢复。事件说明 BIOS 更新这类官方固件仍可能造成严重故障，同时也为 DIY 维修和“维修权”提供了现实案例。

hackernews · jp\_sc · 8月18日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=49345220)

**「背景」** Framework 13 笔记本的 AMD Ryzen 7040 系列通常通过官方 BIOS 更新来修复安全漏洞和提升稳定性，但用户反馈显示，部分 BIOS 更新或相关故障可能导致设备彻底无法启动，即“变砖”。例如，有用户在收到 Framework 13 7040 系列仅三天后就遇到无法充电、无法启动的问题。在此背景下，使用低成本工具（如 20 美元的编程器）进行固件恢复成为一种可行的维修途径。

**「影响」** 对于遭遇同类 BIOS 变砖的 Framework 13（AMD 7040 系列）用户，这一案例提供了一条可自行尝试的低成本恢复路径，降低了对官方售后的依赖。

**「社区讨论」** 评论中有人认为官方软件缺陷导致硬件变砖应承担法律责任，甚至应诉诸小额索赔；也有人分享 ThinkPad Nano 类似故障，并对厂商普遍不重视 BIOS 更新问题感到震惊。还有用户对 Framework 的部件市场表达顾虑，认为缺少竞争导致维修仍被原厂锁定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/">Fixing a bricked AMD 7040 series Framework 13 ” laptop with $20...</a></li>
<li><a href="https://community.frame.work/t/solved-framework-13-7040-series-bricked-after-using-it-for-3-days/65381">[Solved] - Framework 13 7040 series bricked after using it for 3 days</a></li>

</ul>
</details>

**标签**: `#hardware`, `#firmware`, `#laptop-repair`, `#BIOS`, `#Framework-laptop`

---

<a id="item-tech-news-6"></a>
### [摄像头版 AirPods B790 现身，macOS 26.7 演示视觉智能](https://www.macrumors.com/2026/08/17/camera-equipped-airpods-macos-26-7/) ⭐️ 7.0/10

苹果正在开发配备摄像头的 AirPods，产品代号为 B790。macOS Tahoe 26.7 RC 中的演示视频显示，这款 AirPods 的摄像头可识别书名，并通过视觉智能保存信息；Siri 还能回答佩戴者周边环境的问题并记录内容。Mark Gurman 称该产品最快可能在 9 月发布，但这一消息目前仍属传闻，尚未正式发布。若成真，这将是苹果首次把视觉智能从 iPhone 扩展到可穿戴设备。

telegram · zaihuapd · 8月18日 02:00

**「背景」** 苹果在 iPhone 16 系列中引入了视觉智能功能，用户可通过相机按钮识别物体、地点和文本。目前 AirPods 主要提供音频播放、通话和健康监测等功能，B790 则被视为 AirPods 向环境感知设备扩展的传闻产物。

**「影响」** 若如期发布，摄像头版 AirPods 将首次把视觉智能和 Siri 的环境问答引入可穿戴场景，让用户无需掏出手机即可获取周边信息。不过目前仍是传闻，发布时间和最终功能仍存在不确定性。

**标签**: `#Apple`, `#AirPods`, `#visual-intelligence`, `#hardware`, `#macOS`

---

<a id="item-tech-news-7"></a>
### [macOS 26.7 代码揭示中国大陆 Apple 智能写作工具审查机制](https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/) ⭐️ 7.0/10

据 MacRumors 报道，未发布的 macOS 26.7 等系统中的代码显示，Apple 智能的“写作工具”将登陆中国大陆，并内置专属的内容安全过滤机制。系统会先提示“需要进行内容安全更新”，自动更新完成后 iPhone 才能使用该工具；对于无法由 Apple 智能编辑的内容，系统将提示无法编辑，并建议将文本发送给其他应用处理。代码还显示，若用户多次触发安全警报，“写作工具”会暂时受限，相关安全审查规则可以通过云控远程下发。这表明中国大陆版 Apple 智能的写作功能具备独立的内容过滤、拦截和处罚机制，并可能随云端策略动态调整。

telegram · zaihuapd · 8月18日 02:16

**「背景」** Apple 智能是苹果在 macOS、iOS 中集成的 AI 功能套件，“写作工具”提供改写、校对和文本总结等能力。中国大陆对生成式内容有严格的合规要求，海外企业常需对输出进行审查或本地化调整。此次代码曝光表明苹果不是简单禁用该功能，而是为中国大陆版本构建一套可远程变更的独立审查体系。

**「影响」** 中国大陆用户使用“写作工具”时可能遇到内容无法编辑、安全更新弹窗以及多次触发安全警报后的临时限制；依赖该功能的应用开发与内容生产流程也需要考虑云控规则更新的不确定性。

**标签**: `#Apple`, `#AI censorship`, `#content moderation`, `#China`, `#Apple Intelligence`

---

<a id="item-tech-news-8"></a>
### [中国要求政府机构提前卸载定制版 Windows 10](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 7.0/10

中国国家安全部要求部分政府相关机构卸载定制版 Windows 10，使原定 2027 年 2 月的停用计划提前数月。指令源于数据安全担忧，但未说明具体漏洞。微软回应称，未发现影响该产品的安全事件，该产品仍在定期获得安全更新。此举显示中国正加速减少政府机构对微软系统的依赖，可能影响微软在中国的业务布局。

telegram · zaihuapd · 8月18日 06:22

**「背景」** 定制版 Windows 10 是微软面向中国政府相关机构提供的专用操作系统版本，原计划于 2027 年 2 月正式停用。此次国家安全部要求部分机构提前卸载该版本，是基于数据安全方面的担忧，但尚未说明具体漏洞；微软则表示未发现影响该产品的安全事件，且产品仍在定期获得安全更新。

**「影响」** 受影响机构需要立即寻找替代操作系统，可能推动国产系统的更快部署，并给微软在华政府业务带来不确定性。

**标签**: `#policy`, `#microsoft`, `#windows`, `#china`, `#security`

---

<a id="item-tech-news-9"></a>
### [国产 AI 芯片 2026 年将占中国近 90% 寒武纪华为受益](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-homegrown-ai-accelerators-to-supply-90-percent-of-the-countrys-domestic-market-analysts-suggest-cambricon-and-huawei-expected-to-be-the-biggest-winners-in-the-shift-away-from-nvidia-and-amd) ⭐️ 7.0/10

TrendForce 预计，到 2026 年中国本土 AI 加速器将占国内市场近 90%，较去年的 45% 大幅提升，寒武纪与华为被视为最大受益者。2025 年英伟达以 220 万颗出货量占据 55% 市场份额，华为出货 81.2 万颗、份额为 20.3%。报告指出，中国需要在一年内将高端 AI 芯片产量提升 2.2 倍至约 196 万颗，才能支撑这一市场转变，但产能能否跟上仍存疑。该预测基于分析师推算而非已确认事件，实际进展仍有不确定性。

telegram · zaihuapd · 8月18日 13:03

**「背景」** AI 加速器是专门用于训练和推理人工智能模型的芯片，目前市场主要由英伟达（NVIDIA）主导。受美国对华出口管制影响，中国厂商正加速转向国产芯片，华为升腾（Ascend）系列和寒武纪思元（MLU）系列是主要的替代方案。TrendForce 的预测基于这一趋势，反映国产 AI 芯片在中国市场占比的快速提升。

**「影响」** 对中国 AI 芯片采购方和国产供应链而言，国产替代加速将显著降低对英伟达和 AMD 的依赖，但能否兑现近 90% 的份额目标，取决于国内高端芯片产能是否能在一年内实现 2.2 倍增长。

**标签**: `#AI chips`, `#Huawei`, `#Cambricon`, `#semiconductors`, `#China tech`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [贵州茅台净利罕见下滑，折射中国经济与消费结构转变](https://www.cnbc.com/2026/08/19/china-economy-moutai-ai-property.html) ⭐️ 8.0/10

贵州茅台 8 月发布的上半年财报显示，净利润同比下滑 1.95%至 445 亿元人民币（约 66 亿美元），为 2014 年以来首次上半年净利下降；此前 2025 年全年净利已下降 4.5%，是有记录以来首次年度下滑。

rss · CNBC Finance · 8月18日 23:18

**「背景」** 该公司股票曾是 A 股“风向标”，2020 至 2023 年是内地市值最大的上市公司；作为政商宴请常用白酒，其需求与房地产繁荣密切相关。如今中国反腐趋严、房地产降温、经济转向人工智能等科技产业，酒类消费场景减少，分析师认为白酒市场已饱和。

**「影响」** 受此影响，资金年内多数时间从重仓白酒的食品饮料 ETF 净流出，部分科技股的市值已超过茅台，显示投资者正重新评估传统消费板块。

**标签**: `#China economy`, `#Kweichow Moutai`, `#earnings`, `#consumer staples`, `#market bellwether`

---

<a id="item-finance-news-2"></a>
### [债市压力挤压美国家庭：房贷与柴油成本上升](https://www.cnbc.com/2026/08/18/bond-market-treasury-yields-warsh-main-street.html) ⭐️ 8.0/10

美国国债市场近期抛售推高长期收益率，10 年期美债收益率周二超过 4.7%，推高 30 年期房贷利率至 6.75%；同时柴油价格同比上涨 48%，加重家庭用油负担。

rss · CNBC Finance · 8月18日 16:48

**「背景」** 此前美联储在新任主席凯文·沃什领导下维持利率不变，长期收益率上升反映市场对增长、通胀和财政赤字的担忧；美国国会预算办公室估计，截至 9 月的本财年赤字将达 2.1 万亿美元，约占 GDP 的 6.4%。

**「影响」** 房贷利率和柴油价格上涨将直接挤压依赖贷款购房和用油的家庭；与此同时，过去三年标普 500 指数累计回报 77%，但股票持有集中在最富有美国人手中，普通家庭从股市上涨中获益有限。

**标签**: `#Bond Market`, `#Treasury Yields`, `#Federal Reserve`, `#Mortgage Rates`, `#Fiscal Policy`

---

<a id="item-finance-news-3"></a>
### [汇丰要求部分内地投资客户提交资金来源声明，逾期或终止服务](https://36kr.com/newsflashes/3944605562797192) ⭐️ 7.0/10

汇丰香港要求部分内地存量投资客户在 9 月 12 日前通过 App 提交资金来源声明书，若 8 月 20 日前未提交，投资相关服务可能被暂停；若 9 月 12 日前仍未提交，服务可能被终止。汇丰称此举是遵循监管要求，仅适用于投资服务客户。

telegram · zaihuapd · 8月18日 07:30

**「背景」** 声明书属于“了解你的客户（KYC）”和客户尽职调查环节，需确认投资资金来自中国内地以外合法来源，并同意银行可应执法或监管机构要求披露个人资料。

**标签**: `#HSBC`, `#KYC`, `#Hong Kong`, `#cross-border investment`, `#financial regulation`

---

<a id="item-finance-news-4"></a>
### [苹果美国 App Store 佣金收入降 18%，二季度用户消费额同比下降 6%](https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/) ⭐️ 7.0/10

第三方数据机构 Appfigures 和 Sensor Tower 显示，苹果美国 App Store 佣金收入自 2026 年初以来下降 18%，美国用户第二季度 App Store 消费额同比减少 6%（去年同期为增长 9%）；苹果称监管变化已拖累服务业务增长。

telegram · zaihuapd · 8月18日 12:17

**「背景」** 苹果在最近的财报电话会议中表示，监管变化已开始拖累其服务业务增长；巴西和日本也在实施新规后出现 App Store 收入下滑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vuink.com/post/znpehzbef-d-dpbz/2026/08/18/apple-app-store-revenue-falling">Apple &#x27;s US App Store Commission Revenue Down 18... | Vuink.com</a></li>

</ul>
</details>

**标签**: `#Apple`, `#App Store`, `#regulation`, `#services revenue`, `#app economy`

---