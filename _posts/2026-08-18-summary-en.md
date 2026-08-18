---
layout: default
title: "Horizon Summary: 2026-08-18 (EN)"
date: 2026-08-18
lang: en
---

> From 38 items, 13 important content pieces were selected

---

**Technology News**
1. [Qwen 3.8 27B Matches GPT-5.6 Luna on AI Index](#item-tech-news-1) ⭐️ 9.0/10
2. [Linux 7.3 Improves Performance When GPU VRAM Is Exhausted](#item-tech-news-2) ⭐️ 8.0/10
3. [Mojo programming language is now open source](#item-tech-news-3) ⭐️ 8.0/10
4. [Turbovec brings Google&\#x27;s TurboQuant vector search to Rust](#item-tech-news-4) ⭐️ 7.0/10
5. [Bricked Framework Laptop Fixed with $20 Tools](#item-tech-news-5) ⭐️ 7.0/10
6. [Camera-Equipped AirPods B790 Appear in macOS Tahoe Demo](#item-tech-news-6) ⭐️ 7.0/10
7. [Apple Code Reveals China AI Writing Tool Content Moderation](#item-tech-news-7) ⭐️ 7.0/10
8. [China Orders Some Agencies to Uninstall Custom Windows 10 Months Early](#item-tech-news-8) ⭐️ 7.0/10
9. [China Homegrown AI Accelerators Forecast to Supply Nearly 90% of Domestic Market by 2026](#item-tech-news-9) ⭐️ 7.0/10

**Financial News**
1. [Kweichow Moutai posts rare first-half profit drop as China&\#x27;s economy shifts](#item-finance-news-1) ⭐️ 8.0/10
2. [Bond sell-off pushes 10-year yield above 4.7% as mortgage and diesel costs rise](#item-finance-news-2) ⭐️ 8.0/10
3. [HSBC sets fund-source declaration deadlines for some mainland China investment clients](#item-finance-news-3) ⭐️ 7.0/10
4. [Apple&\#x27;s U.S. App Store Commission Revenue Down 18%; Q2 2026 User Spending Falls 6%](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen 3.8 27B Matches GPT-5.6 Luna on AI Index](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 9.0/10

Qwen 3.8 27B scores 52 on the Artificial Analysis Intelligence Index, the same score as GPT-5.6 Luna \(max\) and just one point behind GLM-5.2 \(max\) and DeepSeek V4 Pro 0813 \(max\). The GLM model has 753B parameters and the DeepSeek model has 1.7T parameters, while Luna&\#x27;s size is unknown but presumably much larger than 27B. This means a relatively small 27B model matches the index score of much larger frontier models, marking a significant milestone in model efficiency. Simon Willison describes Qwen 3.8 27B as a truly astonishing model.

rss · Simon Willison · Aug 17, 23:58

**「Background」** The Artificial Analysis Intelligence Index is a standardized benchmark that scores large language models across a range of tasks to compare their overall capability. Qwen is an open-weight model family developed by Alibaba, and Qwen 3.8 27B is a relatively small 27-billion-parameter model that supports text and image input with a 256k token context window. Scoring 52 on this index means it matches or nearly matches frontier models that are far larger, which is notable because smaller models typically score much lower in such evaluations.

**「Impact」** For AI practitioners, a 27B model matching the index score of models with hundreds of billions or over a trillion parameters suggests that competitive performance may no longer require enormous model sizes, potentially making such capabilities more accessible to run, fine-tune, and deploy.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/qwen3-8-27b">Qwen3.8 27B Intelligence , Performance &amp; Price Analysis</a></li>

</ul>
</details>

**Tags**: `#ai`, `#llms`, `#qwen`, `#benchmarks`, `#model-efficiency`

---

<a id="item-tech-news-2"></a>
### [Linux 7.3 Improves Performance When GPU VRAM Is Exhausted](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

An article on PixelCluster describes how Linux kernel 7.3 improves performance when GPU memory \(VRAM\) is exhausted, building on the performance and gaming enhancements already introduced in 7.2. The key change appears to involve VRAM overcommit handling, reducing the performance hit when a workload exceeds available video memory. The improvements are not yet upstreamed, and the article suggests that applications themselves are best positioned to inform the kernel about memory stickiness to VRAM. Community reaction is enthusiastic, though Nvidia users note that vendor support for VRAM paging remains limited.

hackernews · flaburgan · Aug 18, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49342719)

**「Background」** Linux is a widely used open-source kernel developed collaboratively by many contributors, responsible for core system tasks such as memory management. VRAM \(video RAM\) is the dedicated memory on a GPU; when it is exhausted, the kernel may store GPU data in ordinary system RAM, an approach sometimes called VRAM overcommit. This item describes improvements in the Linux 7.3 kernel line that aim to make that fallback faster and reduce performance problems under memory pressure.

**「Impact」** GPU-heavy workloads on Linux that exceed VRAM capacity could see significantly better performance once the 7.3 improvements reach stable releases. Nvidia GPU users may not benefit immediately, as their driver stack reportedly lacks similar paging support.

**「Community Discussion」** Commenters widely praised the article and the kernel work, with several expressing eagerness for 7.3 after 7.2&\#x27;s performance gains. Some raised concerns that Nvidia GPUs do not support comparable paging, and one hoped for a fix to system freezes when system RAM itself fills up.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Linux">Linux - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#linux`, `#kernel`, `#vram`, `#memory-management`, `#performance`

---

<a id="item-tech-news-3"></a>
### [Mojo programming language is now open source](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 8.0/10

Mojo&\#x27;s compiler and toolchain are now open source under an Apache 2 license, fulfilling a promise made when the language launched in May 2023 and following last week&\#x27;s 1.0 release. The language, created by Modular, is no longer committed to becoming a full Python superset, a vision revised around August 2025. It now positions itself as its own Python-inspired language aimed at making GPU programming easier, with AI-assisted migration tools expected to help translate Python code. The open source release gives developers access to the underlying implementation and tooling.

rss · Simon Willison · Aug 18, 21:39

**「Background」** Mojo is a programming language developed by Modular, initially announced as a potential superset of Python to bootstrap an ecosystem while adding high-performance GPU capabilities. The original May 2023 announcement promised an eventual open source release, and the project revised its compatibility goal in August 2025.

**「Impact」** Developers can now inspect, modify, and build on Mojo&\#x27;s compiler and toolchain under a permissive Apache 2 license, potentially accelerating adoption and third-party tooling for GPU-focused Python-style programming.

**Tags**: `#mojo`, `#open-source`, `#programming-languages`, `#compiler`, `#ai`

---

<a id="item-tech-news-4"></a>
### [Turbovec brings Google&\#x27;s TurboQuant vector search to Rust](https://github.com/RyanCodrai/turbovec) ⭐️ 7.0/10

Turbovec is an open-source Rust library that implements Google&\#x27;s TurboQuant quantization technique for efficient vector search, targeting large-scale document indexing with a reported memory footprint of about 4GB for 10 million documents. The project aims to make high-performance, memory-efficient vector retrieval more accessible to Rust developers, potentially enabling faster reverse-index construction and smoother local development and debugging workflows. Since TurboQuant has already been integrated into systems like Qdrant, Turbovec&\#x27;s value lies in offering a Rust-native alternative rather than introducing a fundamentally new technique. Detailed validation and benchmarks are not yet available in the provided context, and the project is still evolving with community interest in features like SQLite bindings and WebAssembly support.

hackernews · fittingopposite · Aug 18, 18:07 · [Discussion](https://news.ycombinator.com/item?id=49349898)

**「Background」** Vector search stores high-dimensional embeddings, and quantization compresses those vectors \(for example, from float32 to compact integer codes\) to cut memory and speed up nearest-neighbor lookup while ideally preserving accuracy. TurboQuant is a 2025 compression method from Google Research \(Zandieh, Mirrokni, Daliri, Hadian\) designed for LLM inference, KV-cache compression, vector databases, and nearest-neighbor search; Google describes it as delivering extreme compression with near-zero accuracy loss. Turbovec is a Rust library that applies TurboQuant to vector indexing, using a codebook-free approach with an optional TQ+ calibration step for real-world embeddings.

**「Impact」** Developers building local, privacy-first vector search in Rust gain a TurboQuant-based index with Python bindings, and the ecosystem is already producing Postgres extensions \(pg\_turbovec\) and LangGraph-based RAG pipelines, extending the library&\#x27;s practical reach beyond a standalone index.

**「Community Discussion」** Commenters were enthusiastic about the 4GB-for-10M-documents claim, noting it could accelerate reverse indexing and improve development workflows, with some eagerly awaiting SQLite bindings and asking whether the Rust code can compile to WebAssembly for browser-based privacy-focused search. Others advised making the README more human-friendly, pointed out that established systems like Qdrant already integrate TurboQuant, and shared benchmark references suggesting FAISS is no longer state-of-the-art.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TurboQuant">TurboQuant - Wikipedia</a></li>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>
<li><a href="https://medium.com/data-science-in-your-pocket/turbovec-googles-turboquant-makes-vector-search-smaller-faster-and-simpler-fdea72674aad">turbovec : Google’s TurboQuant Makes Vector Search Smaller, Faster, and Simpler | by Mehul Gupta | Data Science in Your Pocket | Medium</a></li>
<li><a href="https://github.com/RyanCodrai/turbovec">GitHub - RyanCodrai/turbovec: A vector index built on TurboQuant, written in Rust with Python bindings · GitHub</a></li>
<li><a href="https://www.alphamatch.ai/blog/turbovec-rust-vector-index-rag-2026">TurboVec: The Rust-Powered Vector Index That&#x27;s Quietly Changing the RAG Game</a></li>

</ul>
</details>

**Tags**: `#vector-search`, `#rust`, `#quantization`, `#machine-learning`, `#open-source`

---

<a id="item-tech-news-5"></a>
### [Bricked Framework Laptop Fixed with $20 Tools](https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/) ⭐️ 7.0/10

A hands-on account describes recovering a Framework 13 laptop with an AMD 7040-series processor that was bricked by a BIOS update, using roughly $20 worth of tools. The episode highlights how firmware update failures can disable otherwise functional hardware and shows that low-cost flashing and recovery equipment can revive such devices. It also raises broader questions about firmware reliability and right-to-repair, since BIOS-update bricks remain common across laptop brands. The author documents the practical repair steps and argues that manufacturers should make recovery paths more accessible.

hackernews · jp\_sc · Aug 18, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49345220)

**「Background」** Framework&\#x27;s AMD Ryzen 7040 series Framework Laptop 13 received a BIOS update that the company recommends installing for security, stability, and performance. However, BIOS updates can fail or be faulty, and users have reported fully bricked units that refuse to charge or boot after the update. The article describes recovering such a bricked laptop using low-cost hardware tools, highlighting that repair may be possible without manufacturer support.

**「Impact」** Owners of BIOS-bricked laptops, especially Framework 13 AMD 7040 models, gain a concrete low-cost recovery option that may avoid expensive repairs or premature e-waste.

**「Community discussion」** Commenters debated responsibility for BIOS-update bricking: one suggested small-claims action against Framework for supplying faulty firmware, while another recounted a similar ThinkPad Nano failure and found manufacturers largely indifferent. Others expressed frustration that official updates can worsen devices and that Framework&\#x27;s proprietary parts create lock-in and stock shortages.

<details><summary>References</summary>
<ul>
<li><a href="https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/">Fixing a bricked AMD 7040 series Framework 13 ” laptop with $20...</a></li>
<li><a href="https://community.frame.work/t/solved-framework-13-7040-series-bricked-after-using-it-for-3-days/65381">[Solved] - Framework 13 7040 series bricked after using it for 3 days</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#firmware`, `#laptop-repair`, `#BIOS`, `#Framework-laptop`

---

<a id="item-tech-news-6"></a>
### [Camera-Equipped AirPods B790 Appear in macOS Tahoe Demo](https://www.macrumors.com/2026/08/17/camera-equipped-airpods-macos-26-7/) ⭐️ 7.0/10

Apple&\#x27;s camera-equipped AirPods, carrying product code B790, have surfaced in a macOS Tahoe 26.7 Release Candidate demo, showing visual intelligence features such as recognizing book titles and saving the information, with Siri able to answer questions about the wearer&\#x27;s surroundings and record details. According to Mark Gurman, the devices could launch as soon as September. While the demonstration is concrete, the product remains unannounced and is still considered a rumor.

telegram · zaihuapd · Aug 18, 02:00

**「Background」** Apple has reportedly been developing AirPods with integrated cameras to expand its visual intelligence capabilities, similar to the on-device scene understanding found in recent iPhones. macOS Tahoe is Apple&\#x27;s next-generation desktop operating system, and a Release Candidate is the near-final build distributed for testing before public release.

**「Impact」** If released as reported, the camera-equipped AirPods would introduce a new wearable form factor for Apple&\#x27;s visual intelligence features, potentially changing how users interact with Siri and gather information from their environment. However, because the product is unconfirmed and no official specifications or pricing have been provided, the practical impact remains uncertain.

**Tags**: `#Apple`, `#AirPods`, `#visual-intelligence`, `#hardware`, `#macOS`

---

<a id="item-tech-news-7"></a>
### [Apple Code Reveals China AI Writing Tool Content Moderation](https://www.macrumors.com/2026/08/17/macos-26-7-unreleased-apple-devices/) ⭐️ 7.0/10

Code references in an unreleased macOS 26.7 build, reported by MacRumors, indicate that Apple is preparing to bring its &\#x27;Writing Tools&\#x27; features to mainland China with built-in content moderation. The code mentions automatic safety-content updates, messages for texts that cannot be edited, and temporary restrictions if security alerts are triggered repeatedly. These findings suggest that Apple Intelligence&\#x27;s writing features in mainland China may include independent content safety filtering, interception, and punishment mechanisms, with review rules that can be remotely configured. This matters because it reveals how Apple is adapting its AI writing tools to comply with China&\#x27;s content regulations.

telegram · zaihuapd · Aug 18, 02:16

**「Background」** Apple Intelligence is Apple&\#x27;s platform for AI-powered features, including Writing Tools that help users rewrite, summarize, and proofread text. Mainland China requires internet services to filter content that violates local regulations, so any AI writing tool offered there would need built-in compliance measures. The newly exposed code hints at how Apple may implement such requirements for its Chinese version of Apple Intelligence.

**「Impact」** For users in mainland China, the code suggests that Apple&\#x27;s Writing Tools, when available, will include mandatory content filtering and could be temporarily disabled after repeated security alerts, with rules updated remotely.

**Tags**: `#Apple`, `#AI censorship`, `#content moderation`, `#China`, `#Apple Intelligence`

---

<a id="item-tech-news-8"></a>
### [China Orders Some Agencies to Uninstall Custom Windows 10 Months Early](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 7.0/10

Bloomberg reports that China&\#x27;s Ministry of State Security has told some state-affiliated agencies to uninstall a customized Windows 10 build, moving the previously planned retirement forward from February 2027 by several months. The directive is said to stem from data security concerns, although no specific vulnerability was identified. Microsoft responded that it has not found a security incident affecting the product and that the customized version continues to receive regular security updates. The exact agencies, scope, and technical rationale remain undisclosed.

telegram · zaihuapd · Aug 18, 06:22

**「Background」** Chinese state agencies affected by this directive use a customized version of Microsoft Windows 10 developed with China&\#x27;s Ministry of State Security. The original plan called for decommissioning this version by February 2027, but the new directive requires removal months ahead of that schedule. The reported reason is data security concerns, though no specific vulnerability has been identified.

**「Impact」** Affected government agencies must accelerate migration off the customized Windows 10 months before the original February 2027 deadline, with Microsoft disputing any security incident linked to the product.

**Tags**: `#policy`, `#microsoft`, `#windows`, `#china`, `#security`

---

<a id="item-tech-news-9"></a>
### [China Homegrown AI Accelerators Forecast to Supply Nearly 90% of Domestic Market by 2026](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-homegrown-ai-accelerators-to-supply-90-percent-of-the-countrys-domestic-market-analysts-suggest-cambricon-and-huawei-expected-to-be-the-biggest-winners-in-the-shift-away-from-nvidia-and-amd) ⭐️ 7.0/10

TrendForce projects that Chinese domestic AI accelerators will supply nearly 90% of China&\#x27;s market by 2026, up sharply from 45% last year, making Cambricon and Huawei the biggest beneficiaries. In 2025, Nvidia shipped 2.2 million accelerators for a 55% share, while Huawei shipped 812,000 units for a 20.3% share. The forecast implies that China must boost high-end AI chip production by 2.2 times to roughly 1.96 million units within a year, and analysts express doubt about whether capacity can keep pace. This shift away from Nvidia and AMD reflects tightening export controls and accelerating domestic substitution in China&\#x27;s AI hardware market.

telegram · zaihuapd · Aug 18, 13:03

**「Background」** China&\#x27;s AI accelerator market has historically relied on imported chips from NVIDIA and AMD, but domestic firms like Cambricon and Huawei have been developing their own accelerators to reduce dependence. TrendForce&\#x27;s projection reflects a broader push for self-sufficiency amid export controls and supply concerns.

**「Impact」** Chinese cloud vendors, AI developers, and chip buyers will face accelerating dependence on Cambricon and Huawei accelerators, while near-term supply remains uncertain given the required 2.2x production increase and capacity constraints.

**Tags**: `#AI chips`, `#Huawei`, `#Cambricon`, `#semiconductors`, `#China tech`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Kweichow Moutai posts rare first-half profit drop as China&\#x27;s economy shifts](https://www.cnbc.com/2026/08/19/china-economy-moutai-ai-property.html) ⭐️ 8.0/10

Kweichow Moutai reported a 1.95% drop in first-half net profit to 44.5 billion yuan \($6.6 billion\), its first decline for the January-June period since 2014, after a 4.5% fall in full-year 2025 net profit — its first annual decline on record.

rss · CNBC Finance · Aug 18, 23:18

**「Background」** Moutai makes baijiu, a strong Chinese liquor that was long a staple at government and business banquets, making its stock a market bellwether; but China&\#x27;s anti-corruption crackdown, real-estate slowdown, and transition to high-tech industries have dampened demand for premium baijiu.

**「Impact」** Investors have felt the shift: Moutai shares have fallen for four straight years, state funds Central Huijin and China Securities Finance no longer rank among its top 10 shareholders, and baijiu-heavy food and beverage ETFs have seen net outflows for much of this year.

**Tags**: `#China economy`, `#Kweichow Moutai`, `#earnings`, `#consumer staples`, `#market bellwether`

---

<a id="item-finance-news-2"></a>
### [Bond sell-off pushes 10-year yield above 4.7% as mortgage and diesel costs rise](https://www.cnbc.com/2026/08/18/bond-market-treasury-yields-warsh-main-street.html) ⭐️ 8.0/10

A bond market sell-off has pushed the 10-year Treasury yield above 4.7%, lifting a typical 30-year mortgage rate to 6.75% and squeezing households facing diesel prices that are up 48% from a year ago. Analysts quoted in the article say heavy U.S. budget deficits leave the economy vulnerable to shocks.

rss · CNBC Finance · Aug 18, 16:48

**「Background」** Long-term Treasury yields are driven by growth and inflation expectations and influence mortgage and other consumer borrowing costs; the U.S. deficit is estimated at about 6.4% of GDP for the fiscal year, while the Federal Reserve under new Chairman Kevin Warsh has kept rates steady.

**「Impact」** Home buyers and consumers facing higher mortgage and fuel costs are the direct losers, and the article concludes the squeeze is likely to persist unless fiscal policy or Fed policy changes.

**Tags**: `#Bond Market`, `#Treasury Yields`, `#Federal Reserve`, `#Mortgage Rates`, `#Fiscal Policy`

---

<a id="item-finance-news-3"></a>
### [HSBC sets fund-source declaration deadlines for some mainland China investment clients](https://36kr.com/newsflashes/3944605562797192) ⭐️ 7.0/10

HSBC Hong Kong is asking some mainland China investment clients to submit a source-of-funds declaration by Sept. 12; the bank warns that missing an earlier Aug. 20 deadline could suspend investment services and missing the final deadline could terminate them.

telegram · zaihuapd · Aug 18, 07:30

**「Background」** The declaration asks clients to confirm that their investment funds come from legal sources outside mainland China and to update their contact information; HSBC says it is following regulatory requirements and the request applies only to investment-service clients.

**Tags**: `#HSBC`, `#KYC`, `#Hong Kong`, `#cross-border investment`, `#financial regulation`

---

<a id="item-finance-news-4"></a>
### [Apple&\#x27;s U.S. App Store Commission Revenue Down 18%; Q2 2026 User Spending Falls 6%](https://www.macrumors.com/2026/08/18/apple-app-store-revenue-falling/) ⭐️ 7.0/10

According to market trackers Appfigures and Sensor Tower, Apple&\#x27;s U.S. App Store commission revenue fell 18% since early 2026, and U.S. user spending on the App Store fell 6% in the second quarter of 2026 year over year, after growing 9% a year earlier. Apple said regulatory changes have dragged on the growth of its services business.

telegram · zaihuapd · Aug 18, 12:17

**「Background」** Regulatory changes in the U.S., Brazil, and Japan—such as new rules affecting app store payments—have led to declines in Apple’s App Store commission revenue and consumer spending; Apple acknowledged on its latest earnings call that these changes have started to weigh on its Services growth.

**「Impact」** App developers selling through Apple&\#x27;s U.S. App Store are directly affected, as the drop in consumer spending and commissions reflects weaker App Store revenue from U.S. users following regulatory changes.

<details><summary>References</summary>
<ul>
<li><a href="https://vuink.com/post/znpehzbef-d-dpbz/2026/08/18/apple-app-store-revenue-falling">Apple &#x27;s US App Store Commission Revenue Down 18... | Vuink.com</a></li>
<li><a href="https://bingx.com/ur/news/post/apple-s-us-app-store-commission-revenue-down-this-year">Apple ’s U . S . App Store commission revenue falls 18% since the...</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#App Store`, `#regulation`, `#services revenue`, `#app economy`

---