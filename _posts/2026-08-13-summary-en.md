---
layout: default
title: "Horizon Summary: 2026-08-13 (EN)"
date: 2026-08-13
lang: en
---

> From 42 items, 14 important content pieces were selected

---

**Technology News**
1. [Qwen Releases Qwen3.8-2.4T-A95B, a 2.4T-Parameter Open-Weight MoE](#item-tech-news-1) ⭐️ 9.0/10
2. [DeepSeek V4 Pro 0813 Released on OpenRouter, Early Tests Mixed](#item-tech-news-2) ⭐️ 8.0/10
3. [Tailscale digs into 16-year-old SQLite WAL-reset bug](#item-tech-news-3) ⭐️ 8.0/10
4. [Zed unveils Delta for collaborative AI-agent conversations](#item-tech-news-4) ⭐️ 8.0/10
5. [Grok 4.6 Release Sparks Benchmark and API Debates](#item-tech-news-5) ⭐️ 8.0/10
6. [uBlock Origin Gives Up on Blocking Facebook Ads](#item-tech-news-6) ⭐️ 7.0/10
7. [Adam&\#x27;s Per-Coordinate Scaling Breaks GD&\#x27;s Implicit Low-Rank Bias](#item-tech-news-7) ⭐️ 7.0/10
8. [White House to Expand AI Safety Testing to Open-Source Models](#item-tech-news-8) ⭐️ 7.0/10
9. [Apple seeks news licensing deals for Siri AI with nine-figure budget](#item-tech-news-9) ⭐️ 7.0/10
10. [Trump Memo Lets Private Firms Run US-Backed Cyber Operations](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [EVs Dominate China’s New Car Market, With NEV Share at 65.1%](#item-finance-news-1) ⭐️ 8.0/10
2. [Chinese chipmaker YMTC overtakes Micron and Kioxia in NAND memory shipments](#item-finance-news-2) ⭐️ 7.0/10
3. [CME plans first futures tied to AI chip rental costs](#item-finance-news-3) ⭐️ 7.0/10
4. [China’s gig workforce hits 53 million as jobs outpace demand](#item-finance-news-4) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Qwen Releases Qwen3.8-2.4T-A95B, a 2.4T-Parameter Open-Weight MoE](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen released Qwen3.8-2.4T-A95B, an open-weights mixture-of-experts model with 2.4T total parameters and 95B active parameters. The release currently offers BF16 and FP8 checkpoints, with the BF16 version around 4.9TB; no lower-precision QAT checkpoints were provided initially. Qwen positions the model as competitive with top proprietary systems, and the associated Qwen3.8-Max adds vision, 1M context, and built-in tools that the open-weight version lacks. The model uses a license allowing internal use or commercial use under $50M annual revenue, with restrictions above that threshold.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**「Background」** Qwen3.8-2.4T-A95B is the largest open-weight model released by Alibaba&\#x27;s Qwen team and the open-weight variant of the proprietary Qwen3.8-Max. It is a sparse mixture-of-experts \(MoE\) model with 2.4 trillion total parameters but only 95 billion activated per token, using a fine-grained MoE architecture with hybrid full and linear attention and a long context window. This design lets a very large model serve with compute closer to a much smaller model, which is why its performance claims rival frontier proprietary models.

**「Impact」** Organizations can access near-frontier model weights openly, but deployment initially requires multi-terabyte memory and external quantization work; the license also restricts commercial serving above $50M annual revenue.

**「Community Discussion」** Commenters praised the 1-bit quantized size \(~397GB\) as bringing Opus-level performance to single-machine setups, while others noted that the open-weights version lacks the vision and 1M-context features of Qwen3.8-Max. There is also active comparison with DeepSeek V4-Pro and debate about when affordable hardware will run the full model.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/serve-qwen3-8-2-4t-a95b-a-2-4t-parameter-model-with-configurable-reasoning-on-nvidia-gb300-nvl72/">Serve Qwen3.8-2.4T-A95B, a 2.4T-Parameter Model, with Configurable ...</a></li>
<li><a href="https://benchable.ai/models/qwen/qwen3.8-2.4t-a95b-20260812">Qwen: Qwen3.8 2.4T A95B - AI Model Details &amp; Benchmarks</a></li>
<li><a href="https://openrouter.ai/qwen/qwen3.8-2.4t-a95b">Qwen3.8 2.4T A95B - API Pricing &amp; Providers | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#large language models`, `#AI`, `#Qwen`, `#open source`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [DeepSeek V4 Pro 0813 Released on OpenRouter, Early Tests Mixed](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek V4 Pro 0813 is a newly released DeepSeek model available through OpenRouter, with official API documentation and an independent Artificial Analysis page now listing it. Early Hacker News testing reports show strong results on at least one heavy workload: a user running a traffic simulator/distributed physics engine reported significant gains without introducing new problems, at roughly $12.50 for 2 billion tokens with 50% cache hits. Another user&\#x27;s task to generate a Docker Compose/Caddy/Postgres deployment produced &\#x27;few issues&\#x27; for DeepSeek V4 Pro 0813, while GPT-5.6-terra-high had none, suggesting mixed performance in containerization scenarios. These early reports highlight interest in the model&\#x27;s cost-per-task performance relative to other low-cost models like the latest DeepSeek Flash update.

hackernews · explosion-s · Aug 12, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49274600)

**「Background」** DeepSeek V4 Pro 0813 is the general-availability release of DeepSeek&\#x27;s flagship V4 Pro model, ending a preview period that lasted nearly four months; the build appeared on August 12, 2026. The V4 family offers a 1M-token context length and includes two variants: V4 Pro with 1.6T total parameters \(49B active\) and V4 Flash with 284B total parameters \(13B active\), with V4 Pro positioned to rival top closed-source models. The model is available through OpenRouter and the DeepSeek API, drawing interest for its cost-effectiveness and performance on development tasks.

**「Impact」** Developers now have a cheaper, 1M-context DeepSeek V4 Pro 0813 option via OpenRouter, priced roughly 11x less for input and 34x less for output than GPT-5.6 Sol and 36x/89x less than Claude Opus 5, but early community results are mixed: one user found it had issues on a Docker/Caddy deployment task that GPT-5.6-terra-high handled cleanly, while another reported significant gains on a distributed physics engine without regressions. Public benchmark coverage is not yet available for this model profile, so verification is incomplete.

**「Community Discussion」** Community reaction is mostly positive on pricing and practical coding, with one user reporting meaningful performance gains on a physics/traffic simulator for about $12.50 per 2B tokens \(50% cache hits\), and another eager to move from the DeepSeek Flash line. A counterexample found DeepSeek V4 Pro 0813 still had &\#x27;few issues&\#x27; on a Docker/Caddy/Postgres deployment task where GPT-5.6-terra-high had none, and several users emphasized cost-per-task over peak intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://www.unite.ai/deepseek-ships-v4-pro-as-its-flagship-model-leaves-preview/">DeepSeek Ships V4 Pro as Its Flagship Model Leaves ...</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260424/">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>
<li><a href="https://codersera.com/blog/deepseek-v4-pro-review-benchmarks-pricing-2026/">DeepSeek V4-Pro Review: Pricing, Benchmarks &amp; Verdict</a></li>
<li><a href="https://benchlm.ai/models/deepseek-v4-pro">DeepSeek V4 Pro Benchmarks &amp; Pricing (August 2026)</a></li>

</ul>
</details>

**Tags**: `#deepseek`, `#llm`, `#ai-models`, `#model-release`, `#openrouter`

---

<a id="item-tech-news-3"></a>
### [Tailscale digs into 16-year-old SQLite WAL-reset bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale published a detailed post-mortem of a 16-year-old SQLite WAL-reset race condition that affected its control plane. The company took out a commercial SQLite support contract and funded the development of an open-source VFS shim tool; the tool isolated the race condition almost immediately and is expected to help track down similar bugs in the future. The post-mortem shows that even a single-writer design can hit the subtle WAL-reset race when checkpointing happens concurrently, and it highlights the value of purpose-built debugging tools and paid support contracts for open-source infrastructure. The write-up drew strong Hacker News discussion, with commenters praising Tailscale&\#x27;s transparency and commitment to correctness.

hackernews · ropbear · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**「Background」** SQLite&\#x27;s write-ahead logging \(WAL\) mode allows one writer plus multiple readers without blocking, but a 16-year-old race condition in the WAL-reset path could corrupt databases when the write-ahead log is reset while readers are active. Tailscale ran SQLite as a single-writer database for its control plane, exactly the intended usage, yet still hit rare corruption; working with the SQLite developers, they isolated the bug and also found a second stale expression index bug. To accelerate diagnosis, Tailscale funded an open-source SQLite VFS shim debugging tool.

**「Impact」** SQLite users relying on WAL mode gain a reusable open-source VFS shim for diagnosing race conditions, and Tailscale&\#x27;s experience provides a concrete argument for commercial support contracts on critical open-source components.

**「Community Discussion」** Commenters largely praised Tailscale for funding specialized open-source tooling and taking out a support contract, calling it an exemplary model for serious debugging of subtle database bugs. Several questioned how the race could occur despite SQLite&\#x27;s intended single-writer design, while others noted that even SQLite&\#x27;s 92 million lines of tests cannot prove the absence of bugs.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL - Reset bug</a></li>
<li><a href="https://eucloudservers.com/reliability/tailscale-traces-database-corruption-to-16y-o-sqlite-wal-reset-bug/">Tailscale Traces Database Corruption To 16Y/o SQLite WAL - Reset ...</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#bug`, `#database`, `#debugging`, `#open-source`

---

<a id="item-tech-news-4"></a>
### [Zed unveils Delta for collaborative AI-agent conversations](https://zed.dev/blog/introducing-delta) ⭐️ 8.0/10

Zed announced Delta, a feature that embeds collaborative AI-agent conversations as documents directly in the editor. Delta combines real-time multiplayer conversation with a conversation-as-document model, allowing users to comment inline on agent threads. The design targets workflows such as code review and mentoring, where inspecting how an AI agent produced a result could be valuable. However, the practical utility of multiplayer coding is debated, with some users questioning whether it is necessary.

hackernews · khy · Aug 12, 18:19 · [Discussion](https://news.ycombinator.com/item?id=49276574)

**「Background」** Zed is a fast, open-source code editor positioned for agentic workflows, with native support for real-time collaborative editing, Git operations, and AI models such as its open-weight Zeta2 model. The new Delta feature is a specialized multiplayer environment that unifies code and AI-agent conversation into a single workspace, addressing the disconnect between code and discussion. It builds on Zed&\#x27;s existing collaborative and agentic infrastructure, making conversation threads first-class artifacts.

**「Impact」** For Zed users and teams using AI-assisted coding, Delta offers a new way to review and comment on AI-generated changes, potentially improving transparency and mentoring. Its value remains uncertain, as community reactions are divided.

**「Community discussion」** Commenters are split: some question the need for multiplayer editing and dislike verbose AI summaries that can skip edge cases, while others see potential for mentoring junior engineers and auditing agent-produced PRs. One user also criticized the post&\#x27;s low-contrast design for poor readability.

<details><summary>References</summary>
<ul>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-13-zed-introduces-delta-a-new-multiplayer-environment-for-collaborative-coding-with-ai-agents-and-real">Zed Delta: Multiplayer Coding Environment for AI Agents</a></li>
<li><a href="https://zed.dev/">Zed — Your last next editor</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#collaborative editing`, `#code editor`, `#Zed`, `#software development tools`

---

<a id="item-tech-news-5"></a>
### [Grok 4.6 Release Sparks Benchmark and API Debates](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

Grok 4.6 has been released by xAI, with an Artificial Analysis article providing benchmarks and analysis. The release is drawing attention because community members dispute the credibility of its reported gains, noting that many labs have suddenly produced Fable-level models within months. A common complaint is that the API injects a default system prompt that overrides developer instructions and refuses to discuss system prompts. The model is viewed as part of xAI&\#x27;s growing competition in the frontier AI space, but official technical details are not included in the available item.

hackernews · iLuddite · Aug 12, 15:32 · [Discussion](https://news.ycombinator.com/item?id=49274027)

**「Background」** Grok is a series of large language models developed by SpaceXAI \(xAI\), launched in November 2023 by Elon Musk. Grok 4.6 is the latest release, building on Grok 4.5 with a focus on long-running agents and more ambitious interactive and visual work.

**「Impact」** For developers using the Grok API, the added default system prompt can supersede custom instructions and lead to refusals around system-prompt discussion, which may disrupt agent workflows.

**「Community Discussion」** Commenters are split on whether the rapid appearance of Fable-level scores across labs indicates leaked techniques, distillation, or benchmark hacking, and some argue Grok&\#x27;s concise behavior makes it more pleasant than rivals like GPT-5.6 Sol and Claude 4.8/5. Others note xAI&\#x27;s heavy inference investment makes Grok a credible cheaper alternative for some frontier tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_%28chatbot%29">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://x.ai/news/grok-4-6">Introducing Grok 4 . 6 | SpaceXAI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Grok`, `#model release`, `#benchmarks`, `#xAI`

---

<a id="item-tech-news-6"></a>
### [uBlock Origin Gives Up on Blocking Facebook Ads](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 7.0/10

uBlock Origin has stopped trying to block ads on Facebook, saying the platform&\#x27;s ad markup is too difficult to filter. The change, reported by Neowin and discussed on Reddit, means the popular open-source blocker will no longer hide Facebook ads. Facebook achieves this by obfuscating ad markers—for example, splitting the word “ad” into single-letter spans with random class names and deep nested divs. Users who rely on uBlock Origin must now either tolerate ads or leave Facebook, underscoring the escalating arms race between ad blockers and social platforms.

hackernews · Markoff · Aug 12, 11:28 · [Discussion](https://news.ycombinator.com/item?id=49270726)

**「Background」** uBlock Origin is a widely used open-source content blocker that typically hides ads by matching filter-list rules against page markup and CSS selectors. Facebook has long made its ads difficult to block through obfuscated markup, random class names, and nested elements, forcing maintainers into a constant cat-and-mouse game. After years of this arms race, the volunteer team behind uBlock Origin decided to stop actively filtering Facebook ads altogether, according to recent reports.

**「Impact」** Users of uBlock Origin will now see Facebook ads that were previously hidden, and the decision removes one of the most widely used ad-blocking tools from the Facebook arms race. For those unwilling to accept ads, the practical alternatives are switching to another blocker or leaving Facebook, though commenters note that those options face similar challenges.

**「Community Discussion」** Commenters point to Facebook&\#x27;s deliberate obfuscation, with one describing how the word “ad” is split into single-letter spans with random class names and eight-layer-deep div nesting. Several argue that the only reliable solution is to leave Facebook, while others anticipate future computer-vision-based blockers that draw rectangles over ads.

<details><summary>References</summary>
<ul>
<li><a href="https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html">uBlock Origin Is Giving Up the Fight to Keep Ads Off Facebook</a></li>
<li><a href="https://www.neowin.net/news/facebook-ads-are-so-hard-to-block-that-ublock-origin-stopped-filtering-them/">Facebook ads are so hard to block that uBlock Origin stopped ...</a></li>

</ul>
</details>

**Tags**: `#uBlock Origin`, `#Facebook`, `#ad blocking`, `#privacy`, `#open source`

---

<a id="item-tech-news-7"></a>
### [Adam&\#x27;s Per-Coordinate Scaling Breaks GD&\#x27;s Implicit Low-Rank Bias](https://www.reddit.com/r/MachineLearning/comments/1vmjb3p/the_loss_does_not_see_the_basis_but_adam_does_r/) ⭐️ 7.0/10

Experiments with nine update rules on underdetermined matrix sensing at matched training loss show that Adam, RMSProp, Lion, signum, and Adafactor lose GD&\#x27;s implicit low-rank bias, while GD, shared-scalar Adam, Muon, and Shampoo retain it. The author attributes the split to Adam&\#x27;s per-coordinate second moment, which breaks the rotation invariance that the factored loss W=UV^T should respect. A one-parameter family interpolating between a per-coordinate denominator and a single shared scalar recovers the bias monotonically, pointing to anisotropy rather than adaptivity as the culprit. Muon is exact on truly low-rank targets but degrades fastest as a spectral tail is added, crossing over with GD near 4% tail energy. The author also found their own optimizer&\#x27;s per-coordinate clipping reduced recovery \(0.347 to 0.220 with global norm clip\), and cautions that a 43–44% held-out error reduction on hyperspectral data relied on a train-only learning-rate rule that disadvantages Adam.

reddit · r/MachineLearning · /u/EtherealGlyph · Aug 12, 16:39

**「Background」** In factored models W=UV^T, the loss is invariant to rotating U and V by an orthogonal matrix, and gradient descent respects that invariance. Adam&\#x27;s per-coordinate second moment breaks the invariance because scaling depends on the basis in which the factors are written. The post argues this basis dependence determines whether an optimizer keeps or loses GD&\#x27;s implicit low-rank bias in underdetermined problems.

**「Impact」** Practitioners relying on Adam for low-rank factorization may silently lose the low-rank bias that gradient descent would provide; switching to rotation-invariant optimizers or global norm scaling appears to restore it, though the author cautions that the reported hyperspectral gains depend on a train-only learning-rate rule and the theory covers only memoryless update rules.

**Tags**: `#optimization`, `#Adam`, `#low-rank bias`, `#matrix sensing`, `#machine learning`

---

<a id="item-tech-news-8"></a>
### [White House to Expand AI Safety Testing to Open-Source Models](https://www.wired.com/story/the-white-house-is-going-to-expand-its-ai-policy/) ⭐️ 7.0/10

According to a WIRED report, the White House plans to expand its AI policy framework to include pre-release safety testing for open-source models that reach frontier capability. The framework currently applies only to closed-source developers such as Anthropic and OpenAI, with open-source models expected to be added in the coming months. Because the Trump administration believes formal regulation would only help China catch up, the framework remains voluntary. Some officials worry that a possible 30-day testing requirement could inhibit U.S. company growth.

telegram · zaihuapd · Aug 13, 00:43

**「Background」** In early August 2026, the White House finalized a voluntary AI safety testing framework requiring the most powerful closed models from U.S. labs to undergo federal safety review before public release, while initially excluding open-weight models. The framework remains voluntary, and the administration has not publicly released the full policy or testing criteria. Under the reported expansion, open-source models that reach frontier capability would also be subject to pre-release safety testing, potentially including a 30-day review requirement.

**「Impact」** The expansion would require open-source model developers to undergo pre-release safety testing once their models reach frontier capability, extending rules that currently cover only closed models such as those from Anthropic and OpenAI. Officials worry the possible 30-day testing requirement could suppress U.S. innovation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wired.com/story/the-white-house-is-going-to-expand-its-ai-policy/">The White House Is Going to Expand Its AI Policy | WIRED</a></li>
<li><a href="https://www.theguardian.com/technology/2026/aug/07/white-house-ai">The White House’s plan to vet potentially dangerous AI is cloaked in secrecy | AI (artificial intelligence) | The Guardian</a></li>
<li><a href="https://www.yahoo.com/news/politics/articles/white-house-ai-framework-excludes-073920495.html">White House AI Framework Excludes Open-Weight Models From Federal Security Review, Creating Structural Competitive Asymmetry</a></li>
<li><a href="https://www.wired.com/story/the-white-house-is-going-to-expand-its-ai-policy/">The White House Is Going to Expand Its AI Policy | WIRED</a></li>
<li><a href="https://witho2.com/news/white-house-voluntary-ai-framework-frontier-models">White House Voluntary AI Rules: What the New Framework Means</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#open source`, `#regulation`, `#safety testing`, `#United States`

---

<a id="item-tech-news-9"></a>
### [Apple seeks news licensing deals for Siri AI with nine-figure budget](https://9to5mac.com/2026/08/12/report-apple-seeks-publisher-deals-to-give-siri-ai-better-access-to-current-events/) ⭐️ 7.0/10

Apple is negotiating multi-year content deals with publishers to supply its forthcoming Siri AI with current news and information, according to a Wall Street Journal report covered by 9to5Mac and MacRumors. The talks reportedly involve usage-based payments to partners rather than the fixed prepaid licensing fees typical of major AI companies, with a budget that could reach nine figures. No agreements have been announced, and Apple declined to comment. Siri AI is expected to launch later in 2026. The arrangement would represent a shift away from upfront lump-sum news licensing toward payments tied to actual content consumption.

telegram · zaihuapd · Aug 13, 04:40

**「Background」** Siri AI is Apple&\#x27;s upcoming AI assistant, expected to arrive later in 2026. AI companies often license news content through large upfront payments to train models or provide real-time answers. Apple&\#x27;s reportedly planned usage-based approach would instead pay publishers based on how often Siri AI uses their content.

**「Impact」** If completed, usage-based, nine-figure licensing could give publishers a revenue stream tied directly to Siri AI queries and make Siri AI a stronger competitor in real-time news responses, though the financial terms could make Apple&\#x27;s licensing costs larger and less predictable than fixed-fee deals.

**Tags**: `#Apple`, `#Siri`, `#AI`, `#news licensing`, `#artificial intelligence`

---

<a id="item-tech-news-10"></a>
### [Trump Memo Lets Private Firms Run US-Backed Cyber Operations](https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal) ⭐️ 7.0/10

President Trump signed a memorandum allowing private companies to conduct US-government-backed overseas surveillance and cyberattacks against foreign transnational criminal cyber organizations targeting Americans. The Department of Homeland Security will operate the program and coordinate oversight with the Department of Justice. Participating companies must maintain at least $1 million in bond or escrow funds, which can be forfeited if they fail to comply with contract terms. This policy significantly expands the private sector&\#x27;s role in US offensive cyber operations and raises implications for technology firms, privacy, and international security.

telegram · zaihuapd · Aug 13, 05:10

**「Background」** Offensive cyber operations and overseas surveillance have traditionally been conducted almost exclusively by U.S. government agencies such as the National Security Agency or U.S. Cyber Command, with the private sector largely restricted to defensive roles or contracting support. The newly announced program, outlined by the White House, allows vetted private U.S. companies to conduct cyber surveillance and offensive operations against foreign transnational criminal organizations while acting &\#x27;under the direction of the United States Government.&\#x27; The Department of Homeland Security will run the program in coordination with the Justice Department, and participating companies must maintain a bond or escrow of at least $1 million that can be forfeited if they fail to comply with their contracts.

**「Impact」** Cybersecurity and surveillance companies can now legally engage in US-government-endorsed overseas surveillance and cyberattacks under DHS-DOJ oversight, with a $1 million bond requirement governing their participation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal">Trump Signs Memo Allowing Private Firms to Conduct Cyber Attacks ...</a></li>
<li><a href="https://news.slashdot.org/story/26/08/13/0052208/trump-administration-enlists-private-companies-to-hack-foreign-cybercrime-groups">Trump Administration Enlists Private Companies To Hack... - Slashdot</a></li>
<li><a href="https://www.whitehouse.gov/presidential-actions/2026/08/expanding-capabilities-to-combat-transnational-cyber-enabled-crime/">Expanding Capabilities to Combat Transnational Cyber -Enabled Crime</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#policy`, `#surveillance`, `#technology-industry`, `#private-sector`

---

## Financial News

<a id="item-finance-news-1"></a>
### [EVs Dominate China’s New Car Market, With NEV Share at 65.1%](https://www.cnbc.com/2026/08/12/china-car-sales-data-byd-tesla-geely-vw.html) ⭐️ 8.0/10

New energy vehicles—battery and hybrid cars—accounted for 65.1% of new passenger cars sold in China in July, up from 54% a year earlier, according to China Passenger Car Association data; among model rankings from Autohome for the six months through July, Geely’s Xingyuan electric hatchback was the top seller with nearly 197,500 units, followed by Tesla’s Model Y.

rss · CNBC Finance · Aug 13, 01:31

**「Background」** China’s car market has shifted quickly toward electric vehicles, and competition has intensified as domestic brands cut prices and expand model lineups. In the same period, BYD reported passenger car sales down more than 10% in the first half, while overall passenger car sales fell 20.3% for the year through July.

**Tags**: `#China auto market`, `#electric vehicles`, `#BYD`, `#Tesla`, `#Geely`

---

<a id="item-finance-news-2"></a>
### [Chinese chipmaker YMTC overtakes Micron and Kioxia in NAND memory shipments](https://www.cnbc.com/2026/08/13/chinese-firm-tops-micron-kioxia-shipments-nand-memory-chips.html) ⭐️ 7.0/10

Chinese chipmaker YMTC took third place in global NAND memory chip shipments in the second quarter, with a 14% share that put it ahead of Micron and Kioxia but behind Samsung and SK hynix, according to Counterpoint Research. The company still trails Micron and Kioxia in NAND revenue, Counterpoint said.

rss · CNBC Finance · Aug 13, 02:59

**「Background」** NAND chips are memory chips that retain data when devices are powered off, and YMTC is preparing for an IPO in mainland China.

**Tags**: `#NAND memory`, `#YMTC`, `#semiconductor industry`, `#market share`, `#China tech`

---

<a id="item-finance-news-3"></a>
### [CME plans first futures tied to AI chip rental costs](https://www.cnbc.com/2026/08/11/ai-computing-power-becomes-a-tradable-asset-class-as-cme-starts-futures.html) ⭐️ 7.0/10

CME Group plans to launch the first futures contracts tied to AI chip rental costs on Oct. 5, pending regulatory approval, giving companies and investors a way to trade and hedge the price of AI computing capacity.

rss · CNBC Finance · Aug 12, 14:14

**「Background」** The contracts would be based on Silicon Data indexes that track hourly rental prices for Nvidia GPUs, with each contract representing a month&\#x27;s rent for an Nvidia H100, and would also cover the newer Blackwell B200.

**「Impact」** If approved, AI developers and data-center operators could use the contracts to hedge their computing costs, while investors could gain exposure to compute prices without owning chips or data centers.

**Tags**: `#AI`, `#futures`, `#CME Group`, `#GPU pricing`, `#commodities`

---

<a id="item-finance-news-4"></a>
### [China’s gig workforce hits 53 million as jobs outpace demand](https://www.ft.com/content/a3803e70-cb4d-444f-a31e-05be2f2c44f6?accessToken=zwAAAZ_5xcXzkdOjgD5wy01ET9OjHgW-LyxE9g.MEUCIQCWTIny3JTJV8e-PGyK0XL2tg5g_7Ay-rpKkwGZCpp1-AIgbMgJQPlqWgqAsX4s1k4gYaC4b8k0JveZOs35OJQvbZ4&amp;amp;sharetype=gift&amp;amp;token=7e8483bb-395d-429e-afca-2f4ab5ad150b) ⭐️ 7.0/10

According to a Financial Times report, China’s food-delivery and ride-hailing workforce reached more than 53 million by 2025, up 10 million in two years, but the supply of workers is outstripping available work and pushing incomes down.

telegram · zaihuapd · Aug 13, 06:40

**「Background」** The increase comes as China’s property downturn, weak consumption, manufacturing contraction and automation push surplus labour into flexible work such as food delivery and ride-hailing.

**「Impact」** The glut is visible at major airports, where taxi drivers at Shanghai Pudong, Beijing Daxing and Chengdu Tianfu reported waiting up to 7, 8 and 10 hours, and Shenzhen declared its ride-hailing market saturated in June.

**Tags**: `#China`, `#gig economy`, `#employment`, `#labor market`, `#economic slowdown`

---