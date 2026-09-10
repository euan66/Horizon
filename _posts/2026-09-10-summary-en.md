---
layout: default
title: "Horizon Summary: 2026-09-10 (EN)"
date: 2026-09-10
lang: en
---

> From 41 items, 10 important content pieces were selected

---

**Technology News**
1. [Calif Research claims WeWorm zero-click WeChat call worm with AI-built RCE](#item-tech-news-1) ⭐️ 9.0/10
2. [Shopify moves mobile app from React Native back to Swift and Kotlin](#item-tech-news-2) ⭐️ 8.0/10
3. [Rust Is Now a Tier-1 Language at Microsoft](#item-tech-news-3) ⭐️ 8.0/10
4. [Ant International, Visa and Mastercard to Build AI-Agent Payment Standard](#item-tech-news-4) ⭐️ 8.0/10
5. [DeepSeek releases V4.1 Flash: 552B multimodal model with API pricing changes](#item-tech-news-5) ⭐️ 7.0/10
6. [Tencent Hunyuan Releases Open-Source Audio Editing Model AuK](#item-tech-news-6) ⭐️ 7.0/10

**Technology Blog**
1. [Following the Bottleneck: MiniMax M3 on AMD MI355X](#item-tech-blog-1) ⭐️ 9.0/10
2. [vLLM&\#x27;s Tiered KV Cache Offloading via Host Memory](#item-tech-blog-2) ⭐️ 8.0/10

**Financial News**
1. [Kalshi launches ‘perps’ for gold and silver following CFTC approval, expanding futures offerings](#item-finance-news-1) ⭐️ 7.0/10
2. [China AI chipmakers raise prices as HBM shortage bites](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Calif Research claims WeWorm zero-click WeChat call worm with AI-built RCE](https://simonwillison.net/2026/Sep/10/calif-research/) ⭐️ 9.0/10

Calif Research has released a demo of WeWorm, which it describes as the first zero-click worm to spread through WeChat calls across both iOS and Android. According to the release, the victim does not need to answer the call or interact with the phone at all, and even if they do answer they hear nothing while the exploit still succeeds. The team says that working with AI it found the bug and wrote the first remote code execution exploit in about two days, then built the worm in one more week—work it claims used to take a larger team months, with the humans supplying only judgment about what to target and how to test safely. These claims come from the researchers&\#x27; own release and have not been independently confirmed, so the reported scale and speed of the AI-assisted exploit development remain unverified.

rss · Simon Willison · Sep 10, 00:56

**「Background」** A zero-click exploit compromises a device without any action from the victim—no tap, no answered call, no reply—which is what makes such bugs especially dangerous on widely used messaging platforms. A worm differs from a single-target attack in that it self-propagates: according to Help Net Security, WeWorm hijacks each victim&\#x27;s WeChat account and then uses that account&\#x27;s saved contacts to reach further devices, hopping between iOS and Android phones. Calif Research, which describes its mission as keeping the internet together &quot;by occasionally taking it apart,&quot; published the WeWorm demo on its own research site, so the claims currently rest on the team&\#x27;s release rather than on independent verification.

**「Impact」** For WeChat users on both iOS and Android, Calif Research&\#x27;s demo claims that a single incoming call can hand an attacker full control of the account in seconds and let the worm propagate to the victim&\#x27;s contacts with no interaction at all. That consequence remains unverified beyond the researchers&\#x27; own release, since the cited coverage describes a proof-of-concept demo rather than independently confirmed exploitation in the wild.

<details><summary>References</summary>
<ul>
<li><a href="https://calif.io/research/weworm">WeWorm | Calif</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">&quot;Zero-click&quot; WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/09/08/wechat-weworm-vulnerability-exploit-account-hijacking/">&quot;Zero-click&quot; WeChat worm could hijack accounts and spread via a single call - Help Net Security</a></li>
<li><a href="https://cybersecuritynews.com/weworm-first-0-click-worm/">WeWorm - First 0-Click Worm Spreading Through WeChat Calls Across iOS and Android</a></li>
<li><a href="https://www.theregister.com/security/2026/09/09/wechat-worm-could-pwn-a-friend-before-they-even-answered-the-call/5295234">WeChat worm could pwn a friend before they even answered the call</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#zero-click exploit`, `#WeChat`, `#remote code execution`, `#mobile worm`

---

<a id="item-tech-news-2"></a>
### [Shopify moves mobile app from React Native back to Swift and Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify&\#x27;s engineering team has published an account of moving its mobile app from React Native back to native Swift and Kotlin. The change is notable because a major commerce company is reversing a cross-platform choice in favor of separate native iOS and Android codebases, a decision that bears on how mobile teams weigh development speed, platform fidelity, and long-term maintenance. The supplied material does not include specific migration scope, performance benchmarks, version numbers, or timelines, so those details remain unverified here. The item drew substantial discussion on Hacker News, where commenters debated when cross-platform frameworks make sense and how AI-assisted code generation may change the calculus.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**「Background」** Shopify&\#x27;s mobile strategy has moved between cross-platform and native approaches. In 2020, Shopify adopted React Native to avoid building features twice and to let developers work across stacks, and in January 2025 the team published &quot;Five years of React Native at Shopify,&quot; reaffirming its investment in the framework. The current reversal to separate Swift and Kotlin codebases is attributed to coding agents reducing the cost of building, translating, testing, reviewing, and maintaining two native platforms.

**「Impact」** For mobile teams evaluating React Native against fully native development, Shopify’s public reversal provides a high-profile case study, though the supplied material does not include the migration’s technical metrics or timelines.

**「Community Discussion」** Commenters largely framed the choice as a resource-dependent engineering decision rather than a universal verdict, with one saying companies fall on a spectrum and another arguing that React Native’s main appeal—letting web developers build mobile apps—matters less as native code generation improves. Several shared practical migration experience: one reported moving a roughly 15–20 screen app from React Native to native using Codex and Maestro, getting about 90% working overnight before a few days of polish, while another commenter objected to being pushed toward Shopify’s app for package tracking.

<details><summary>References</summary>
<ul>
<li><a href="https://shopify.engineering/back-to-native">Native is now the future of mobile at Shopify (2026) - Shopify</a></li>
<li><a href="https://dev.to/jamilxt/shopify-is-moving-its-mobile-apps-back-to-native-coding-agents-made-it-cheaper-to-build-twice-than-4bf9">Shopify Is Moving Its Mobile Apps Back to Native. Coding ...</a></li>
<li><a href="https://picx.dev/news/LsT33N">Shopify moves from React Native back to native Swift and ...</a></li>

</ul>
</details>

**Tags**: `#React Native`, `#Swift`, `#Kotlin`, `#mobile development`, `#cross-platform engineering`

---

<a id="item-tech-news-3"></a>
### [Rust Is Now a Tier-1 Language at Microsoft](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 8.0/10

Microsoft has made Rust a tier-1 language, according to a Rust Foundation guest post. The move signals expanded first-class support for Rust in Microsoft&\#x27;s systems programming ecosystem and marks an important industry signal from a major OS and toolchain vendor. Community discussion has focused on memory safety, MSVC integration, and C/C++ migration, including claims about replacing LLVM with MSVC&\#x27;s backend and automating large-scale C-to-Rust conversion. The designation is significant because it could accelerate Rust adoption for greenfield systems development and improve its integration with Microsoft&\#x27;s toolchain.

hackernews · mmastrac · Sep 10, 13:39 · [Discussion](https://news.ycombinator.com/item?id=49643546)

**「Background」** Microsoft sorts programming languages into support tiers that determine how much tooling, compliance, and engineering investment they receive for production software, which must pass extensive security and quality workflows. Promoting Rust to Tier-1 means the company now treats it as a first-class language for systems development, a notable shift for a vendor whose stack has long centered on C++ and C\# — C++ still dominates Microsoft&\#x27;s codebases after decades of accumulated development. Rust&\#x27;s memory-safety guarantees are the main motivation for the change, though adoption inside the company remains uneven; developers report that Rust is still not widely used in large Microsoft C++ projects such as Azure Storage, partly because cross-language interoperability was complicated when last attempted.

**「Impact」** Microsoft engineering teams and Rust developers building for Windows gain first-class toolchain support, with the discussed MSVC backend integration being the change most likely to affect how Rust code is compiled and linked on that platform. The broader ambition of removing Microsoft&\#x27;s C and C++ codebase by 2030 remains an internal target rather than a committed deliverable.

**「Community Discussion」** Commenters largely welcomed the news as evidence that Rust is a mature competitor to C++ and C\#; one contrasted it favorably with newer &quot;better C/C++&quot; languages like Zig and Odin, while another flagged the MSVC backend replacing LLVM as the headline detail. The thread also cited Microsoft&\#x27;s reported goal to convert 1 billion lines of code to Rust by 2030 with automated tooling enabling &quot;1 engineer, 1 month, 1 million lines of code,&quot; DARPA work on C-to-Rust conversion across six teams, and a RustCon talk by Azure CTO Mark Russinovich stating that 70% of CVEs are memory-safety issues.

<details><summary>References</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://qatrial.com/developer-open-source/rust-is-tier-1-language-at-microsoft/">Rust Is Tier-1 Language At Microsoft - QAtrial</a></li>
<li><a href="https://lobste.rs/s/eerwba/rust_is_tier_1_language_at_microsoft">Rust Is Tier-1 Language at Microsoft | Lobsters</a></li>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier-1 Language at Microsoft</a></li>
<li><a href="https://www.theregister.com/software/2025/12/24/microsoft-wants-to-replace-its-entire-c-and-c-codebase/2339230">Microsoft wants to replace its entire C and C++ codebase</a></li>

</ul>
</details>

**Tags**: `#Rust`, `#Microsoft`, `#systems programming`, `#memory safety`, `#programming languages`

---

<a id="item-tech-news-4"></a>
### [Ant International, Visa and Mastercard to Build AI-Agent Payment Standard](https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html) ⭐️ 8.0/10

Ant International announced it is partnering with Visa and Mastercard to develop a common standard for AI-agent payments. The three parties plan to establish a &quot;Know Your Agent&quot; mechanism that links agents to valid entities, evaluates their behavior and monitors risk, with the goal of improving interoperability and security across different payment systems. They cited a McKinsey forecast that AI agents could handle $3 trillion to $5 trillion of global consumer commerce transactions by 2030. The announcement, reported by CNBC, is a brief statement without technical specifications or independent verification, so the framework&\#x27;s concrete requirements and timeline remain undefined.

telegram · zaihuapd · Sep 10, 03:00

**「Background」** AI-agent payments involve autonomous software agents that initiate or complete transactions on behalf of users or businesses, which existing payment controls built around human customers and merchants do not directly cover. The &quot;Know Your Agent&quot; framework from Ant International, Visa and Mastercard is intended to link each agent to a valid entity, assess and monitor its behavior, and allow an agent registered with one participating payment provider to avoid re-registering with the others \(tool-1-1, tool-1-2, tool-1-3\). The three companies cite a McKinsey forecast that AI agents could handle $3 trillion to $5 trillion of global consumer commerce by 2030.

**「Impact」** If adopted, the shared &quot;Know Your Agent&quot; framework would give merchants, payment networks, and AI-agent developers a common way to link agents to valid legal entities and assess risk across Ant International, Visa, and Mastercard rails, reducing the need for separate per-platform integrations. The announcement supplies no timeline, technical specification, or governance structure, so whether the standard is widely implemented — and whether agentic commerce reaches the $3T–$5T by 2030 that the three parties cite from McKinsey — remains unverified; McKinsey&\#x27;s own published estimates focus on roughly $1T in US agentic retail revenue by 2030.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/10/ant-international-visa-mastercard-ai-agent-payment-standard.html">Ant International, Visa and Mastercard team up on AI payment standard</a></li>
<li><a href="https://crypto.news/ant-international-joins-visa-mastercard-to-build-ai-agent-payment-standards/">Ant International joins Visa, Mastercard to build AI agent payment standards</a></li>
<li><a href="https://bitcoinethereumnews.com/tech/ai-agent-payment-standards-set-by-visa-mastercard-ant/">AI Agent Payment Standards Set by Visa, Mastercard, Ant</a></li>
<li><a href="https://www.digitalcommerce360.com/2025/10/20/mckinsey-forecast-5-trillion-agentic-commerce-sales-2030/">McKinsey : Up to $5 trillion in agentic commerce sales by 2030</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#payment standards`, `#fintech`, `#interoperability`, `#risk management`

---

<a id="item-tech-news-5"></a>
### [DeepSeek releases V4.1 Flash: 552B multimodal model with API pricing changes](https://mp.weixin.qq.com/s/qg0NU3NNUbp1co2PdkAPAg) ⭐️ 7.0/10

DeepSeek announced V4.1 Flash, described as the smallest model in a new model-architecture series, built on a 552B-parameter Causal-Encoder-Decoder design with 8B input and 16B output activations and native support for multimodal visual understanding. The model is already available through the DeepSeek API under the model name deepseek-flash. New pricing takes effect on September 10, 2026 at 12:00, and after September 14, 2026 at 12:00 requests to deepseek-v4-pro will be routed to V4.1 Flash and billed at its pricing. The announcement is a brief promotional release and does not include benchmarks, a technical paper, or independent confirmation, so the claimed performance and efficiency advantages remain unverified.

telegram · zaihuapd · Sep 10, 05:54

**「Background」** DeepSeek is a Chinese AI lab that ships both open-weight and API-served models; V4-Pro is the flagship of its current V4 line, and V4.1 Flash is positioned as the smallest member of a new &quot;Causal Encoder–Decoder&quot; architecture family. That architecture label describes a decoder-style generative model whose input and output stages carry different activation budgets — roughly 8B active parameters for input \(prefill\) and 16B for output \(decode\) — rather than a conventional dense or uniformly sparse setup. Third-party write-ups describe the 552B backbone as a mixture-of-experts model with image-and-text input and a 1M-token context window, while DeepSeek attributes the model&\#x27;s standing relative to earlier flagships such as V4-Pro to new pretraining methods plus larger-scale RL post-training.

**「Impact」** Developers and applications calling deepseek-v4-pro will have those requests automatically routed to V4.1 Flash and billed at Flash-series rates from 12:00 Beijing time on September 14, 2026, until a future V4.1 Pro release, so existing integrations will change underlying model and cost without any code change.

<details><summary>References</summary>
<ul>
<li><a href="https://www.deepseek.com/en/news/deepseek-v4-1-flash/">DeepSeek | Introducing DeepSeek-V4.1-Flash: smarter, faster, more efficient.</a></li>
<li><a href="https://www.progressiverobot.com/2026/09/10/deepseek-v4-1-flash-552b-moe-model-hugging-face/">DeepSeek V4.1 Flash: Powerful 552B MoE at a Surprising Price</a></li>
<li><a href="https://benchlm.ai/models/deepseek-v4-1-flash">DeepSeek V4.1 Flash Benchmarks &amp; Pricing (September 2026)</a></li>
<li><a href="https://api-docs.deepseek.com/quick_start/pricing/">Models &amp; Pricing | DeepSeek API Docs</a></li>
<li><a href="https://technode.com/2026/09/10/deepseek-formally-launches-v4-1-flash-routes-v4-pro-requests-to-flash/">DeepSeek formally launches V4.1 Flash, routes V4 Pro requests to Flash · TechNode</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#large language models`, `#multimodal AI`, `#model release`, `#API pricing`

---

<a id="item-tech-news-6"></a>
### [Tencent Hunyuan Releases Open-Source Audio Editing Model AuK](https://x.com/TencentHunyuan/status/2097996926876795197) ⭐️ 7.0/10

Tencent Hunyuan has officially released AuK, an open-source audio editing model that uses natural-language instructions and reference audio to unify speech generation and editing. The model supports zero-shot text-to-speech, timbre/style/emotion editing, accent removal, and multi-speaker speech separation. Tencent also released AuK-Flash, a variant that uses 4-step inference and is claimed to be about 4.5x faster under matched conditions. Code, model weights, and demos are available, though the announcement does not provide benchmarks, model sizes, or license details.

telegram · zaihuapd · Sep 10, 11:56

**「Background」** Unified speech generation and editing systems aim to combine synthesis and modification in a single model instead of separate pipelines; AuK takes natural-language instructions together with reference audio, covering zero-shot text-to-speech, timbre/style/emotion editing, accent removal, and multi-speaker separation. AuK-Flash is a companion variant that runs inference in 4 steps, a common way to reduce generation latency at some cost to quality. Tencent Hunyuan is Tencent&\#x27;s AI model family, which has also recently released open-source speech models such as the Hy ASR 3.0 preview.

**「Impact」** Developers and audio practitioners gain a permissively MIT-licensed 1.5B speech foundation model they can run or fine-tune locally for instruction-based TTS, content and acoustic editing, enhancement, and source separation, with the 4-step AuK-Flash variant lowering inference cost for latency-sensitive deployments. The practical speedup, however, is only claimed under matching conditions, since the announcement provides no benchmarks or independent measurements.

<details><summary>References</summary>
<ul>
<li><a href="https://www.woshipm.com/ai/6441202.html">AI互联网日报：Qwen-Image-3.0降到0.18...</a></li>
<li><a href="https://huggingface.co/tencent/AuK-Flash">tencent/AuK-Flash · Hugging Face</a></li>
<li><a href="https://github.com/Tencent-Hunyuan/AuK">GitHub - Tencent-Hunyuan/AuK: AuK: An Open-Source ...</a></li>
<li><a href="https://ai-tldr.dev/models/auk/">AuK — Tencent&#x27;s Open Speech Generation Model | AI/TLDR</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#audio-editing`, `#text-to-speech`, `#speech-editing`, `#Tencent-Hunyuan`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Following the Bottleneck: MiniMax M3 on AMD MI355X](https://vllm.ai/blog/2026-09-10-minimax-m3-mi355x) ⭐️ 9.0/10

rss · vLLM Blog · Sep 10, 00:00

**「Background」** MiniMax M3&\#x27;s day-0 vLLM implementation on AMD Instinct MI355X was functional but slow: 109.1 output tokens/s/GPU at concurrency 32 with MXFP8 under a fixed TP4/EP1 topology. The follow-up asks what to optimize next when the bottleneck keeps moving across 60 decoder layers, 57 of which use sparse MoE and sparse attention.

**「Solution」** The team&\#x27;s method was to change the level of the question after each win, and the results were cumulative: 342.4 output tok/s/GPU at concurrency 32 \(3.14x day-0\) and 623.7 at concurrency 128 \(2.09x\), with MXFP4 later reaching 943.5 on TP2/EP1 and P/D disaggregation reaching 6,370.5 total tok/s/GPU at concurrency 512 with 1.32 s median TTFT. First they tuned for local shapes after sharding: at TP8, replicated KV and index heads make the fused QKV projection see local N=1536, so vLLM \#45725 split launchers into large-M and small-M regimes and \#46117 picked tiles from the real shape, yielding 1.08-1.46x in TP4 tests, with AITER sparse attention requiring one KV head per rank \(legal at TP4, falling back to Triton at TP2\). Next they batched repeated work: \#46545 appended the shared expert to the routed expert table and ran both through the same grouped GEMMs, improving throughput 30.2% at concurrency 1 but only 5.6% at 128, while \#45743 batched the MSA indexer per request \(48.9% kernel gain, ~3.3% end-to-end\). Then they moved metadata rather than bytes: \#47269 shared top-k block decisions across sparse layers for ~10% TPOT improvement at concurrency 1, \#47287 compiled away the unused index producer branch and turned each selected 128-token block into eight 16-token AITER pages instead of copying KV. An audit also caught an attribution error: a 1.5 MB collective was configured for INT4 QuickReduce but never met the 16 MB eligibility gate, so its curve was reclassified as a cumulative checkpoint; similarly, correctness fixes such as FP8 KV views on FNUZ ROCm \(GSM8K 0.0099 to 0.9575\) and an EP mask \(cosine similarity 0.527 to 1.0\) exposed contracts rather than speedups. EAGLE3 required its own decode loop fixes, including a cache-key bug from differing query-head counts, and reached 682.4 tok/s/GPU; P/D needed per-layer transfer geometry, sealed write counts, and heterogeneous-TP acknowledgments before tuning the 2:1 prefill/decode ratio, trading higher mean TPOT \(31.26 to 54.60 ms\) for a cleared prompt queue.

**「Takeaway」** The author&\#x27;s conclusion is that sustained serving speedups come from repeatedly re-profiling and changing the level of the bottleneck question, from tiles to repeated paths to sparse metadata to distributed state to workload queues, with a correctness gate beside every performance gate. The first AgentX run, at 127.4 output tok/s/GPU with a 92.1% realized vs 96.7% theoretical cache hit rate, suggests the next gains lie in prefix alignment, scheduling, and cache policy rather than another GEMM.

**Tags**: `#LLM inference optimization`, `#AMD Instinct MI355X`, `#vLLM`, `#sparse attention/MoE`, `#performance profiling`

---

<a id="item-tech-blog-2"></a>
### [vLLM&\#x27;s Tiered KV Cache Offloading via Host Memory](https://vllm.ai/blog/2026-09-10-tiered-kv-offloading) ⭐️ 8.0/10

rss · vLLM Blog · Sep 10, 00:00

**「Background」** Long-context models and multi-turn conversations build massive KV caches; when accelerator HBM fills, vLLM evicts that data and must recompute it from scratch on a later request, wasting compute and inflating latency. Tiered KV cache offloading, available in vLLM since v0.22, preserves evicted KV data in host memory and lower tiers instead.

**「Solution」** The framework&\#x27;s core design choice, per the authors, is that all KV data flows through host memory: offload copies accelerator data to host DRAM via async DMA, freeing accelerator memory before any secondary transfer begins, and reload allocates accelerator memory only once data is ready in host — a just-in-time pattern. Tensor-parallel shards are consolidated into one shared host region under a canonical layout \(one page per block per layer, all KV heads gathered\), so nodes with different TP sizes, attention backends \(FlashAttention, FlashInfer, Triton\), or accelerator types produce identical chunks and can share data with no remapping. Host memory is a real LRU/ARC cache, not a staging buffer: the scheduler checks it first, and on a miss queries secondary tiers in configured order, promoting the chunk asynchronously while receiving a RETRY. Secondary tiers are single processes using CPU libraries — filesystem \(content-addressed, atomic writes, separate read/write pools\), S3-compatible object storage via NIXL, and peer-to-peer sharing over ZMQ plus RDMA, where an orchestrator such as llm-d picks peers for prefill/decode disaggregation or load balancing. The canonical layout also normalizes hybrid layer types \(full attention, sliding window, MLA, Mamba\) into uniform byte buffers. In the authors&\#x27; benchmark \(Qwen3.6-35B-A3B, 2×H100, TP=2, local NVMe storage tier, 12K-token prompts, 8 rounds, concurrency 64\), HBM holds the working set up to roughly 64 conversations; at 64–128 CPU offload sustains throughput; beyond 128, storage offload more than doubles throughput versus alternatives, though storage latency keeps it below peak. Out-of-tree tiers need only four methods, and Prometheus metrics plus KV events expose per-tier hit rates and locality to orchestration systems.

**「Takeaway」** By routing every transfer through host memory and normalizing the layout, vLLM turns KV cache tiering into an ordinary CPU-side caching problem that scales horizontally and accepts arbitrary backends. At scale, the authors argue, a storage-backed cache hit decisively beats a full recompute.

**Tags**: `#KV cache offloading`, `#vLLM`, `#LLM inference serving`, `#memory tiering`, `#prefill-decode disaggregation`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Kalshi launches ‘perps’ for gold and silver following CFTC approval, expanding futures offerings](https://www.cnbc.com/2026/09/10/kalshi-launches-perps-for-gold-and-silver-following-cftc-approval-expanding-futures-offerings.html) ⭐️ 7.0/10

Kalshi won CFTC approval and launched perpetual futures on gold and silver, expanding its regulated derivatives offerings beyond crypto and prediction markets.

rss · CNBC Finance · Sep 10, 14:00

**Tags**: `#Kalshi`, `#perpetual futures`, `#CFTC`, `#gold and silver`, `#derivatives regulation`

---

<a id="item-finance-news-2"></a>
### [China AI chipmakers raise prices as HBM shortage bites](https://www.reuters.com/world/asia-pacific/chinas-ai-chipmakers-raise-prices-high-bandwidth-memory-shortage-bites-2026-09-10/) ⭐️ 7.0/10

A global shortage of high-bandwidth memory \(HBM\) — the fast memory stacked next to AI processors — is pushing Chinese AI chipmakers including Huawei and Cambricon to raise prices, according to a Reuters report. Huawei&\#x27;s Ascend 950DT chip is quoted about 20%–50% higher than two months ago, with some older chips up roughly 30%, while Cambricon&\#x27;s new SiYuan 690 is expected to cost about 20%–30% more.

telegram · zaihuapd · Sep 10, 09:29

**「Background」** High-bandwidth memory \(HBM\) is a specialised memory stacked alongside AI processors to feed them data quickly, and it is supplied mainly by SK Hynix, Samsung and Micron, with U.S. export controls further restricting Chinese firms&\#x27; access to advanced chips. Huawei and Cambricon had filled the gap those controls left in China&\#x27;s AI chip market, and the HBM shortage now limits how far that domestic expansion can go.

**「Who is affected」** Chinese AI and cloud companies buying domestic chips — Huawei&\#x27;s Ascend and Cambricon&\#x27;s Siyuan lines — face a higher cost for each unit of AI computing capacity, because the HBM shortage both raises chip prices and limits how many chips suppliers can build.

<details><summary>References</summary>
<ul>
<li><a href="https://www.msn.com/en-us/technology/hardware-and-devices/china-ai-chipmakers-raise-prices-amid-hbm-shortage/vi-AA2bXQwL">China AI chipmakers raise prices amid HBM shortage</a></li>
<li><a href="https://money.usnews.com/investing/news/articles/2026-09-10/exclusive-chinas-ai-chipmakers-raise-prices-as-high-bandwidth-memory-shortage-bites">Exclusive- China &#x27;s AI Chipmakers Raise Prices as High-Bandwidth...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/exclusive-chinas-ai-chipmakers-raise-050223278.html?fr=sycsrp_catchall">Exclusive-China&#x27;s AI chipmakers raise prices as high ...</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/chinas-ai-chipmakers-raise-prices-high-bandwidth-memory-shortage-bites-2026-09-10/">EXCLUSIVE: China&#x27;s AI chipmakers raise prices as high ...</a></li>
<li><a href="https://moderndiplomacy.eu/2026/09/10/china-ai-chips-hbm-shortage-prices/">China’s AI Chipmakers Raise Prices as HBM Shortage Squeezes ...</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#HBM`, `#China semiconductors`, `#export controls`, `#pricing`

---