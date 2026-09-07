---
layout: default
title: "Horizon Summary: 2026-09-07 (EN)"
date: 2026-09-07
lang: en
---

> From 34 items, 9 important content pieces were selected

---

**Technology News**
1. [LLM-guided program evolution improves 10 circle-packing records](#item-tech-news-1) ⭐️ 8.0/10
2. [LG Smart TVs&\#x27; 216M Audio-Logging Privacy Problem](#item-tech-news-2) ⭐️ 7.0/10
3. [TPU Inference Externalization Advances via InferenceX and Ironwood](#item-tech-news-3) ⭐️ 7.0/10
4. [Rustuna: Rust-based Optuna-Compatible Hyperparameter Optimization](#item-tech-news-4) ⭐️ 7.0/10
5. [Yandex Team Proposes KV Cache as Agent Runtime for Interactive LLMs](#item-tech-news-5) ⭐️ 7.0/10
6. [Huawei Releases Kirin 9050 Pro, Its First Flagship Chip in Six Years](#item-tech-news-6) ⭐️ 7.0/10
7. [China&\#x27;s Top Court Clarifies AI Civil Liability in New Rules](#item-tech-news-7) ⭐️ 7.0/10

**Technology Blog**
1. [Inside Tenstorrent&\#x27;s vLLM Plugin for Mesh Hardware](#item-tech-blog-1) ⭐️ 8.0/10

**Financial News**
1. [China to Inject $54 Billion into Three State Banks and Five Insurers](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [LLM-guided program evolution improves 10 circle-packing records](https://www.reddit.com/r/MachineLearning/comments/1w9xlyi/llmguided_program_evolution_improves_10_bestknown/) ⭐️ 8.0/10

A Reddit post describes an LLM-guided program-evolution method that improved 10 best-known sum-of-radii solutions on the Packomania csqv circle-packing benchmark, for N=101-114, with relative gains of 2.4-5.4% after 15 iterations. The loop starts from a simple seed solver; an LLM proposes algorithmic changes informed by a scoreboard and failure history, and an independent verifier scores each candidate to retain only improvements. Packomania independently accepted the results, and the post links to the paper, code, solutions, and benchmark. The reported total LLM cost was $27.72.

reddit · r/MachineLearning · /u/SIGH\_I\_CALL · Sep 7, 16:54

**「Background」** The Packomania csqv benchmark asks how to arrange N variable-radius circles inside a unit square to maximize the sum of their radii, and researchers have long competed to improve recorded best-known solutions. LLM-guided program evolution is an emerging technique in which an LLM repeatedly proposes changes to an optimization algorithm, each candidate is executed and scored by an independent verifier, and only successful modifications are retained; this automates algorithmic discovery without relying on the model to directly compute circle coordinates. In this work, the method was applied to csqv instances for N ranging from 101 to 114, which explains why the reported results target relatively large packing problems.

**「Impact」** For researchers and practitioners using circle-packing or benchmark-driven optimization, the accepted solutions establish new best-known values on Packomania csqv for those instances and show that LLM-driven algorithm evolution can be a low-cost alternative to hand-designed solvers.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.05093">[2609.05093] LLM - Guided Program Evolution for Circle Packing ...</a></li>
<li><a href="https://arxiv.org/html/2609.05093">LLM - Guided Program Evolution for Circle Packing :Breaking 10...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#program evolution`, `#optimization`, `#circle-packing`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [LG Smart TVs&\#x27; 216M Audio-Logging Privacy Problem](https://www.youtube.com/watch?v=6IFVTcM28KA) ⭐️ 7.0/10

A widely shared video and its linked NotebookCheck article report that LG Smart TVs engage in invasive data collection at massive scale, involving roughly 216 million devices. The coverage says the television sets log audio even while the screen is off and actively snoop on other local devices connected to the home network, beyond ordinary fingerprinting. LG&\#x27;s appliance contract terms reportedly require owners to notify household members and guests that their voices may be captured and processed, and to obtain all necessary consents from third parties. The situation matters because millions of owners may have accepted these terms unknowingly, and the practices create privacy and potential wiretap-law concerns for anyone in range of an LG TV.

hackernews · treve · Sep 7, 00:22 · [Discussion](https://news.ycombinator.com/item?id=49592375)

**「Background」** Smart TVs often collect viewing and usage data to support advertising and connected services, but investigations have repeatedly raised concerns that some collection exceeds what consumers expect. In this case, an investigation by Gamers Nexus found that LG smart TVs sweep local networks to map phones and nearby devices and can capture microphone audio even when the screen is off; the data is then uploaded once the TV reconnects to the internet. LG&\#x27;s own terms require users to obtain consent from third parties whose voices may be captured, underscoring the privacy and legal stakes for anyone near these devices.

**「Impact」** For LG Smart TV owners, the concrete consequence is a difficult practical choice: accept invasive data collection, warn and obtain consent from every guest who could be overheard, or disable network features and smart functionality entirely to protect privacy.

**「Community Discussion」** Commenters largely agree the behavior is unacceptable, with some reporting that they declined LG&\#x27;s terms, disabled all network functions, or physically unplugged the Wi-Fi/BT chip in their LG OLEDs; others point out that all-party wiretap laws could make both LG and device owners liable if guests are recorded without consent.

<details><summary>References</summary>
<ul>
<li><a href="https://www.notebookcheck.net/LG-smart-TVs-caught-logging-audio-with-screen-off-and-snooping-on-local-devices.1391214.0.html">LG smart TVs caught logging audio with screen off and snooping ...</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#smart-tv`, `#security`, `#IoT`, `#LG`

---

<a id="item-tech-news-3"></a>
### [TPU Inference Externalization Advances via InferenceX and Ironwood](https://newsletter.semianalysis.com/p/tpu-inferencex-full-steam) ⭐️ 7.0/10

SemiAnalysis reports that Google’s TPU stack is rapidly being externalized for AI inference under the InferenceX initiative, with claims of up to 50% better performance per dollar and a growing customer base. The item highlights Ironwood, also referred to as TPUv8i, as part of this push. The report positions TPU inference externalization as a growing competitive factor that could reduce NVIDIA’s CUDA moat. The snippet provides limited concrete implementation details, so the reported gains and timeline remain early-stage signals.

rss · Semianalysis · Sep 7, 20:00

**「Background」** Google has developed custom Tensor Processing Units \(TPUs\) for years, offering them through Google Cloud and using them internally for models such as Gemini. The eighth generation reportedly splits duties, with the TPUv8 ax &quot;Sunfish&quot; aimed at training and the TPUv8 x &quot;Zebrafish&quot; at large-scale inference; other reports describe TPUv8t and TPUv8i variants replacing the TPUv7 &quot;Ironwood&quot; lineup available since 2025. In this context, &quot;externalization&quot; refers to making Google&\#x27;s TPU stack more broadly accessible to external customers for AI inference workloads. Because Nvidia&\#x27;s CUDA software ecosystem remains a key advantage for its GPUs, competitive efforts to reduce that CUDA moat are part of the broader market backdrop.

**「Impact」** For Google Cloud customers, the InferenceX push—claiming up to 50% better performance per dollar on Ironwood/TPUv8i—could make TPUs a more cost-effective inference alternative to Nvidia and erode CUDA&\#x27;s ecosystem moat, but supply constraints and the structural difficulty of building a developer ecosystem may limit how fast externalization pays off.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techpowerup.com/343957/google-prepares-tpuv8ax-for-training-and-tpuv8x-for-inference">Google Prepares TPUv 8 ax for Training and... | TechPowerUp</a></li>
<li><a href="https://wccftech.com/google-splits-tpuv8-strategy-two-chips-broadcom-training-mediatek-inference-duties/">Google Splits TPUv 8 Strategy Into Two Chips, Handing Broadcom...</a></li>
<li><a href="https://newsletter.semianalysis.com/p/tpuv7-google-takes-a-swing-at-the">Google TPUv7: The 900lb Gorilla In the Room</a></li>
<li><a href="https://www.youtube.com/watch?v=p-6ZBuOEr4c">Why Google &#x27;s Chip Was Never the Problem: The... - YouTube</a></li>
<li><a href="https://fourweekmba.com/ai-google-tpu-selling-renting-compute-alphabet-q2-2026/">Google Is Selling TPUs and Renting Outside... - FourWeekMBA</a></li>

</ul>
</details>

**Tags**: `#TPU`, `#AI inference`, `#hardware`, `#Google Cloud`, `#CUDA`

---

<a id="item-tech-news-4"></a>
### [Rustuna: Rust-based Optuna-Compatible Hyperparameter Optimization](https://www.reddit.com/r/MachineLearning/comments/1w9nyhz/rustuna_a_highperformance_rust_implementation_of/) ⭐️ 7.0/10

Rustuna is a newly released, open-source implementation of the Optuna hyperparameter optimization framework, written in Rust and available at github.com/optuna/rustuna. It preserves Optuna&\#x27;s familiar API and core concepts while using Rust&\#x27;s native memory management to achieve lower memory usage and high speed. The library is designed with zero Python dependencies, which the developers say mitigates the risk of supply chain attacks. This release, announced on Reddit by u/c-bata with a Medium blog post, gives Rust users an Optuna-compatible optimization workflow without requiring a Python runtime.

reddit · r/MachineLearning · /u/c-bata · Sep 7, 10:01

**「Background」** Optuna is a widely used Python-based hyperparameter optimization framework that helps machine learning engineers and researchers efficiently search model parameters. Rustuna aims to bring the same study, trial, and suggestion concepts to the Rust ecosystem, offering an alternative for teams that want to avoid Python dependencies or optimize memory overhead while keeping a familiar API.

**「Impact」** The most concrete consequence is that Rust developers can now adopt an Optuna-compatible hyperparameter optimizer directly in Rust without installing Python or relying on Python package dependencies, potentially reducing supply-chain exposure and memory footprint for optimization tasks. However, this is a new library announcement, so its practical performance and stability have yet to be independently validated.

**Tags**: `#rust`, `#optuna`, `#hyperparameter-optimization`, `#machine-learning`, `#performance`

---

<a id="item-tech-news-5"></a>
### [Yandex Team Proposes KV Cache as Agent Runtime for Interactive LLMs](https://www.reddit.com/r/MachineLearning/comments/1w9myqc/kv_cache_as_an_agent_runtime_r/) ⭐️ 7.0/10

A Yandex research team proposes treating the KV cache—the model&\#x27;s inference state—as an agent runtime to make LLM systems more interactive and responsive. This approach involves modifying the KV cache during inference and has been used in the lab&\#x27;s earlier papers Hogwild\! Inference and AsyncReasoning. The accompanying blog post previews future work in which a Qwen3.8-27B agent plays a DOOM environment interactively using similar techniques. The authors suggest that model inference and runtime design may be an under-explored axis of agent capabilities, distinct from model choice and agent harness design. The Reddit submission itself contains no detailed methodology or independent evaluation.

reddit · r/MachineLearning · /u/\_puhsu · Sep 7, 09:03

**「Background」** The KV \(key-value\) cache is the memory of attention key and value vectors that transformer-based LLMs maintain during inference, avoiding recomputation of earlier context for each new token. Yandex Research&\#x27;s prior work, including the AsyncReasoning project, explored modifying or reusing this inference state to enable asynchronous, more responsive decoding. This post builds on that idea by framing the KV cache itself as a controllable agent runtime, positioned between higher-level harness design and expensive full model retraining.

**「Impact」** This proposal could encourage ML researchers and agent builders to explore runtime-level KV-cache manipulation as a practical middle ground between costly model changes and abstract harness design, potentially enabling more responsive interactive LLM systems.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/yandex-research/AsyncReasoning">GitHub - yandex-research/AsyncReasoning · GitHub</a></li>

</ul>
</details>

**Tags**: `#kv-cache`, `#llm-agents`, `#inference`, `#machine-learning`, `#interactive-ai`

---

<a id="item-tech-news-6"></a>
### [Huawei Releases Kirin 9050 Pro, Its First Flagship Chip in Six Years](https://www.news.cn/20260907/adf46c5c003240d28cc3cf6de54f9b5f/c.html) ⭐️ 7.0/10

Huawei unveiled the Mate XT 2 tri-fold phone in Guangzhou, powered by the new Kirin 9050 Pro chip, its first new flagship Kirin processor in six years since the Mate 40&\#x27;s global launch. According to the Xinhua report, the Kirin 9050 Pro is the first high-performance chip to employ logic-folding technology, arranging logic units in stacked layers within a single chip rather than a single plane. It adds vertical interconnect channels, described as elevators, which shorten signal-transmission paths, lower latency, and improve performance. The launch marks Huawei&\#x27;s return to introducing a brand-new Kirin chip at a flagship event after a six-year gap.

telegram · zaihuapd · Sep 7, 08:20

**「Background」** Huawei&\#x27;s previous flagship Kirin chip was the Kirin 9000 series introduced with the Mate 40 lineup in 2020; since then, U.S. sanctions restricted Huawei&\#x27;s access to advanced chip manufacturing and it did not release a new flagship Kirin processor at subsequent flagship events. The Mate XT 2 launch, hosted by Huawei&\#x27;s Yu Chengdong at a HarmonyOS 7 and new-device event, marks the first time in six years that Huawei has introduced a new flagship Kirin chip, the Kirin 9050 Pro.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/0/999/300.htm">华为继 Mate 40 后时隔六年再次发布高性能芯片，麒麟 9050 Pro 首发逻辑折叠技术 - IT之家</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#hardware`, `#Huawei`, `#chip-design`, `#mobile`

---

<a id="item-tech-news-7"></a>
### [China&\#x27;s Top Court Clarifies AI Civil Liability in New Rules](https://www.cnr.cn/news/20260907/t20260907_527806795.shtml) ⭐️ 7.0/10

China&\#x27;s Supreme People&\#x27;s Court published a judicial interpretation on September 7 that clarifies civil liability in artificial intelligence disputes. The interpretation contains 24 articles in five parts and addresses AI face-swapping, algorithmic price discrimination, impersonation endorsements, autonomous driving, and intellectual property. It states that creating recognizable faces or voices with AI without consent may constitute personality rights infringement, algorithmic price discrimination that harms rights and interests can trigger liability, and AI impersonation that induces consumers may support punitive damages claims. It also says AI-enabled “cyber doxxing” and “human flesh search” that violate privacy rights will be regulated under the interpretation. The document provides more concrete legal criteria for AI-related civil litigation in China.

telegram · zaihuapd · Sep 7, 09:32

**「Background」** Judicial interpretations from the Supreme People&\#x27;s Court are binding explanations of how Chinese courts should apply existing laws. This interpretation addresses a gap in China&\#x27;s legal framework by providing specific rules for emerging AI disputes, which previously relied on general personality, consumer, and privacy law.

**「Impact」** AI developers, online platforms, and commercial users in China now face clearer legal exposure for unauthorized face or voice synthesis, discriminatory algorithmic pricing, and fake endorsements, and individuals harmed by such practices can cite this interpretation when seeking damages.

**Tags**: `#AI regulation`, `#AI liability`, `#deepfake`, `#algorithmic pricing`, `#China law`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Inside Tenstorrent&\#x27;s vLLM Plugin for Mesh Hardware](https://vllm.ai/blog/2026-09-07-vllm-tt-plugin) ⭐️ 8.0/10

rss · vLLM Blog · Sep 7, 00:00

**「Background」** Tenstorrent accelerators are meshes of cores and chips whose programs are compiled and traced for the whole mesh, so they do not look like GPUs and cannot be expressed with vLLM&\#x27;s usual tensor-parallel ranks or host collectives. The authors introduce the vLLM TT Plugin, which brings Tenstorrent hardware into vLLM through its standard out-of-tree plugin mechanism without forking vLLM core.

**「Solution」** The plugin registers a Tenstorrent platform only when ttnn is importable, then swaps in custom worker and scheduler classes through existing extension points. Because traced execution rewards shape-stable batches, the scheduler admits either prefill-only or decode-only steps per device step, interleaving decode between chunked prefill chunks rather than mixing phases; the cost is whole-step granularity and drain of the overlap pipeline on each mode switch. For single-execute models on Galaxy, which have one program spanning the entire mesh but multiple internal DP submeshes, standard process data parallelism has nothing to partition, so the plugin uses in-process lane data parallelism: one coordinator merges per-lane scheduler outputs, builds a single device batch, and retries decode when KV pressure prevents a forced prefill step from admitting tokens. On-device sampling is used when the batch needs no logprobs or custom logits processors, with automatic per-batch fallback to host sampling for correctness. Async decode overlap is explicitly narrower than an async execution model: it is asynchronous host readback of steady-state traced steps, enabled only for models declaring support, while prefill remains synchronous in practice.

**「Takeaway」** The authors show that vLLM&\#x27;s V1 extension points, especially the pluggable scheduler, are general enough to express a phase-constrained, mesh-native execution model without core changes. They invite feedback on whether in-process lanes are the right user-facing surface for single-execute models and which model families to prioritize next.

**Tags**: `#vLLM`, `#Tenstorrent`, `#LLM inference`, `#hardware plugin`, `#scheduler design`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China to Inject $54 Billion into Three State Banks and Five Insurers](https://www.cnbc.com/2026/09/07/china-state-banks-lenders-insurers-capital-solvency-bankrupt-nim-.html) ⭐️ 7.0/10

China’s finance ministry and state institutions plan to inject a combined 360 billion yuan \(about $53.6 billion\) into three state banks and five insurers. Citibank said the package was smaller than markets had expected; Hong Kong-listed shares of the lenders and insurers fell Monday.

rss · CNBC Finance · Sep 7, 09:26

**「Background」** The move follows Beijing’s 500 billion yuan capital injection into four state banks last year and a 300 billion yuan special treasury bond pledge this year, as lenders face record-low net interest margins — the gap between loan income and deposit costs — and insurers’ solvency cushions have thinned.

**Tags**: `#China`, `#banking`, `#recapitalization`, `#financial policy`, `#insurers`

---