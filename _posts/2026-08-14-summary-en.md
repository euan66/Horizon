---
layout: default
title: "Horizon Summary: 2026-08-14 (EN)"
date: 2026-08-14
lang: en
---

> From 44 items, 18 important content pieces were selected

---

**Technology News**
1. [OpenAI and Cerebras Unveil GPT-5.6 Sol Ultrafast](#item-tech-news-1) ⭐️ 8.0/10
2. [DRAM Controller Manipulation Research Exposes Low-Level Attack Surface](#item-tech-news-2) ⭐️ 8.0/10
3. [Why Teams Should Choose Boring Technology](#item-tech-news-3) ⭐️ 8.0/10
4. [systemd-journald writes 49KB+ per log line on ext4, 110KB+ on btrfs](#item-tech-news-4) ⭐️ 8.0/10
5. [DeepMind Unveils SL2T Sign-Language-to-Text AI on Pixel 11](#item-tech-news-5) ⭐️ 8.0/10
6. [Gemini 3.7 Flash Launch Sparks Pricing and Value Debate](#item-tech-news-6) ⭐️ 7.0/10
7. [DeepSeek Harness Developer Preview: Traceable Agent Plugins](#item-tech-news-7) ⭐️ 7.0/10
8. [Understanding Code Becomes the New Bottleneck](#item-tech-news-8) ⭐️ 7.0/10
9. [Kubernetes on Oxide: Customer Needs Drive CCM and Cluster API Integrations](#item-tech-news-9) ⭐️ 7.0/10
10. [City2Graph Library Converts Urban Geodata into Heterogeneous Graphs](#item-tech-news-10) ⭐️ 7.0/10
11. [Worldproof shows pixel metrics fail to rank world models on real robot video](#item-tech-news-11) ⭐️ 7.0/10
12. [X open-sources ranking algorithm, lets users check if posts are flagged](#item-tech-news-12) ⭐️ 7.0/10
13. [Vivodyne scales human-tissue testing, aiming to replace animal tests](#item-tech-news-13) ⭐️ 7.0/10

**Financial News**
1. [S&amp;P 500 profit margins hit record 16.9% in Q2, supporting stock rally](#item-finance-news-1) ⭐️ 8.0/10
2. [US President Announces Drone Tariffs, Up to 100% on Some Imports](#item-finance-news-2) ⭐️ 8.0/10
3. [Ackman’s Pershing Square discloses new Netflix stake](#item-finance-news-3) ⭐️ 7.0/10
4. [China’s Gig Workforce Grows to 53 Million as Slowdown Squeezes Jobs](#item-finance-news-4) ⭐️ 7.0/10
5. [Apple Proposes Up to 15% Commission for Off-App-Store Purchases](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI and Cerebras Unveil GPT-5.6 Sol Ultrafast](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 8.0/10

OpenAI and Cerebras announced GPT-5.6 Sol Ultrafast, a faster inference mode that the companies say completed all 2,500 Humanity&\#x27;s Last Exam \(HLE\) questions in 11 hours and 11 minutes, compared with Claude Fable 5&\#x27;s 78 hours and 27 minutes, achieving comparable accuracy nearly 7x faster. The announcement highlights that the ultrafast variant can work through frontier benchmarks in a single working day, and commenters also cite output-speed comparisons of 11x faster than Fable 5 and 5x faster than Opus 4.8 on Fast mode. However, neither the Cerebras nor OpenAI posts explicitly state that Ultrafast preserves the same performance as the regular GPT-5.6 Sol, and no pricing information has been released. The collaboration is significant because inference speed can affect how models are deployed and iterated for real-world use, but the unresolved parity question leaves room for skepticism.

hackernews · pr337h4m · Aug 13, 18:10 · [Discussion](https://news.ycombinator.com/item?id=49289844)

**「Background」** GPT-5.6 Sol is OpenAI&\#x27;s latest frontier large language model, and Ultrafast mode is a newly previewed OpenAI API service tier, powered by Cerebras, that runs the model up to 14× faster with up to 750 output tokens per second. Cerebras, known for its wafer-scale AI accelerators, announced the collaboration in a blog post and investor press release, stating the speed comes without quality compromise. The new tier is initially available to a select group of customers, with broader access expected over time.

**「Impact」** OpenAI has previewed Ultrafast, a new API service tier for GPT-5.6 Sol powered by Cerebras that runs up to 14x faster than Standard processing and generates up to 750 output tokens per second, giving developers a concrete way to run the model with dramatically lower latency. However, OpenAI has not yet announced pricing for the tier, and the company has not explicitly stated that accuracy in Ultrafast mode is identical to Standard mode, leaving performance parity and cost as open questions.

**「Community Discussion」** Community reactions mix enthusiasm with skepticism: some celebrate the long-awaited OpenAI-Cerebras result and argue faster inference improves iterative reasoning, while others note the lack of an explicit statement that Ultrafast performs exactly like regular 5.6 Sol and flag the absence of pricing information.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT‑5.6 Sol at up to ... - OpenAI</a></li>
<li><a href="https://investors.cerebras.ai/news-releases/news-release-details/cerebras-powers-ultrafast-mode-openais-gpt-56-sol">Cerebras Powers Ultrafast Mode for OpenAI’s GPT-5.6 Sol ...</a></li>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT-5.6 Sol Ultrafast with OpenAI - cerebras.ai</a></li>
<li><a href="https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai">Accelerating GPT - 5 . 6 Sol Ultrafast with OpenAI</a></li>
<li><a href="https://openai.com/index/previewing-ultrafast/">Previewing Ultrafast mode: GPT - 5 . 6 Sol at up to 14X the speed</a></li>

</ul>
</details>

**Tags**: `#openai`, `#cerebras`, `#gpt`, `#ai-hardware`, `#llm-inference`

---

<a id="item-tech-news-2"></a>
### [DRAM Controller Manipulation Research Exposes Low-Level Attack Surface](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 8.0/10

Security researcher Christopher Domas released a project called &quot;Spaghettifying DRAM&quot; that demonstrates techniques for manipulating DRAM controller behavior to enable low-level system compromise, including access to normally protected &quot;negative ring&quot; territory. The work is presented through a GitHub repository and an accompanying Black Hat talk, and it targets the AMD Jaguar architecture, an older AMD low-power family from around 2013. The research exposes DRAM controllers themselves as a significant attack surface, with notes indicating newer CPUs such as Zen 3 use a different base address for memory controller registers. It matters because it shows that once ring 0 code execution is achieved, an attacker can potentially expand control to nearly all hidden hardware privileges on affected systems.

hackernews · matt\_d · Aug 13, 14:17 · [Discussion](https://news.ycombinator.com/item?id=49286341)

**「Background」** DRAM scrambling is a memory controller feature that obfuscates the mapping between physical addresses and DRAM cells, normally to mitigate side-channel attacks and improve signal integrity. This research by Christopher Domas \(xoreaxeaxeax\) shows that flipping specific configuration bits in the memory controller can &\#x27;spaghettify&\#x27; the address mapping, defeating DRAM scrambling and exposing low-level CPU features such as the Platform Security Processor \(PSP\), microcode updates, SMM, and other areas hidden from normal ring-0 access. The attack specifically targets AMD&\#x27;s Jaguar architecture \(AMD16h\), a 2013 low-power family, though notes indicate Zen 3 has a different memory controller register base address, leaving uncertainty about which other processor families might be susceptible.

**「Impact」** On affected AMD Jaguar-based systems, an attacker with ring-0 code execution can flip memory controller configuration bits to remap physical addresses and access or alter data in the CPU&\#x27;s most protected negative-ring memory regions, undermining the isolation normally provided by the memory controller. The research is so far demonstrated only on the 2013-era AMD Jaguar architecture, and it remains unproven whether the technique can be ported to newer families such as Zen 3 or whether boot-time lockdowns prevent the required register reconfiguration.

**「Community Discussion」** Commenters expressed strong enthusiasm for Domas&\#x27;s upcoming Black Hat talk, citing his past reverse-engineering and hardware security presentations as highly accessible and compelling. Several questioned how broadly the attack applies beyond AMD Jaguar, while others noted the growing complexity and attack surface of modern DRAM interfaces and speculated that console security teams may be concerned about post-ring-0 exploitation possibilities.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/dram-scrambling-attack/">New DRAM Scrambling Attack Exposes CPU&#x27;s Most Protected...</a></li>
<li><a href="https://github.com/xoreaxeaxeax/skitter-creek-bath-salts">GitHub - xoreaxeaxeax/ skitter - creek - bath - salts : Unlocking...</a></li>
<li><a href="https://cybersecuritynews.com/dram-scrambling-attack/">New DRAM Scrambling Attack Exposes CPU&#x27;s Most Protected...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49286341">Spaghettifying DRAM | Hacker News</a></li>

</ul>
</details>

**Tags**: `#hardware-security`, `#DRAM`, `#exploitation`, `#reverse-engineering`, `#low-level-systems`

---

<a id="item-tech-news-3"></a>
### [Why Teams Should Choose Boring Technology](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

The 2015 essay &\#x27;Choose Boring Technology&\#x27; argues that organizations have a limited supply of &\#x27;innovation tokens&\#x27;—a fixed capacity for adopting new, unproven technology—and should spend those tokens selectively rather than chasing novelty for every problem. It recommends defaulting to mature, well-understood &\#x27;boring&\#x27; technologies for most work, reserving innovation for areas where it can create real competitive advantage. The concept has become a touchstone for engineering-culture discussions, especially as a way to explain technical tradeoffs to colleagues at all levels. The accompanying Hacker News discussion shows it remains influential, with readers extending the idea to modern AI-agent tooling choices.

hackernews · tosh · Aug 13, 17:48 · [Discussion](https://news.ycombinator.com/item?id=49289512)

**「Background」** Dan McKinley&\#x27;s 2015 essay argues that organizations have a limited capacity for innovation, metaphorically called &\#x27;innovation tokens,&\#x27; and that spending them on new or trendy infrastructure leaves little room for solving the problems that actually differentiate the business. The piece emerged amid widespread JavaScript framework churn, using examples like Node.js and MongoDB as token-expending choices, while recommending dependable tools such as Postgres, Python, Memcached, and Cron. The essay&\#x27;s core framework remains a common reference for pragmatic technology selection.

**「Community Discussion」** Commenters largely endorse the framework: one PM and engineering leader calls innovation tokens one of the most useful concepts in their career, and another suggests pushing all innovation tokens into AI agents while keeping the rest of the stack boring. Others push back, arguing novelty is a weak proxy and engineers should evaluate requirements, risks, and tradeoffs directly; one commenter also views the essay as a reaction to JavaScript framework churn and cites IBM&\#x27;s late move to integrated circuits as a historical counterpoint.

<details><summary>References</summary>
<ul>
<li><a href="https://mcfunley.com/choose-boring-technology">Dan McKinley :: Choose Boring Technology</a></li>
<li><a href="https://jadon.us/posts/notes-on-choose-boring-technology/">Notes on - Choose Boring Technology by Dan McKinley</a></li>
<li><a href="https://www.annageller.com/p/summary-choose-boring-technology">Summary: Choose Boring Technology by Dan McKinley - Anna Geller</a></li>

</ul>
</details>

**Tags**: `#software-engineering`, `#technology-choice`, `#innovation-tokens`, `#engineering-culture`, `#pragmatism`

---

<a id="item-tech-news-4"></a>
### [systemd-journald writes 49KB+ per log line on ext4, 110KB+ on btrfs](https://github.com/systemd/systemd/issues/40262) ⭐️ 8.0/10

A GitHub issue reports that systemd-journald can cause 49KB+ of disk writes on ext4 and 110KB+ on btrfs for a single log line, exposing a serious inefficiency in its file allocation strategy. The problem matters because journald is a core logging component in many Linux systems, and such exaggerated write amplification can increase I/O load and storage wear. The report includes concrete measurements and has generated active community discussion. This issue highlights a significant performance flaw in systemd-journald that systems engineers and anyone relying on journald for logging should consider. No further technical details are available from the supplied source content.

hackernews · ValdikSS · Aug 13, 18:41 · [Discussion](https://news.ycombinator.com/item?id=49290215)

**「Background」** systemd-journald is the logging daemon of the systemd init system, storing structured logs in a binary journal format rather than plain text files. Its native journal format is inspired by classic log files and git repositories: log data is appended only at the end to ensure robustness and atomicity with mmap\(\)-based access, while header metadata references the new additions. This append-only design, combined with indexing and filesystem allocation behavior, can result in far more disk writes than the log message itself contains, which is why a single log line can cause 49KB+ writes on ext4 or 110KB+ writes on btrfs.

**「Impact」** Users relying on systemd-journald for logging may experience significantly elevated disk I/O and storage wear because even a small log entry can trigger 49KB or 110KB of writes depending on the filesystem.

**「Community Discussion」** Commenters criticize journald for poor indexing performance and lack of control over chatty subsystems, with some recommending using it only as a router and forwarding logs to rsyslog for filtering. One commenter notes that journald&\#x27;s design does not match the original intent and that a single buggy driver can generate tens or hundreds of thousands of log entries per day, making the write amplification worse.

<details><summary>References</summary>
<ul>
<li><a href="https://eucloudservers.com/data-platforms-storage/single-log-line-is-49kb-ext4-110kb-btrfs-of-systemd-journald-disk-writes/">Single Log Line Is 49 KB + ( Ext 4 ) / 110KB+ ( Btrfs )... - EU Cloud Servers</a></li>
<li><a href="https://wiki.archlinux.org/title/Systemd/Journal">systemd /Journal - ArchWiki</a></li>

</ul>
</details>

**Tags**: `#systemd`, `#journald`, `#logging`, `#filesystem`, `#performance`

---

<a id="item-tech-news-5"></a>
### [DeepMind Unveils SL2T Sign-Language-to-Text AI on Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

Google DeepMind has released SL2T, a large-scale multilingual sign language-to-text model, and for the first time is bringing sign language AI into consumer products: it launches on the Pixel 11, supporting American Sign Language \(ASL\) to English in Gboard and Live Transcribe, with plans to expand to more devices and languages. The model was trained on over 100,000 hours of sign language data spanning more than 50 sign languages, and achieves a zero-shot score of 70 BLEURT on the FLEURS-ASL benchmark, well above the previous record. To protect privacy, SL2T processes only hand and body pose keypoints rather than raw video. This deployment is significant because it puts sign language understanding into widely used accessibility tools on consumer hardware.

telegram · zaihuapd · Aug 13, 08:55

**「Background」** Sign language-to-text AI has been challenging because sign languages are distinct, visual languages with far less training data than spoken languages. DeepMind&\#x27;s SL2T addresses this by training across more than 50 sign languages and using pose keypoints to preserve privacy, while also establishing a new benchmark on FLEURS-ASL.

**「Impact」** American Sign Language users with a Pixel 11 can now use Gboard and Live Transcribe to convert sign language into English text on-device, with the promise of broader language and device support later.

**Tags**: `#sign language`, `#DeepMind`, `#AI accessibility`, `#machine learning`, `#speech-to-text`

---

<a id="item-tech-news-6"></a>
### [Gemini 3.7 Flash Launch Sparks Pricing and Value Debate](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 7.0/10

Google introduced Gemini 3.7 Flash, a fast model in its Gemini lineup, with API documentation linked from the announcement. The release follows Gemini 3.6 Flash by only about three weeks and gives developers another low-cost, high-volume option for text-heavy and vision-related tasks like image-to-HTML. Practical tests already show strong vision performance relative to its price, though commenters note the introductory pricing is scheduled to double on December 31, 2026. The model also performs well on the DeepSWE 1.1 benchmark, but cheaper alternatives such as Luna still lead in some comparisons. Overall, this is an incremental but notable update for Gemini API users rather than a paradigm shift.

hackernews · thisisauserid · Aug 13, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49289112)

**「Background」** Gemini Flash models are Google&\#x27;s lightweight, low-latency AI models designed for high-volume, cost-sensitive workloads such as summarization, parsing, and agentic tasks. Gemini 3.7 Flash is the latest in this line, launched with an introductory price of $0.75 per million input tokens and $3.75 per million output tokens through December 31, 2026, after which prices are scheduled to double to $1.50 and $7.50 per million tokens, matching the standard pricing of the preceding Gemini 3.6 Flash model.

**「Impact」** Gemini 3.7 Flash became generally available on August 13, 2026, at half Gemini 3.6 Flash&\#x27;s introductory pricing, giving API developers a faster and more competitively priced option for high-volume text workloads, with benchmark gains reported as real. However, the price is scheduled to double after December 31, 2026, and community discussion highlights that cheaper models such as Luna may undercut the Flash line&\#x27;s value proposition.

**「Community Discussion」** Commenters generally praise Gemini 3.7 Flash&\#x27;s vision-to-HTML output and benchmark results for its price, but several question its positioning: one tester found Opus still best in class for image-to-HTML while Gemini 3.7 looked strong at a comparable price, and another said Luna \(Max\) still beats it on DeepSWE 1.1. Others criticize the introductory pricing schedule, noting it is set to double at the end of 2026, that 3.6 Flash shipped only weeks earlier, and that cheaper options like Luna undercut the need for Flash.

<details><summary>References</summary>
<ul>
<li><a href="https://venturebeat.com/technology/googles-gemini-3-7-flash-targets-coding-and-agents-with-a-50-introductory-price-cut">Google’s Gemini 3.7 Flash targets coding and agents with a 50% introductory price cut | VentureBeat</a></li>
<li><a href="https://www.youtube.com/watch?v=6WAReFHbnUQ">Gemini 3 . 7 Flash Explained in 5 Minutes - Benchmarks... - YouTube</a></li>
<li><a href="https://artificialanalysis.ai/models/gemini-3-7-flash">Gemini 3 . 7 Flash (high) - Intelligence, Performance &amp; Price Analysis</a></li>

</ul>
</details>

**Tags**: `#Gemini`, `#Google AI`, `#LLM`, `#model release`, `#pricing`

---

<a id="item-tech-news-7"></a>
### [DeepSeek Harness Developer Preview: Traceable Agent Plugins](https://deepseek.com/harness/en/) ⭐️ 7.0/10

DeepSeek has released an early developer preview of DeepSeek Harness, an open-source agent harness framework under the MIT license. The framework emphasizes full traceability: every run is recorded in an append-only session log covering system prompts, reasoning, tool calls, subagent scheduling, and context injections, inspectable in a Trajectory view with resume, fork, search, and replay capabilities. It also introduces a plugin system with hot-reload and dynamic enable/dispose features, built on Cordis v4, which can revert side effects when unloading plugins. DeepSeek Harness is at an early stage, so users should expect rough edges and compatibility-breaking changes.

hackernews · bjin · Aug 13, 12:58 · [Discussion](https://news.ycombinator.com/item?id=49285244)

**「Background」** DeepSeek Harness \(dsh\) is an open-source framework from DeepSeek AI for building and running AI agents, centered on a plugin architecture and traceable sessions. In agent engineering, a &\#x27;harness&\#x27; is the runtime layer that orchestrates model calls, tools, memory, and subagents, so the framework aims to make those components modular and inspectable. The early developer preview builds on Cordis v4, a plugin system for hot-loading and unloading plugins that was already used in the Koishi bot framework, and it is released under the MIT license but is not yet stable.

**「Impact」** AI agent developers gain an open-source framework with fully traceable agent executions and hot-swappable plugins, but the preview status means it is not yet suitable for production use without expecting breaking changes.

**「Community Discussion」** Commenters praised the traceable event-stream design and the plugin cleanup capabilities as standout features, while others argued the concept is not new, comparing it to Eclipse-style plugins, and questioned its practical utility beyond previous agent systems.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/deepseek-harness">GitHub - deepseek-ai/deepseek-harness: DeepSeek Harness: Everything is a Plugin. · GitHub</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#ai-agents`, `#agent-harness`, `#open-source`, `#traceability`

---

<a id="item-tech-news-8"></a>
### [Understanding Code Becomes the New Bottleneck](https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck) ⭐️ 7.0/10

An essay argues that comprehension, not code generation, is now the limiting factor in software development, particularly as LLM-assisted workflows make it easier to produce code. The post contends that this problem predates LLMs: code that works while breaking the underlying model is difficult to spot unless the reader holds the model as the standard. It drew significant Hacker News engagement, with 257 points and 140 comments. Commenters offered supporting examples, such as LLM-generated pull request descriptions being mechanically detailed but lacking motivation, and emphasized the need for humans to understand code in order to verify LLM outputs.

hackernews · sebg · Aug 13, 18:47 · [Discussion](https://news.ycombinator.com/item?id=49290299)

**「Background」** Geoffrey Litt, a Design Engineer at Notion, published this essay as a written version of a talk he gave at the AI Engineer conference in July 2026. The piece argues that in modern software development—especially with LLM assistance—understanding or comprehending code has become the more critical bottleneck compared to generating code. Litt proposes techniques such as explanations, micro-worlds, and shared spaces to help developers build deeper understanding of AI-generated code.

**「Impact」** The takeaway for software teams is that improving code comprehension and maintaining a clear mental model of the codebase will matter more than maximizing code generation throughput in LLM-assisted development.

**「Community discussion」** Commenters largely agree with the diagnosis, with one noting that engineers are discovering a long-standing bottleneck previously handled by engineering leadership and program management. Others report that LLM-generated PR descriptions are universally disliked for their lack of motivation, and one commenter agrees with the problem but not the proposed solutions, arguing that the underlying issue predates LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck">Understanding is the new bottleneck</a></li>
<li><a href="https://www.startuphub.ai/ai-news/artificial-intelligence/2026/understanding-is-the-new-bottleneck-in-ai">Understanding is the New Bottleneck in AI | StartupHub.ai</a></li>

</ul>
</details>

**Tags**: `#software engineering`, `#LLMs`, `#code comprehension`, `#developer productivity`, `#program management`

---

<a id="item-tech-news-9"></a>
### [Kubernetes on Oxide: Customer Needs Drive CCM and Cluster API Integrations](https://oxide.computer/blog/kubernetes-on-oxide) ⭐️ 7.0/10

Oxide&\#x27;s blog post describes how customer requirements influenced its Kubernetes integrations on Oxide hardware, specifically the cloud-controller-manager \(CCM\) and Cluster API. It discusses the \`oxide-cloud-controller-manager\` being built for modern Kubernetes and explores whether the design yields meaningful differences from CCMs that originated in-tree. The post also covers Cluster API as an approach for managing Kubernetes clusters on bare metal. The material is technical and aimed at infrastructure engineers. Specific versions, dates, and performance data are not included in the supplied summary.

hackernews · stevehipwell · Aug 13, 14:26 · [Discussion](https://news.ycombinator.com/item?id=49286485)

**「Background」** Oxide is a company selling on-premises, rack-scale cloud hardware with its own control plane and APIs, allowing organizations to run cloud-native workloads outside traditional public clouds. Its Kubernetes integrations include a Cluster API provider \(CAPOx\) for provisioning clusters, and an optional cloud-controller-manager \(CCM\) that runs inside managed clusters to connect Kubernetes with Oxide APIs at runtime, handling node health, load balancing, and routes. Cluster API is the Kubernetes project for declarative cluster lifecycle management, while the CCM pattern integrates Kubernetes with underlying infrastructure providers.

**「Community Discussion」** Commenters expressed interest in how \`oxide-cloud-controller-manager\` is being built and whether it differs from in-tree CCMs; one predicted a \`karpenter-provider-oxide\` would appear. Others asked about Kubernetes on Oxide versus KubeVirt/Proxmox setups, wanted Oxide to open source its documentation system, and praised Cluster API as an underappreciated but solid approach.

<details><summary>References</summary>
<ul>
<li><a href="https://oxide.computer/blog/kubernetes-on-oxide">Kubernetes on Oxide : How Customer Needs Shaped Our Integrations</a></li>
<li><a href="https://techfieldday.com/appearance/oxide-presents-at-cloud-field-day-24/?trk=article-ssr-frontend-pulse_little-text-block">Oxide Presents at Cloud Field Day 24 - Tech Field Day</a></li>
<li><a href="https://rfd-site.vercel.app/rfd/0493">493 - Initial Kubernetes Integrations / RFD / Oxide</a></li>

</ul>
</details>

**Tags**: `#Kubernetes`, `#Cloud Controller Manager`, `#Cluster API`, `#Oxide`, `#Bare Metal`

---

<a id="item-tech-news-10"></a>
### [City2Graph Library Converts Urban Geodata into Heterogeneous Graphs](https://www.reddit.com/r/MachineLearning/comments/1vn8oya/city2graph_a_python_library_for_heterogeneous/) ⭐️ 7.0/10

City2Graph is a newly published Python library that turns geospatial data into analysis-ready heterogeneous graphs for spatial analysis, network analysis, and Graph Neural Networks in GeoAI. It covers morphological graphs of buildings, streets, and urban fabric from OpenStreetMap and Overture Maps; transportation graphs from GTFS and GBFS feeds loaded through DuckDB; mobility graphs from OD matrices and flow data; and proximity/contiguity graphs using KNN, Delaunay, Gilbert, Waxman, and queen/rook methods under Euclidean, Manhattan, or network distances. The library supports heterogeneous node and edge types with metapaths, and provides round-trip conversions between GeoDataFrames, NetworkX, rustworkx, and PyTorch Geometric Data/HeteroData while preserving geometries and attributes. The accompanying peer-reviewed paper appears in Computers, Environment and Urban Systems \(volume 130, article 102492\) and is endorsed for citation when using the library in research. The project is available on GitHub at https://github.com/c2g-dev/city2graph, with issues and pull requests welcome.

reddit · r/MachineLearning · /u/Tough\_Ad\_6598 · Aug 13, 11:59

**「Background」** Urban systems analysis traditionally treats geographic data as flat feature tables, which loses the relational structure between buildings, streets, transit stops, and movement flows. Graph Neural Networks and network analysis require explicit graph representations, and heterogeneous graphs allow multiple node and edge types to coexist, making them well suited to capture the complex interdependencies in urban environments.

**「Impact」** Researchers and developers using GeoAI or urban analytics can now directly convert common geospatial and transit data sources into PyTorch Geometric-compatible heterogeneous graphs without building custom pipelines, reducing friction for GNN-based urban modeling. Support for GTFS, GBFS, and mobility flows also broadens the tool&\#x27;s applicability to transportation and mobility studies.

**Tags**: `#graph neural networks`, `#geospatial data`, `#urban analytics`, `#python library`, `#spatial analysis`

---

<a id="item-tech-news-11"></a>
### [Worldproof shows pixel metrics fail to rank world models on real robot video](https://www.reddit.com/r/MachineLearning/comments/1vnliv7/worldproof_diagnosing_where_worldmodel/) ⭐️ 7.0/10

The open-source diagnostic tool worldproof \(Apache-2.0, pip install worldproof\) evaluates world models by comparing rollouts to ground truth and physical invariants, and its validation found a striking evaluation failure: a last-frame &\#x27;predict nothing changes&\#x27; baseline scored 0.983 SSIM and 53.9 dB PSNR on dynamic regions of a real SO-101 arm recording at 30fps across 64 rollouts and a 6-step horizon, with error flat rather than growing over steps. On DROID at 15fps over 48 steps, the same baseline showed three regimes: near-perfect ties at steps 1-3, a steep monotonic decline at steps 4-24, and a floor around 0.20 SSIM/10.3 dB after step 28 where predictions are decorrelated and models tie again. The usable evaluation window for that footage is roughly steps 8-24, but the author notes this depends on frame rate and task speed. The post also warns that including step 0 inflates horizon-averaged scalars \(119.8 dB at step 0 on the 30fps recording\), LPIPS unexpectedly failed to separate the datasets, and n=8 rollouts gave misleading wide intervals compared with n=64.

reddit · r/MachineLearning · /u/georgia\_bucea · Aug 13, 19:58

**「Background」** World models are neural predictors that produce future frames given context and actions, commonly evaluated with pixel-similarity metrics such as SSIM, PSNR, and LPIPS. A trivial baseline that copies the last frame tests whether the evaluation setup has any discriminative power: if a do-nothing predictor ties near-perfect metrics, better models cannot be ranked.

**「Impact」** Teams evaluating world models on real robot video should measure horizon-dependent curves rather than single scalars and check a static baseline before trusting SSIM/PSNR rankings, with a concrete usable window around 8-24 steps for 15fps manipulation footage; the exact horizon will vary with frame rate and task speed.

**Tags**: `#world models`, `#evaluation metrics`, `#SSIM`, `#PSNR`, `#robotics`

---

<a id="item-tech-news-12"></a>
### [X open-sources ranking algorithm, lets users check if posts are flagged](https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/) ⭐️ 7.0/10

X has expanded its open-source release by publishing the &quot;For You&quot; timeline and core ranking engine code on GitHub under the Apache 2.0 license, with the codebase roughly 10 to 15 times larger than its previous disclosure. The company also introduced a transparency tool in settings that lets users who posted at least 10 times in the past month download a JSON file showing whether their account or posts have been flagged by the ranking system. The tool is initially rolling out to test users whose accounts have been registered for at least one year. However, X did not disclose parts of its Grok system used to judge rule-violating content.

telegram · zaihuapd · Aug 14, 01:03

**「Background」** X \(formerly Twitter\) has gradually opened parts of its recommendation system since Elon Musk’s acquisition, but this latest release is a significant expansion: the company published the source code for the &\#x27;For You&\#x27; timeline and core ranking engine on GitHub under the permissive Apache 2.0 license. Previously, X had only released smaller, partial components, and the new code represents a complete rewrite rather than just an update. The announcement follows Musk’s January 10, 2026, pledge to open-source the full recommendation algorithm, and the newly added transparency tool reflects growing pressure on platforms to explain how ranking decisions affect content visibility.

**「Impact」** Eligible X users can now proactively check whether their account or posts have been flagged by the ranking system, and developers can freely inspect and reuse the core ranking engine code under a permissive license. The disclosure is incomplete, though: the Grok-based content-violation judgment system remains proprietary.

<details><summary>References</summary>
<ul>
<li><a href="https://www.okaynews.com/x-expands-open-source-algorithm-and-adds-ranking-transparency-tool/">X Expands Open-Source Algorithm and Adds Ranking Transparency...</a></li>
<li><a href="https://cryptobriefing.com/x-open-sources-for-you-algorithm/">X open-sources For You algorithm to enhance transparency and ...</a></li>

</ul>
</details>

**Tags**: `#open source`, `#algorithm transparency`, `#social media`, `#ranking algorithm`, `#X`

---

<a id="item-tech-news-13"></a>
### [Vivodyne scales human-tissue testing, aiming to replace animal tests](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 7.0/10

Vivodyne is operating a robotic laboratory system in South San Francisco that uses AI-designed experiments to test human tissues at unprecedented scale. The system currently has 12 “hive” robotic labs and can run more than 3 million controlled tissue experiments per year, roughly twice the capacity of all U.S. clinical trials combined, according to the company. Vivodyne’s approach is intended to better predict drug efficacy and safety before human trials, addressing the fact that about 90% of clinical trials fail even after passing animal testing. If validated, this could make traditional animal testing obsolete and reshape drug development, though the specific technical details and independent verification are not provided in the source.

telegram · zaihuapd · Aug 14, 01:48

**「Background」** Drug development has long relied on animal testing to predict safety and efficacy, yet animal models often fail to mirror human biology, contributing to the roughly 90% of clinical trials that fail even after passing animal tests. Vivodyne is building what it calls the world&\#x27;s largest human biological datacenter, using robotic experimentation on lab-grown, vascularized human tissues at the scale of large clinical biopsies to generate data for training AI models of human biology. The company says this approach can recapitulate the complexity of human disease more accurately than animal models, which is why it has attracted a $40 million Series A to scale its AI-powered human tissue testing.

**「Impact」** For drug developers and clinical researchers, Vivodyne’s claimed capacity could offer a higher-throughput, human-relevant alternative to animal models for early drug screening, potentially reducing late-stage clinical trial failures. However, these benefits depend on the reliability and regulatory acceptance of the AI-designed tissue experiments, which remain to be proven.

<details><summary>References</summary>
<ul>
<li><a href="https://www.businesswire.com/news/home/20260812148428/en/Vivodyne-Launches-the-Worlds-Largest-Human-Biological-Datacenter-to-Train-the-First-World-Model-of-Human-Biology">Vivodyne Launches the World’s Largest Human Biological Datacenter...</a></li>
<li><a href="https://hitconsultant.net/2025/05/30/vivodyne-secures-40m-series-a-to-scale-ai-powered-human-tissue-testing/">Vivodyne Secures $40M Series A to Scale AI -Powered Human ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Drug Discovery`, `#Lab Automation`, `#Biotech`, `#Robotics`

---

## Financial News

<a id="item-finance-news-1"></a>
### [S&amp;P 500 profit margins hit record 16.9% in Q2, supporting stock rally](https://www.cnbc.com/2026/08/13/these-charts-show-why-stocks-keep-rallying-profit-margins-are-highest-on-record.html) ⭐️ 8.0/10

S&amp;P 500 net profit margins hit a record 16.9% in the second quarter, up from 14.8% in the first quarter and 12.9% a year earlier, according to FactSet data cited by CNBC.

rss · CNBC Finance · Aug 13, 20:21

**「Background」** Net profit margin is the percentage of revenue a company keeps after paying all expenses. The gain was broad, with eight of 11 S&amp;P 500 sectors reporting higher margins than a year earlier; Alphabet and Amazon were the biggest contributors, but even excluding them the margin was a record 15%.

**Tags**: `#S&amp;P 500`, `#profit margins`, `#corporate earnings`, `#stock market`, `#FactSet`

---

<a id="item-finance-news-2"></a>
### [US President Announces Drone Tariffs, Up to 100% on Some Imports](https://www.whitehouse.gov/presidential-actions/2026/08/adjusting-imports-of-unmanned-aircraft-systems-and-unmanned-aircraft-systems-components-into-the-united-states/) ⭐️ 8.0/10

The U.S. president signed a proclamation on August 13 imposing a 100% tariff starting September 3, 2026, on imported drones with a maximum takeoff weight over 25 kg, drones with thermal imagers, drone base stations, and certain key components, while drones weighing 25 kg or less will face a 25% tariff; an additional 25% tariff on some other drone components will take effect on February 9, 2027.

telegram · zaihuapd · Aug 14, 01:24

**「Background」** Tariffs are import duties paid by importers when goods enter the United States; this proclamation adjusts imports of unmanned aircraft systems and their components on a phased schedule.

**「Impact」** The tariffs will raise costs for U.S. importers, drone buyers, and manufacturers that rely on affected foreign components once the duties take effect in 2026 and 2027.

**Tags**: `#drones`, `#tariffs`, `#US trade policy`, `#import duties`, `#aviation`

---

<a id="item-finance-news-3"></a>
### [Ackman’s Pershing Square discloses new Netflix stake](https://www.cnbc.com/2026/08/13/ackman-buys-netflix-again-four-years-later-says-it-won-streaming-wars.html) ⭐️ 7.0/10

Bill Ackman’s Pershing Square has disclosed in its semiannual report a new Netflix stake, saying the company has “effectively won the streaming wars” and is attractively valued after a steep sell-off that cut its shares by about 50% from their June 2025 high and left the stock at roughly 21 times forward earnings.

rss · CNBC Finance · Aug 13, 18:04

**「Background」** Ackman briefly owned Netflix in 2022 but exited three months later after the company reported its first subscriber decline in more than a decade and its shares plunged. Pershing now points to Netflix’s 325 million subscribers, nearly twice the combined base of Disney+ and HBO Max, as the scale that lets it spend heavily on programming while spreading costs across a larger audience.

**Tags**: `#Bill Ackman`, `#Netflix`, `#Pershing Square`, `#streaming`, `#investment disclosure`

---

<a id="item-finance-news-4"></a>
### [China’s Gig Workforce Grows to 53 Million as Slowdown Squeezes Jobs](https://www.ft.com/content/a3803e70-cb4d-444f-a31e-05be2f2c44f6?accessToken=zwAAAZ_5xcXzkdOjgD5wy01ET9OjHgW-LyxE9g.MEUCIQCWTIny3JTJV8e-PGyK0XL2tg5g_7Ay-rpKkwGZCpp1-AIgbMgJQPlqWgqAsX4s1k4gYaC4b8k0JveZOs35OJQvbZ4&amp;amp;sharetype=gift&amp;amp;token=7e8483bb-395d-429e-afca-2f4ab5ad150b) ⭐️ 7.0/10

China’s economic slowdown is squeezing the labor market: as of 2025, the number of food-delivery and ride-hailing drivers exceeded 53 million, up 10 million in two years, yet the supply of such gig work still outweighs demand and is cutting incomes and extending working hours.

telegram · zaihuapd · Aug 13, 06:40

**「Background」** China&\#x27;s gig economy has become a crucial employment buffer as the property crisis cuts construction jobs and manufacturers shed workers through automation and cost-cutting, helping explain why 53 million people now work in food delivery and ride-hailing.

**「Impact」** For the more than 53 million gig workers, oversupply translates into longer idle time and lower hourly earnings; taxi drivers at Shanghai Pudong, Beijing Daxing, and Chengdu Tianfu airports have been reported waiting as long as 7, 8, and 10 hours for passengers, and Shenzhen said in June that its ride-hailing market was saturated.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tbsnews.net/world/chinas-booming-gig-economy-masks-job-market-pain-strains-welfare-system-1482271">China&#x27;s booming gig economy masks job market pain, strains ...</a></li>
<li><a href="https://www.ft.com/content/a3803e70-cb4d-444f-a31e-05be2f2c44f6?syn-25a6b1a6=1">China’s great jobs squeeze - Financial Times</a></li>

</ul>
</details>

**Tags**: `#China`, `#gig economy`, `#employment`, `#labor market`, `#economic slowdown`

---

<a id="item-finance-news-5"></a>
### [Apple Proposes Up to 15% Commission for Off-App-Store Purchases](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 7.0/10

Apple has proposed to a US court commissions of up to 15% for purchases made outside the App Store, in the ongoing Epic Games antitrust case. The proposal sets 15% for standard apps, 10% for video/news partnerships and subscription renewals, and 5% for small-business-program apps; it is not final, and Epic has yet to respond.

telegram · zaihuapd · Aug 14, 02:33

**「Background」** The proposal was filed in the ongoing Epic Games antitrust case over Apple’s App Store rules. A federal judge recently rejected Apple’s request to pause the fee proceedings while the Supreme Court reviews a related contempt ruling, so the lower court is deciding the commission rate for purchases made through external links.

<details><summary>References</summary>
<ul>
<li><a href="https://appleinsider.com/articles/26/08/13/apples-latest-commission-rates-for-external-app-store-purchases-havent-satisfied-epic">External App Store purchase commissions won&#x27;t satisfy Epic</a></li>
<li><a href="https://9to5mac.com/2026/08/11/court-rejects-apples-attempt-to-postpone-app-store-fee-proceedings-in-epic-games-case/">Court rejects Apple’s bid to pause App Store fee proceedings ...</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#App Store`, `#antitrust`, `#commissions`, `#Epic Games`

---