---
layout: default
title: "Horizon Summary: 2026-09-08 (EN)"
date: 2026-09-08
lang: en
---

> From 46 items, 10 important content pieces were selected

---

**Technology News**
1. [OpenAI Claims Navier-Stokes Millennium Problem Solution](#item-tech-news-1) ⭐️ 8.0/10
2. [NeurIPS desk-rejected 178 papers over flawed AI detector](#item-tech-news-2) ⭐️ 8.0/10
3. [Tim Cook Skips Apple September 9 Video as New CEO Leads Foldable iPhone Push](#item-tech-news-3) ⭐️ 8.0/10
4. [ASML and TSMC Map High NA EUV Shift to 12-Inch Photomasks](#item-tech-news-4) ⭐️ 7.0/10
5. [China plans fourfold AI compute boost to 9800 EFLOPS by 2030](#item-tech-news-5) ⭐️ 7.0/10
6. [OpenAI Rolls Out ChatGPT Images 2.5 with Lower Latency](#item-tech-news-6) ⭐️ 7.0/10

**Technology Blog**
1. [Hybrid HiSparse Offloading in vLLM for GLM 5.3](#item-tech-blog-1) ⭐️ 8.0/10
2. [Optimizing Real-World Agentic Serving with vLLM and AgentX](#item-tech-blog-2) ⭐️ 8.0/10

**Financial News**
1. [Crypto platforms lost $3.63 billion in cyberattacks, often despite security audits, CoinGecko says](#item-finance-news-1) ⭐️ 7.0/10
2. [China injects $53.6 billion into state banks and insurers in recapitalization plan](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [OpenAI Claims Navier-Stokes Millennium Problem Solution](https://www.reddit.com/r/MachineLearning/comments/1wavdi7/openal_says_it_has_cracked_one_of_maths/) ⭐️ 8.0/10

OpenAI says it has solved the Navier-Stokes existence and smoothness problem, one of the Clay Mathematics Institute&\#x27;s Millennium Prize Problems, according to a New York Times article and an OpenAI announcement linked in this Reddit post. No technical proof or evidence is included, and the result has not been independently confirmed. If the claim holds up, it would represent a historic breakthrough for AI-driven mathematics and for understanding fluid dynamics, with major implications for science and engineering. The AI/ML community is awaiting release of the full proof and independent verification.

reddit · r/MachineLearning · /u/Shizuka\_Kuze · Sep 8, 17:42

**「Background」** The Navier–Stokes existence and smoothness problem is one of the seven Millennium Prize Problems, each carrying a $1 million reward for a correct solution. It asks whether solutions to the Navier–Stokes equations, which describe fluid motion, always remain smooth or can develop singularities in finite time. OpenAI has announced that an internal, unreleased AI model produced a purported solution showing such singularities can form, reportedly after 88 hours of computation and about $15 million in AI effort, though the claim has not yet been independently verified by the mathematical community.

**「Impact」** If independently confirmed, OpenAI&\#x27;s AI-generated formal proof would make it the first announced solution to a Millennium Prize Problem produced by AI, and its Lean-checked writeup directly targets a problem open for over 90 years. However, the company states that its proposed resolution covers only two of the four statements required for Navier–Stokes existence and smoothness, so mathematicians still need to validate the argument before any prize or broad scientific impact follows.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/navier-stokes-solution/">On the Navier–Stokes Millennium Prize Problem | OpenAI</a></li>
<li><a href="https://www.nytimes.com/2026/09/08/science/openai-proof-millennium-problem.html">OpenAI Says It Has Cracked One of Math’s ‘Millennium Problems’ - The New York Times</a></li>
<li><a href="https://www.newscientist.com/article/2588063-openai-has-solved-the-navier-stokes-millennium-problem-using-15m-of-ai-effort/">OpenAI has solved the Navier-Stokes Millennium problem using $15m of AI effort | New Scientist</a></li>
<li><a href="https://openai.com/index/navier-stokes-solution/">On the Navier–Stokes Millennium Prize Problem | OpenAI</a></li>
<li><a href="https://www.bbc.com/news/articles/cy7zygy3rl2o">OpenAI says it cracked 90-year-old maths problem in 88 hours</a></li>
<li><a href="https://www.nature.com/articles/d41586-026-02842-5">OpenAI claims huge maths breakthrough on a famed ‘Millennium ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Navier-Stokes`, `#mathematics`, `#AI announcements`, `#research news`

---

<a id="item-tech-news-2"></a>
### [NeurIPS desk-rejected 178 papers over flawed AI detector](https://www.reddit.com/r/MachineLearning/comments/1wakf62/neurips_deskrejected_178_papers_for_being/) ⭐️ 8.0/10

NeurIPS&\#x27;s Position Paper Track used the proprietary AI detector Pangram to desk-reject 178 papers, or 18.4% of all submissions, with no human review or appeal process. Independent tests showed the same detector flagged recent papers by the three track chairs at 24% to 69%, meaning they would have been at risk under their own rules. Pangram&\#x27;s default setting originally flagged 42.7% of submissions as mostly AI-generated, and organizers adjusted text windows to bring the rate down to 12.7%. Twenty-two papers were rejected specifically because they scored above 0.5 while authors denied AI use, treating the black-box score as proof of dishonesty. A Stanford study found 61.22% of human-written TOEFL essays were falsely flagged, and NeurIPS published no demographic calibration data, raising particular concerns for ESL researchers. Affected authors can resubmit their papers to ICLR \(deadline September 25\) or ICML.

reddit · r/MachineLearning · /u/tughanbulut · Sep 8, 10:19

**「Background」** NeurIPS is one of the largest machine-learning conferences, and its Position Paper Track invites well-argued position papers rather than standard empirical research, with the track chairs responsible for review policy. In 2026 the track enforced its AI-use disclosure rules by automatically screening submissions with Pangram, a proprietary AI-detection tool. Conference materials reported that the screen flagged a large share of the 969 submissions and led to 178 desk rejections \(18.4%\) plus 123 conditional decisions requiring provenance evidence, while observers noted that the tool was used as an unappealable, uncalibrated gate.

**「Impact」** The 178 desk-rejected researchers were denied review and appeal but are not blacklisted, so their main recourse is resubmitting to another conference such as ICLR or ICML before upcoming deadlines.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.neurips.cc/2026/06/02/ai-generated-papers-in-the-neurips-2026-position-paper-track/">AI-Generated Papers in the NeurIPS 2026 Position Paper Track</a></li>
<li><a href="https://casrai.org/news/neurips-2026-pangram-ai-detector-desk-rejection-controversy">NeurIPS 2026 Pangram AI-Detector Desk Rejections - CASRAI</a></li>
<li><a href="https://news.creeta.com/en/neurips-2026-pangram-desk-rejections-uncalibrated/">NeurIPS 2026 Position Paper Desk Rejections via Pangram AI ...</a></li>

</ul>
</details>

**Tags**: `#NeurIPS`, `#AI detection`, `#academic publishing`, `#research integrity`, `#policy`

---

<a id="item-tech-news-3"></a>
### [Tim Cook Skips Apple September 9 Video as New CEO Leads Foldable iPhone Push](https://www.macrumors.com/2026/09/07/tim-cook-wont-appear-apple-sept-9-event-video/) ⭐️ 8.0/10

Bloomberg&\#x27;s Mark Gurman, citing sources, reports that Tim Cook will attend Apple&\#x27;s September 9 &\#x27;Surprise and Shine&\#x27; event screening but will not appear in the event video. Cook stepped down as CEO on September 1 and became executive chairman, with John Ternus succeeding him as CEO. Apple deliberately orchestrated the transition so that Ternus serves as the public face of the foldable iPhone and upcoming products, as Cook&\#x27;s on-screen presence would weaken that message. The MacRumors report describes this as a carefully planned leadership handoff, timed before the expected foldable iPhone reveal.

telegram · zaihuapd · Sep 8, 05:03

**「Background」** Tim Cook served as Apple&\#x27;s CEO for 15 years before stepping down on September 1, 2026, to become executive chairman. John Ternus, previously Apple&\#x27;s senior vice president of hardware engineering, succeeded him as CEO. Ternus is expected to deliver his first keynote at Apple&\#x27;s September 9 event, where the company is widely anticipated to unveil a foldable iPhone, making Cook&\#x27;s absence from the event video a deliberate part of the leadership transition.

<details><summary>References</summary>
<ul>
<li><a href="https://time.news/report-tim-cook-wont-be-speaking-at-apples-sept-9-event/">Report: Tim Cook Won&#x27;t Be Speaking at Apple&#x27;s Sept. 9 Event - Time News</a></li>
<li><a href="https://www.theverge.com/tech/915272/apple-john-ternus-tim-cook">John Ternus takes over as Apple’s new CEO | The Verge</a></li>
<li><a href="https://www.nbcbayarea.com/news/local/tim-cook-apple-ceo/4135772/">Tim Cook to step down as Apple CEO after 15-year tenure – NBC Bay Area</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#CEO transition`, `#Tim Cook`, `#foldable iPhone`, `#tech industry`

---

<a id="item-tech-news-4"></a>
### [ASML and TSMC Map High NA EUV Shift to 12-Inch Photomasks](https://www.nrc.nl/nieuws/2026/09/08/asml-gaat-samenwerken-met-taiwanese-chipgigant-tsmc-om-zijn-nieuwste-chipmachines-te-upgraden-a4936073) ⭐️ 7.0/10

On September 7, ASML and TSMC launched an industry collaboration to transition High NA EUV lithography from today&\#x27;s 6-inch photomasks to a 12-inch format, with the goal of raising equipment productivity, lowering chip manufacturing costs, and reducing stitching limitations. The plan targets a 12-inch photomask pilot line in 2031 and deployment of related systems for advanced-process mass production by 2033. TSMC intends to start using High NA EUV for large-scale manufacturing at advanced nodes in 2030. These milestones outline a multi-year roadmap that depends on successfully adopting the new mask infrastructure and integrating it into next-generation High NA EUV systems.

telegram · zaihuapd · Sep 8, 06:55

**「Background」** Current EUV and High NA EUV lithography systems use 6-inch photomasks, but High NA EUV&\#x27;s smaller exposure field makes stitching and productivity more challenging on that format. On September 7, 2026, ASML and TSMC announced a collaborative industry initiative, ahead of the SPIE Bacus Conference, to drive a transition to larger 12-inch photomasks to improve productivity and lower costs. The roadmap targets a 12-inch photomask pilot line by 2031 and advanced-node production readiness by 2033, while High NA EUV is initially expected to continue using 6-inch masks, with TSMC aiming for high-volume use around 2030.

**「Impact」** For leading-edge semiconductor manufacturers and the EUV supply chain, this collaboration sets a concrete schedule for the industry&\#x27;s eventual shift to 12-inch photomask infrastructure. If realized, the change could lower per-chip costs and ease pattern stitching constraints on High NA EUV nodes, though the planned 2031 and 2033 dates leave significant room for development and adoption risks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.asml.com/en/news/press-releases/2026/tsmc-and-asml-announce-industry-transition-to-large-format-photomasks-for-high-na-euv">TSMC and ASML Announce Initiative to Pioneer Industry ...</a></li>
<li><a href="https://tbreak.com/tsmc-asml-12-inch-photomasks-euv/">TSMC and ASML target 12-inch photomasks for High NA EUV</a></li>
<li><a href="https://www.digitalcitizen.life/asml-tsmc-and-samsung-push-12-inch-photomasks-to-unlock-high-na-euv-chipmaking/">ASML, TSMC and Samsung Push 12 Inch Photomasks to Unlock High ...</a></li>

</ul>
</details>

**Tags**: `#asml`, `#tsmc`, `#euv-lithography`, `#semiconductor-manufacturing`, `#high-na`

---

<a id="item-tech-news-5"></a>
### [China plans fourfold AI compute boost to 9800 EFLOPS by 2030](https://www.scmp.com/tech/policy/article/3366733/china-targets-fourfold-boost-ai-computing-capacity-2030-major-tech-push) ⭐️ 7.0/10

China&\#x27;s Ministry of Industry and Information Technology has issued a five-year industrial plan targeting 9800 EFLOPS of AI computing capacity by 2030, with cumulative information infrastructure investment of 3.8 trillion yuan from 2026 to 2030. The plan calls for orderly deployment of AI computing clusters at the 10,000-card and above-100,000-card scale, and for improving adaptation between infrastructure and domestic AI accelerator chips. As of the end of June 2026, China&\#x27;s AI computing capacity was 2185 EFLOPS, up 177% year on year, meaning the 2030 goal requires capacity to more than quadruple from that level.

telegram · zaihuapd · Sep 8, 11:23

**「Background」** China&\#x27;s Ministry of Industry and Information Technology \(MIIT\) has published a five-year industry plan that sets a 2030 intelligent computing target. The plan calls for 3.8 trillion yuan \(US$532 billion\) in information infrastructure investment and the deployment of AI clusters with 10,000 or more accelerator cards, while emphasizing adaptation between these clusters and domestic AI chips. As of June, China&\#x27;s intelligent computing capacity stood at 2,185 EFLOPS, so reaching 9,800 EFLOPS would require more than a fourfold expansion from that level.

**「Impact」** The plan gives Chinese AI chip vendors, data-center operators, and infrastructure suppliers a multiyear government-backed demand signal for domestic chip adaptation and very large AI compute clusters, while setting a concrete national capacity target against which progress can be measured.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/tech/policy/article/3366733/china-targets-fourfold-boost-ai-computing-capacity-2030-major-tech-push">China targets fourfold boost in AI computing capacity by 2030 in major tech push | South China Morning Post</a></li>
<li><a href="https://www.successstories.news/2026/09/08/china-targets-fourfold-boost-in-ai-computing-capacity-by-2030-in-major-tech-push-2/">China targets fourfold boost in AI computing capacity by 2030 in major tech push | Success Stories News</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#China tech policy`, `#compute capacity`, `#semiconductor adaptation`

---

<a id="item-tech-news-6"></a>
### [OpenAI Rolls Out ChatGPT Images 2.5 with Lower Latency](https://openai.com/index/introducing-chatgpt-images-2-5/) ⭐️ 7.0/10

OpenAI released ChatGPT Images 2.5 on September 8, an image generation model with clearer detail, more precise editing, and faster generation that cuts latency by up to 50% compared to version 2.0. The model is now available to all users across ChatGPT, ChatGPT Work, and Codex. ChatGPT adds new features including Sketch hand-drawing guidance, templates, image comments, and prompt sharing. On the API side, OpenAI introduced two new models, GPT-Image-2.5 Flare and GPT-Image-2.5 Sunburst.

telegram · zaihuapd · Sep 8, 18:45

**「Background」** OpenAI&\#x27;s ChatGPT Images system lets users generate and edit images from natural-language prompts. Earlier versions set the baseline for speed and fidelity, and this release targets measured improvements in both areas while extending availability across OpenAI&\#x27;s consumer, work, and coding products.

**「Impact」** ChatGPT and Codex users and API developers gain access to faster, higher-fidelity image generation and more precise editing tools, with new API model options that can be integrated into third-party applications.

**Tags**: `#OpenAI`, `#image generation`, `#AI model`, `#ChatGPT`, `#API`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Hybrid HiSparse Offloading in vLLM for GLM 5.3](https://vllm.ai/blog/2026-09-08-glm53-part1-hybrid-sparse-offloading) ⭐️ 8.0/10

rss · vLLM Blog · Sep 8, 00:00

**「Background」** Long-context agentic workloads run many concurrent requests whose KV cache keeps growing and eventually exhausts the fixed GPU block pool. The vLLM Team argues that the two usual responses—preemption, which forces a full re-prefill, and dense offloading to CPU, which still requires every token to be GPU-resident—are insufficient for this setting.

**「Solution」** The team introduces Hybrid HiSparse, a residency policy that keeps sparse-MLA KV cache on the GPU while capacity allows and offloads to CPU only under memory pressure. It exploits GLM 5.3&\#x27;s sparse attention: only top-K indexer-selected rows need to stay accessible, and those rows live in hot buffers leased from the same block pool and stored in the same KV-cache tensor, so they look like ordinary pages to the sparse-MLA kernel. Residency moves through full, mixed, and no-residency states per page; in mixed residency the request tail remains GPU-resident, older pages live on CPU, and a fused resolver reads resident tokens in place, refreshes hot-token LRU entries, and copies misses from pinned host memory without ever waiting on a CPU decision. Completed prefix pages are proactively copied to CPU before pressure arrives, and the copy is queued after the forward pass in one launch, keeping synchronization simple and the decode path CUDA-graph-capturable. In an 8×H200 OpenHands benchmark, Hybrid HiSparse made full 1M-context GLM 5.3 feasible and sustained higher concurrency across context lengths, though the authors note planning limits and that current MTP verification requires sizing hot buffers to \(num\_speculative\_tokens + 2\) × top-K.

**「Takeaway」** The vLLM Team concludes that Hybrid HiSparse is best understood not as another offloading knob but as a residency policy over the shared pool and tensor, enabling longer contexts and higher concurrency by transferring data to CPU only when the system is truly under KV-cache pressure.

**Tags**: `#vLLM`, `#KV cache`, `#sparse attention`, `#GPU memory offloading`, `#long-context inference`

---

<a id="item-tech-blog-2"></a>
### [Optimizing Real-World Agentic Serving with vLLM and AgentX](https://vllm.ai/blog/2026-09-08-vllm-agentx) ⭐️ 8.0/10

rss · vLLM Blog · Sep 8, 00:00

**「Background」** Agentic workloads—multi-turn coding sessions that replay long accumulated contexts each turn—are becoming dominant traffic for vLLM; OpenAI reported in June 2026 that Codex generated 64% of combined Codex and ChatGPT output tokens among enterprise customers. Representative AgentX traces show median 43-turn sessions, 142K-token inputs with only 444 output tokens, and over 96% prefix reuse, stressing both latency and serving cost.

**「Solution」** The authors argue optimization must span three planes. In the data plane, a hybrid KV cache manager uses one shared block pool for full, sliding-window, and linear attention, plus a packed layout that fixed DeepSeek V4&\#x27;s fragmented 92-tensor cache; hierarchical Mooncake Store offloading and interval-plus-selective retention preserve prefixes beyond GPU memory. In the execution plane, model-specific parallelism matters: decode context parallelism \(DCP\) sharded attention and lowered MLA decode latency on Kimi K3, while DeepSeek V4&\#x27;s compressed sparse attention made data/expert parallelism \(DEP\) the default, and prefill context parallelism reached a 2.65× speedup over TP8 on 32K prompts. Two scheduling controls—token caps that break head-of-line blocking and aligned prefill cadence across DEP ranks—improve mixed traffic, and a two-phase saturation sweep finds P/D ratios. Measured on AgentX, vLLM reaches up to 130K total tokens per GPU-second on DeepSeek V4 Pro and a 14.6×–106× serving-cost advantage over Opus 5 pricing. The authors also report &\#x27;bitter lessons&\#x27;: pipeline parallelism does not fit warm prefix-heavy turns, DCP does not transfer to DeepSeek V4, and session-aware sticky routing beats load balancing when inter-turn delays are short.

**「Takeaway」** Real-world agentic serving gains come from coordinating KV cache locality, architecture-specific parallelism, and scheduling policies rather than generic scaling. Exploiting prefix reuse is what makes order-of-magnitude cost advantages possible.

**Tags**: `#agentic workloads`, `#KV cache management`, `#LLM serving`, `#parallelism`, `#prefill/decode`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Crypto platforms lost $3.63 billion in cyberattacks, often despite security audits, CoinGecko says](https://www.cnbc.com/2026/09/08/crypto-platforms-lost-billions-to-cyberattacks-many-even-after-audits.html) ⭐️ 7.0/10

Cryptocurrency platforms lost more than $3.63 billion to cyberattacks and stolen passkeys between January 2025 and July 2026, according to a CoinGecko report. Roughly 88% of the stolen funds came from platforms that had completed independent security audits, and most attacks targeted areas those checks do not typically cover.

rss · CNBC Finance · Sep 8, 08:16

**「Background」** CoinGecko, a cryptocurrency market-data site, tracked 245 security incidents from January 2025 to July 2026. Its report said roughly 88% of stolen funds and about 60% of affected platforms had completed independent security audits, with most attacks exploiting areas—such as stolen passkeys—that routine audits typically do not cover.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/09/08/crypto-platforms-lost-billions-to-cyberattacks-many-even-after-audits.html">Crypto platforms have lost over $3.63 billion to cyberattacks — even though most of them did security checks</a></li>
<li><a href="https://crypto.news/coingecko-crypto-hacks-cost-3-63b-in-19-months/">CoinGecko: Crypto hacks cost $3.63B in 19 months</a></li>

</ul>
</details>

**Tags**: `#cryptocurrency`, `#cyberattacks`, `#CoinGecko`, `#Bybit`, `#financial crime`

---

<a id="item-finance-news-2"></a>
### [China injects $53.6 billion into state banks and insurers in recapitalization plan](https://www.cnbc.com/2026/09/07/china-state-banks-lenders-insurers-capital-solvency-bankrupt-nim-.html) ⭐️ 7.0/10

China’s finance ministry and other state institutions are injecting a combined 360 billion yuan \($53.6 billion\) into three state lenders and five insurers, a recapitalization package that Citibank said was smaller than markets had expected. Hong Kong-listed shares of the banks and insurers fell Monday, with Agricultural Bank of China and ICBC dropping 2.7% and 2.3%.

rss · CNBC Finance · Sep 7, 23:23

**「Background」** This is the first time Beijing has recapitalized insurers, and it follows a 500 billion yuan injection into four major state banks last year. Banks have faced record-low net interest margins — the spread between what they earn on loans and pay on deposits — while insurers’ solvency ratios have declined.

**「Impact」** According to analysts quoted in the article, the capital could help banks write off bad loans and lend to priority sectors, though Macquarie’s chief China economist expects limited short-term economic impact because credit demand is weak.

**Tags**: `#China`, `#bank recapitalization`, `#state-owned insurers`, `#financial policy`, `#capital injection`

---