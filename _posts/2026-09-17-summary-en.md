---
layout: default
title: "Horizon Summary: 2026-09-17 (EN)"
date: 2026-09-17
lang: en
---

> From 41 items, 8 important content pieces were selected

---

**Technology News**
1. [Nvidia launches official CUDA Rust support with two kernel tracks](#item-tech-news-1) ⭐️ 7.0/10
2. [Hackers Got Inside a Flock Camera](#item-tech-news-2) ⭐️ 7.0/10
3. [TMLR probe finds most desk-rejected authors could not explain papers](#item-tech-news-3) ⭐️ 7.0/10
4. [GoBench evaluates LLMs on 9x9 Go against KataGo opponents](#item-tech-news-4) ⭐️ 7.0/10
5. [Micron claims first 512 GB DDR5 RDIMM, targets 2027 production](#item-tech-news-5) ⭐️ 7.0/10

**Financial News**
1. [Fed Raises Rates a Quarter Point, Signals More Hikes Likely](#item-finance-news-1) ⭐️ 9.0/10
2. [Hong Kong Unveils 11 Measures to Encourage Childbirth](#item-finance-news-2) ⭐️ 7.0/10
3. [Pinglu Canal opens, giving southwest China a new water route to ASEAN](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Nvidia launches official CUDA Rust support with two kernel tracks](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/) ⭐️ 7.0/10

Nvidia announced official CUDA Rust support, offering two tracks for writing GPU kernels in Rust. The move gives Rust developers a vendor-backed path to author CUDA kernels, which matters for systems programming and GPU-accelerated AI/ML work that has largely relied on CUDA C++. Because the evidence is a vendor blog post with a promotional tone and earlier Rust-on-GPU efforts already existed, the change appears meaningful but incremental rather than a complete break from the status quo. Specific technical details, limitations, and compatibility constraints are not available in the supplied source content.

hackernews · nonmaskable · Sep 16, 11:15 · [Discussion](https://news.ycombinator.com/item?id=49724881)

**「Background」** CUDA is NVIDIA&\#x27;s proprietary GPU computing platform, and its mature enterprise toolchains have historically centered on CUDA C++ and CUDA Python. In September 2026, NVIDIA announced it was moving native Rust GPU programming from a community experiment into an official CUDA track, with two experimental routes: cuda-oxide for SIMT kernels and cutile-rs for tile-based execution. NVIDIA said it plans to grow and mature CUDA Rust into 2027 and beyond.

**「Impact」** Rust developers targeting Nvidia hardware gain an officially supported path to author CUDA kernels in Rust, which may reduce the need to drop into CUDA C++ for GPU work. Teams that value portability can still choose existing cross-platform Rust GPU approaches such as wgpu, cust, or direct OpenCL/PTX targeting to avoid single-vendor lock-in \[tool-2-1\]\[tool-2-2\]; because the announcement is a vendor blog post, the maturity, performance, and long-term support of the official Rust track remain unverified.

**「Community Discussion」** Hacker News commenters were split: some welcomed Rust&\#x27;s safety guarantees for kernel programming and called CUDA C++ a pain, while others warned that adopting CUDA deepens vendor lock-in and complicates portability. Discussion also questioned the article&\#x27;s provenance, with one commenter saying the launch text was &quot;checked rather than trusted&quot; and appeared fully Claude-written, and another saying the newness of Rust CUDA support revived their interest because LLMs have not yet been trained on it.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/">Introducing CUDA Rust: Two Tracks for Writing GPU Kernels</a></li>
<li><a href="https://andresseo.expert/ai/cuda-rust-is-official-nvidia-ships-two-compiler-tracks-for-safe-gpu-kernels/">CUDA Rust: NVIDIA&#x27;s Two Compiler Tracks for Safe GPU Kernels</a></li>
<li><a href="https://medium.com/@theopinionatedev/the-day-i-ditched-cuda-for-rust-gpu-kernels-7d2c2bf48667">The Day I Ditched CUDA for Rust GPU Kernels | Medium</a></li>
<li><a href="https://arxiv.org/pdf/2608.13759">GPU Offload in Rust : Portable, Safe, and Fast</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#CUDA`, `#GPU programming`, `#Nvidia`, `#developer tooling`

---

<a id="item-tech-news-2"></a>
### [Hackers Got Inside a Flock Camera](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/) ⭐️ 7.0/10

A Wired report, discussed on Hacker News, describes hackers gaining access to a Flock surveillance camera by exploiting security flaws that included hardcoded credentials. Commenters identified a hardcoded API key that can be used to request credentials stored in plaintext, which they said appeared to grant access to Flock&\#x27;s servers; the article body itself is not included in the supplied material. The reporting was done in collaboration with 404media, and Distributed Denial of Secrets published partition images from the camera. Community members also criticized Flock&\#x27;s vulnerability disclosure policy, saying it excludes cases involving interaction with the device or downloading its data, and noted that the camera&\#x27;s data was not suitably encrypted for a device deployed in public spaces.

hackernews · driverdan · Sep 16, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49726586)

**「Background」** Flock Safety is a privately held American manufacturer and operator of surveillance hardware and software, particularly automated license plate recognition \(ALPR\) cameras, mass video surveillance, and gunfire-location systems. Its network has been described as comprising more than 80,000 ALPR cameras and functioning as a de facto national surveillance grid, which is why security flaws in its devices can have broad implications. The reported Flock camera vulnerabilities involve a hard-coded API key that appears usable to obtain credentials for cameras by MAC address, with the API returning Auth0 client IDs and secrets; those credentials were reportedly stored in plaintext.

**「Impact」** Organizations using Flock cameras may need to review credential handling, physical-access threat models, and disclosure practices, since the reported flaws could expose sensitive data to anyone with local access to the device.

**「Community Discussion」** Hacker News commenters broadly agreed that hardcoded credentials and plaintext storage indicate poor security engineering, with one calling it a sign of total incompetence and another attributing it to reduced time to market. They also singled out Flock&\#x27;s vulnerability disclosure policy as performative, noted the 404media collaboration and DDoS partition-image release, and stressed that public-facing devices must account for local physical access.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://micahflee.com/flock-cameras-are-riddled-with-security-vulnerabilities-and-hard-coded-credentials/">Flock cameras are riddled with security vulnerabilities and...</a></li>
<li><a href="https://banthecams.org/posts/2025/12/09/flock-safety-surveillance-network-security-risks/">Vulnerability Assessment and Intelligence Estimate of the Flock ...</a></li>

</ul>
</details>

**Tags**: `#security-vulnerabilities`, `#iot-security`, `#surveillance-technology`, `#vulnerability-disclosure`, `#hardcoded-credentials`

---

<a id="item-tech-news-3"></a>
### [TMLR probe finds most desk-rejected authors could not explain papers](https://www.reddit.com/r/MachineLearning/comments/1wid67h/tmlr_reached_out_to_the_authors_of_10_papers/) ⭐️ 7.0/10

TMLR reached out to the authors of 10 papers slated for desk rejection to see whether they could explain their submissions, according to a Medium post by TmlrOrg summarized on r/MachineLearning. Of the ten submissions, one author withdrew, one said they were unavailable due to other commitments, and one scheduled a meeting but did not attend. Three authors were unable to answer basic questions about their papers, while three could discuss high-level ideas but struggled with technical details. Only one author answered all questions, though the interviewer, a TMLR Co-EiC, identified a major flaw in that paper. The results raise concerns about research integrity and authorship accountability in machine learning publishing.

reddit · r/MachineLearning · /u/hihey54 · Sep 16, 23:20

**「Background」** TMLR \(Transactions on Machine Learning Research\) is a machine learning journal that, according to TMLR, has faced a surge of submissions that outpaced available reviewer capacity, leading it to adopt stricter desk-rejection policies. Desk rejection means a submission is rejected by an editor before full peer review, often to filter out papers that do not meet basic scope, quality, or procedural expectations. In this case, TMLR Co-EiC Nihar Shah contacted authors of 10 papers slated for desk rejection to ask whether they could answer questions about their own submissions.

**「Impact」** For TMLR and the broader ML publishing community, the findings provide a concrete, small-sample signal that authors of some desk-rejected submissions could not explain their own work, raising concerns about authorship and submission integrity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/transactions-on-machine-learning-research-tmlr_asking-authors-about-their-own-papers-activity-7506087797871697920-HbWc">Asking Authors About Their Own Papers | Transactions on ...</a></li>
<li><a href="https://x.com/tmlrorg/status/2100322125491966241">Transactions on Machine Learning Research on X: &quot;TMLR has ...</a></li>

</ul>
</details>

**Tags**: `#ML research integrity`, `#peer review`, `#TMLR`, `#academic publishing`, `#desk rejection`

---

<a id="item-tech-news-4"></a>
### [GoBench evaluates LLMs on 9x9 Go against KataGo opponents](https://www.reddit.com/r/MachineLearning/comments/1wi68jg/gobench_evaluating_llms_on_the_game_of_go_r/) ⭐️ 7.0/10

A new benchmark called GoBench evaluates large language models on 9x9 Go games against a ladder of KataGo opponents ranging from random play to superhuman strength. Its author reports that GoBench scores correlate strongly with ARC-AGI 2 results \(r=0.83\) and that the leaderboard remains highly unsaturated. According to the post, GPT-6 Astra reaches a maximum of 2500 Elo, far below the best KataGo at 4400 Elo, while Codex with Astra reaches 3560 Elo when given coding tools and two hours of preparation before evaluation. The author states the leaderboard will be kept updated as long as it is not saturated, and links to the leaderboard, code repository, and paper. These figures and the claimed correlation come from a Reddit post and have not been independently verified here.

reddit · r/MachineLearning · /u/Roland31415 · Sep 16, 18:54

**「Background」** Go is a two-player board game, and the 9x9 board is a smaller variant often used when evaluating AI systems because games are short enough for repeated trials while still requiring strategic reasoning. KataGo is a Go engine that serves as the opponent ladder in this benchmark, ranging from random to superhuman strength, and Elo ratings provide a relative skill scale for comparing LLMs against those opponents. ARC-AGI-2, also referred to as ARC-AGI v2, is a benchmark for reasoning, spatial reasoning, and vision tasks, typically scored on a 0–1 scale, which helps explain why a Go benchmark&\#x27;s correlation with it is treated as evidence of general reasoning ability.

**「Impact」** If the reported correlation holds, LLM evaluation and reasoning-benchmark developers gain another unsaturated 9x9 Go test that appears to track ARC-AGI 2 performance, though the Elo numbers and r=0.83 correlation rest on the author&\#x27;s unverified claims.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-stats.com/benchmarks/arc-agi-v2">ARC-AGI v2 Leaderboard - llm-stats.com</a></li>

</ul>
</details>

**Tags**: `#LLM evaluation`, `#Go`, `#benchmark`, `#AI reasoning`, `#KataGo`

---

<a id="item-tech-news-5"></a>
### [Micron claims first 512 GB DDR5 RDIMM, targets 2027 production](https://videocardz.com/newz/micron-says-worlds-first-512gb-ddr5-module-will-be-production-ready-for-2027) ⭐️ 7.0/10

Micron says it has shown the world&\#x27;s first 512 GB DDR5 RDIMM for servers, with speeds up to 9200 MT/s. The module uses 3D stacked DRAM chips, and Micron says 24 of them can form 12 TB of memory. Micron says a single module consumes 16 W, compared with 44.2 W for four 128 GB modules, a reduction of more than 60%. AMD and Intel are validating the memory for future server platforms, with production-ready status expected in 2027. The claims have not been independently verified in the supplied source.

telegram · zaihuapd · Sep 16, 16:15

**「Background」** RDIMMs \(registered DIMMs\) are the buffered memory modules used in servers, and their capacity has conventionally grown by increasing DRAM die density and rank count rather than by stacking. Micron reaches 512 GB here by vertically stacking DRAM dies inside each package and connecting them with through-silicon vias \(TSVs\), the same die-stacking approach used in HBM, which is normally associated with bandwidth rather than standard DIMM capacity. Because new memory modules must be validated by platform vendors, AMD and Intel are evaluating this one for future server platforms, with volume production targeted for the second half of 2027.

**「Impact」** If validated, the module could allow future AMD and Intel server platforms to reach 12 TB of memory with 24 modules while cutting memory power by more than 60%, but production is not expected until 2027 and Micron&\#x27;s claims remain unverified.

<details><summary>References</summary>
<ul>
<li><a href="https://www.storagereview.com/news/micron-shows-a-512gb-ddr5-rdimm-12tb-per-dual-socket-server-at-9200-mt-s-volume-production-in-2h-2027">Micron Shows off 512GB DDR5 RDIMM: 12TB per Dual-Socket Server at 9,200 MT/s, Volume Production in 2H 2027 - StorageReview.com</a></li>
<li><a href="https://videocardz.com/newz/micron-says-worlds-first-512gb-ddr5-module-will-be-production-ready-for-2027">Micron says world’s first 512GB DDR5 module will be production ready for 2027 - VideoCardz.com</a></li>

</ul>
</details>

**Tags**: `#DDR5`, `#server memory`, `#Micron`, `#3D stacked DRAM`, `#hardware`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed Raises Rates a Quarter Point, Signals More Hikes Likely](https://www.cnbc.com/2026/09/16/here-are-five-key-takeaways-from-wednesdays-fed-rate-hike.html) ⭐️ 9.0/10

The Federal Reserve on Wednesday raised its key interest rate by a quarter percentage point to a target range of 3.75%-4%, its first hike in more than three years, in a unanimous 12-0 vote. Updated projections showed 16 of 18 participants expected at least one more rate hike this year.

rss · CNBC Finance · Sep 16, 21:23

**「Background」** The Fed had been on hold all year before the hike, and Chair Kevin Warsh said inflation has been &quot;too high ... for too long&quot;; officials projected headline PCE inflation at 3.7% and core inflation at 3.4% this year, both 0.1 percentage point above their June estimates.

**「Impact」** Stocks sold off after the decision, with the Dow Jones Industrial Average tumbling 631 points, while the 2-year Treasury yield, the security most sensitive to Fed rate expectations, rose more than 7 basis points.

**Tags**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#market reaction`, `#FOMC dot plot`

---

<a id="item-finance-news-2"></a>
### [Hong Kong Unveils 11 Measures to Encourage Childbirth](https://www.info.gov.hk/gia/general/202609/16/P2026091600265.htm) ⭐️ 7.0/10

Hong Kong Chief Executive John Lee&\#x27;s policy address set out 11 measures to encourage childbirth, including extending the HK$20,000 newborn baby bonus for three years and raising it to HK$30,000 for a family&\#x27;s second or later child born on or after today. Other measures include lifting the child tax allowance for second and later children from HK$140,000 to HK$160,000 from the 2026/27 tax year, a stamp duty rebate of up to HK$20,000 for eligible parents who buy a home, and a higher mortgage limit for such families under the next Home Ownership Scheme sale.

telegram · zaihuapd · Sep 16, 08:01

**「Background」** Hong Kong&\#x27;s government is shifting from its past non-intervention stance on family size; the HK$20,000 newborn bonus being extended was due to expire on 24 October, and last year&\#x27;s policy address already added 15 subsidised standalone child care centres. The move comes as mainland Chinese cities have been rolling out cash incentives aimed at raising births since early 2025.

**「Who is affected」** Under the announced package, white-form applicants for subsidised Home Ownership Scheme flats who have a newborn could mortgage up to 95% of the price, cutting the upfront deposit, while eligible families buying a home in the specified window could receive up to HK$20,000 off stamp duty — a relief that takes effect only after the amendment bill is passed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cls.cn/detail/2196881">中国 鼓 励 生 育 措 施 前移：多地发钱 鼓 励 结婚</a></li>
<li><a href="https://kaopu.news/story/2026-09-16/hong-kong-boosts-childbirth-incentives-0886f8">香 港 特首李家超宣布 11 项 措 施 鼓 励 生 育 - 靠谱新闻</a></li>
<li><a href="https://www.163.com/dy/article/L6V5J2S10519QIKK.html?clickfrom=w_house">163.com/dy/article/L6V5J2S10519QIKK.html?clickfrom=w_house</a></li>

</ul>
</details>

**Tags**: `#Hong Kong policy`, `#fertility incentives`, `#tax allowances`, `#housing/mortgage`, `#childcare`

---

<a id="item-finance-news-3"></a>
### [Pinglu Canal opens, giving southwest China a new water route to ASEAN](https://www.news.cn/politics/20260916/4d3b671357d14c8db202cbf6120f2c43/c.html) ⭐️ 7.0/10

According to Xinhua, the 134.2 km Pinglu Canal has opened to navigation after construction began in August 2022, built with over RMB 70 billion in investment and able to carry 5,000-tonne vessels. Xinhua reports that cargo from southwest China now travels more than 560 km less than on the traditional route, cutting logistics costs by 18% to 30%, and that two river-sea direct services — Nanning–Can Tho, Vietnam and Nanning–Yangpu — made their first voyages.

telegram · zaihuapd · Sep 16, 09:10

**「Background」** The canal is a backbone project of China&\#x27;s Western Land-Sea New Corridor, meant to give southwest China a direct river-sea link to the Beibu Gulf, its nearest sea outlet, which previously lacked a north-south connection to the Xijiang river system. The idea dates back more than a century to Sun Yat-sen&\#x27;s plan for Qinzhou as a major outlet, and construction began in August 2022.

**「Impact」** Exporters in China&\#x27;s southwest and Guangxi&\#x27;s port, shipping and logistics businesses are the clearest beneficiaries, since inland cargo can now reach Beibu Gulf ports by a direct river-sea route that reports citing Vietnamese media and Chinese analysts say is about 560 km shorter than the route via Guangzhou and cuts logistics costs by 18%–30%.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news.cn/local/20260603/6d0200fe38e44a3cbf64434446ea5fa3/c.html">这条新运河为何备受关注——一文读懂平陆运河-新华网</a></li>
<li><a href="https://news.sina.com.cn/zx/gj/2026-09-16/doc-iniryqve3341143.shtml">世纪工程平陆运河今日通航_新浪新闻</a></li>
<li><a href="https://www.sohu.com/a/1076680147_203783">平陆运河，正式通航_广西_达海_江海</a></li>
<li><a href="https://www.chinanews.com.cn/aseaninfo/2026/09-16/10697404.shtml">全球媒体聚焦丨“平陆运河为东盟国家创造更多增长机遇”-中新网</a></li>
<li><a href="https://www.chinanews.com.cn/dxw/2026/09-15/10697067.shtml">东西问丨余虹：平陆运河通航将如何重构中国—东盟经贸格局？-中新网</a></li>
<li><a href="https://www.sohu.com/a/1076477959_121443915">东西问丨余虹：平陆运河通航将如何重构中国—东盟经贸格局？_广西_产业链_物流</a></li>

</ul>
</details>

**Tags**: `#infrastructure`, `#China-ASEAN trade`, `#logistics`, `#Pinglu Canal`, `#regional development`

---