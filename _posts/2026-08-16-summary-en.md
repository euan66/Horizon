---
layout: default
title: "Horizon Summary: 2026-08-16 (EN)"
date: 2026-08-16
lang: en
---

> From 32 items, 7 important content pieces were selected

---

**Technology News**
1. [Anthropic Publishes Official System Prompts for Claude Models](#item-tech-news-1) ⭐️ 8.0/10
2. [Qwen 3.8 27B is strong but defaults to excessive reasoning](#item-tech-news-2) ⭐️ 8.0/10
3. [SSOG-Attention: Sub-Quadratic Sum of Separable Gaussians Alternative to SDPA](#item-tech-news-3) ⭐️ 8.0/10
4. [Cloudflare silently injects analytics when you switch nameservers](#item-tech-news-4) ⭐️ 7.0/10
5. [PJM&\#x27;s $12B modeling mistake risks repeating, analysis says](#item-tech-news-5) ⭐️ 7.0/10
6. [Questioning ECA&\#x27;s Cross-Channel Interaction Hypothesis](#item-tech-news-6) ⭐️ 7.0/10

**Financial News**
1. [Anthropic&\#x27;s preliminary Q2 revenue tops $11.5B, up 14x from year earlier](#item-finance-news-1) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Anthropic Publishes Official System Prompts for Claude Models](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic published official system prompts for Claude models on its platform documentation, giving developers and researchers a way to inspect and track prompt changes over time. The release makes model behavior more transparent and is directly relevant to prompt engineering and interpretability. Community members highlighted Simon Willison&\#x27;s git commit history that rebuilds the prompts for easier diffing, including an example comparing Opus 4.8 and Opus 5. Commenters also noted concrete prompt instructions, such as Claude checking for the actual presence of an image and prioritizing user wellbeing during crises. The exact scope and update cadence of Anthropic&\#x27;s official prompt documentation remain unclear.

hackernews · tosh · Aug 16, 12:48 · [Discussion](https://news.ycombinator.com/item?id=49319556)

**「Background」** Claude&\#x27;s web and mobile interfaces use a system prompt at the start of every conversation to provide up-to-date information such as the current date and to encourage certain behaviors. Anthropic publishes these system prompts as part of its release notes, updating them with each model release so developers and researchers can examine and track changes over time.

**「Impact」** Developers and researchers using Claude can now study Anthropic&\#x27;s official system prompts as a reference point for understanding model behavior, supporting prompt engineering, interpretability, and safety auditing.

**「Community Discussion」** Commenters welcomed Simon Willison&\#x27;s git commit history for tracking prompt changes and highlighted revealing instructions, such as Claude checking whether an image is actually present and prioritizing wellbeing over task completion in crises. One commenter also raised an off-topic complaint that Hacker News appeared to be removing stories with negative AI portrayals.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/release-notes/system-prompts">System Prompts - Claude Platform Docs</a></li>
<li><a href="https://tactiq.io/learn/claude-system-prompt">Claude System Prompt Explained: What&#x27;s Inside and Why It Matters</a></li>

</ul>
</details>

**Tags**: `#claude`, `#system-prompts`, `#prompt-engineering`, `#anthropic`, `#ai-transparency`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B is strong but defaults to excessive reasoning](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

Alibaba&\#x27;s Qwen lab released Qwen 3.8 27B, an Apache 2 licensed 27B parameter vision-capable LLM. Self-reported benchmarks show gains over Qwen 3.6 27B and the closed-weight Qwen 3.7-Plus. Simon Willison tested the 17GB Q4\_K\_M quantized build on an M5 Max MacBook Pro and an NVIDIA DGX Spark, finding the model defaults to an xhigh reasoning effort that leads to spectacular overthinking. In one test, a pelican SVG took 21 minutes and 22,276 reasoning tokens at the default setting, while the same prompt with reasoning off took about 137 seconds. Willison recommends running Qwen 3.8 27B with low or no reasoning effort, and notes LM Studio&\#x27;s 8,192-token default context limit is too small for the model&\#x27;s default behavior.

rss · Simon Willison · Aug 16, 22:00

**「Background」** Qwen 3.8 27B is a mid-sized open-weight vision-capable LLM from Alibaba&\#x27;s Qwen lab, positioned as a successor to Qwen 3.6 27B. It supports a reasoning\_effort setting with xhigh, medium, and low levels; xhigh is the default and is intended for complex tasks, but it dramatically increases token usage and latency on consumer hardware.

**「Impact」** Local users of Qwen 3.8 27B should explicitly set reasoning\_effort to low or off to avoid excessive wait times and context exhaustion; the default xhigh can turn even simple requests into multi-minute generations. At 17GB for the quantized build, the model remains practical for laptop use once the reasoning level is adjusted.

**Tags**: `#Qwen`, `#LLM`, `#open source`, `#AI`, `#benchmarks`

---

<a id="item-tech-news-3"></a>
### [SSOG-Attention: Sub-Quadratic Sum of Separable Gaussians Alternative to SDPA](https://www.reddit.com/r/MachineLearning/comments/1vpt6ay/ssogattention_sum_of_separable_gaussians_as_a/) ⭐️ 8.0/10

SSOG-Attention replaces standard scaled dot-product attention \(SDPA\) with a Sum Of Separable Gaussians mechanism that learns a few Gaussian atoms per head and steers them based on each query token. Because the atoms factorize into a separable sum, the method reduces complexity from O\(N²·d\) to O\(N·√N·d\). In experiments reported by the author, SSOG clearly outperforms SDPA on CIFAR-100 and achieves equivalent performance with faster convergence on ImageNet-1k, while being faster and more memory efficient as scale increases. The project includes a blog post and an open-source repository.

reddit · r/MachineLearning · /u/4rtemi5 · Aug 16, 10:06

**「Background」** Scaled dot-product attention \(SDPA\) is the core mechanism of transformer models, computing similarity scores between all query and key-value tokens, which leads to quadratic complexity in sequence length. Sub-quadratic attention alternatives aim to reduce this cost by approximating the attention matrix or using factorized kernels. SSOG uses separable Gaussian atoms, a form of kernel-based approximation, to achieve lower complexity while remaining query-dependent.

**「Impact」** Vision transformer practitioners can use the released SSOG implementation to reduce attention cost and memory at scale, with reported accuracy gains on CIFAR-100 and parity on ImageNet-1k.

**Tags**: `#attention mechanisms`, `#sub-quadratic complexity`, `#efficient transformers`, `#computer vision`, `#Gaussian kernels`

---

<a id="item-tech-news-4"></a>
### [Cloudflare silently injects analytics when you switch nameservers](https://news.ycombinator.com/item?id=49322107) ⭐️ 7.0/10

A user reports that after moving nameservers to Cloudflare to enable R2 bucket serving on a subdomain, Cloudflare silently injected its Web Analytics JavaScript beacon into textlog.cc, an HTML-only, JS-free site. The snippet—loaded from static.cloudflareinsights.com/beacon.min.js with version data 2024.11.0—was present until the site owner manually found the Analytics dashboard, added the site, and disabled it. The report warns that Cloudflare&\#x27;s default is to opt users into the snippet, not require opt-in. Nameservers alone do not explain the injection; Cloudflare must be terminating HTTPS/proxying traffic. Commenters confirm seeing the same script on their sites and suggest a Content Security Policy to block third-party scripts.

hackernews · stagas · Aug 16, 17:49

**「Background」** Cloudflare&\#x27;s Web Analytics \(formerly part of its RUM, or Real User Monitoring, efforts\) measures page views and performance by injecting a small JavaScript beacon into proxied HTML responses. When a domain is &\#x27;orange-clouded&\#x27;—using Cloudflare as a reverse proxy for HTTPS—Cloudflare can alter the response body to include this script. DNS-only domains that do not go through the proxy appear not to receive the injection.

**「Impact」** Site owners who switch nameservers and proxy through Cloudflare may unknowingly send visitor data to Cloudflare&\#x27;s analytics and run extra JavaScript unless they explicitly disable Web Analytics; the user had to add the site in the dashboard before the opt-out appeared.

**「Community Discussion」** Commenters confirmed the silent injection: one pasted the exact beacon script with its integrity attribute, while another linked Cloudflare&\#x27;s &\#x27;RUM diaries&\#x27; post about enabling Web Analytics. A suggested workaround is setting a Content-Security-Policy that restricts script-src to &\#x27;self&\#x27; and trusted origins. Others noted that DNS-only domains show no Web Analytics enabled, suggesting the injection depends on using Cloudflare as a proxy.

**Tags**: `#Cloudflare`, `#privacy`, `#web analytics`, `#DNS`, `#site owners`

---

<a id="item-tech-news-5"></a>
### [PJM&\#x27;s $12B modeling mistake risks repeating, analysis says](https://newsletter.semianalysis.com/p/12b-of-us-ratepayers-money-wasted) ⭐️ 7.0/10

SemiAnalysis&\#x27;s Robert Boswall reports that a modeling mistake in PJM&\#x27;s grid wasted $12B of US ratepayers&\#x27; money and that PJM appears poised to make the same error again. The article frames the issue as a critical infrastructure failure rooted in using &\#x27;bad models&\#x27; for grid planning or operations. The specific technical details of the mistaken model and the nature of the repeated proposal are not supplied in the available excerpt, so the underlying mechanics remain limited to the headline claims. Because PJM is a major US grid operator, the $12B figure signals a large-scale impact on ratepayers if the risk materializes.

rss · Semianalysis · Aug 16, 22:27

**「Background」** PJM Interconnection, the largest U.S. power grid operator, runs a capacity market that pays generators years in advance to guarantee future electricity supply, with those costs passed on to ratepayers. The article argues that a modeling mistake in PJM&\#x27;s capacity auction produced roughly $12 billion in unnecessary payments and that PJM risks repeating the same failure. Recent PJM auctions have also drawn criticism over data-center-driven transmission costs and warnings of &quot;structural scarcity&quot; for the region.

**「Impact」** PJM ratepayers have already incurred billions in avoidable capacity costs tied to flawed modeling—IEEFA estimates $9.3 billion in extra costs in one year driven by data-center demand—and proposed PJM backstop and reliability-must-run agreements threaten further rate increases in Maryland and across the footprint.

<details><summary>References</summary>
<ul>
<li><a href="https://www.utilitydive.com/news/ferc-data-center-pjm-transmission-costs/825760/">FERC fails to shield PJM consumers from data center transmission costs: ratepayer advocates | Utility Dive</a></li>
<li><a href="https://avanzaenergy.substack.com/p/the-164-billion-reliability-tax-how?action=share">The $16.4 Billion Reliability Tax: How Data Centers Broke PJM&#x27;s Capacity Auction</a></li>
<li><a href="https://www.capitalgazette.com/2026/05/11/pjm-warns-maryland-energy-bills/">Maryland ratepayers could pay billions as PJM issues grid warning</a></li>
<li><a href="https://ieefa.org/resources/projected-data-center-growth-spurs-pjm-capacity-prices-factor-10">Projected data center growth spurs PJM capacity prices by... | IEEFA</a></li>
<li><a href="https://www.rtoinsider.com/138882-maryland-fears-pjm-backstop-effort-could-raise-ratepayer-costs/">Maryland Ratepayers at Risk from PJM Backstop, Advocate Says</a></li>
<li><a href="https://rtowww.com/85586-maryland-report-details-pjm-cost-increases-for-ratepayers/">Maryland Report Details PJM Cost Increases for Ratepayers</a></li>

</ul>
</details>

**Tags**: `#modeling`, `#energy grid`, `#software error`, `#infrastructure`, `#analysis`

---

<a id="item-tech-news-6"></a>
### [Questioning ECA&\#x27;s Cross-Channel Interaction Hypothesis](https://www.reddit.com/r/MachineLearning/comments/1vptaw9/revisiting_the_efficient_channel_attention_paper/) ⭐️ 7.0/10

The post critiques the Efficient Channel Attention \(ECA\) paper, arguing that applying a 1D convolution to channel means is conceptually flawed because channels lack the spatial topology that convolutions assume. The author reports experiments on 6-piece chess tablebases showing ECA with a kernel size of 1, which has no cross-channel interaction, matches ECA with k=3 and outperforms Squeeze-and-Excitation, undermining the paper&\#x27;s central hypothesis. They also note that the official and third-party repositories rarely test a pure k=1 ablation. While the results are preliminary and from a single Reddit analysis, the post demonstrates that ECA&\#x27;s benefit may not depend on cross-channel interaction as originally claimed.

reddit · r/MachineLearning · /u/arkuto · Aug 16, 10:13

**「Background」** ECA was introduced as an improvement over Squeeze-and-Excitation \(SE\) networks, using a 1D convolution over channel means instead of a dimensionality-reducing hidden layer. The original ECA paper claims that cross-channel interaction is key to its success. Convolutions are designed for data with spatial or temporal topology, so applying them to an unordered set of channels is conceptually questionable.

**「Impact」** If replicated, these findings would suggest that ECA&\#x27;s gains can be achieved with a simple per-channel scalar gate, and that researchers should test k=1 before attributing improvements to cross-channel interaction. The post also urges benchmarking on complete synthetic datasets, such as chess endgame tablebases, to separate regularization effects from architectural efficiency.

**Tags**: `#Efficient Channel Attention`, `#deep learning`, `#attention mechanisms`, `#computer vision`, `#critical analysis`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Anthropic&\#x27;s preliminary Q2 revenue tops $11.5B, up 14x from year earlier](https://www.cnbc.com/2026/08/15/anthropic-revenue-jumps-to-over-11point5-billion-in-q2-report.html) ⭐️ 8.0/10

According to Bloomberg, citing documents, Anthropic&\#x27;s preliminary second-quarter revenue was over $11.5 billion, up more than 14 times year over year from $787 million a year earlier and up from $4.73 billion in Q1 2026. Adjusted operating profit turned positive in the quarter; the figures are preliminary and could change, and the company is preparing for a possibly large IPO this fall.

telegram · zaihuapd · Aug 16, 07:26

**「Background」** Anthropic is the private AI company behind the Claude assistant; its Q1 2026 revenue was $4.73 billion and Q2 2025 revenue was $787 million, giving a baseline for the new preliminary figure.

<details><summary>References</summary>
<ul>
<li><a href="https://forgeglobal.com/insights/how-to-invest-in-anthropic-pre-ipo/">Insights: How to Invest in Anthropic Pre-IPO - Forge</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#earnings`, `#AI industry`, `#IPO`, `#revenue growth`

---