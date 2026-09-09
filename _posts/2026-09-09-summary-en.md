---
layout: default
title: "Horizon Summary: 2026-09-09 (EN)"
date: 2026-09-09
lang: en
---

> From 42 items, 13 important content pieces were selected

---

**Technology News**
1. [Apple Unveils Foldable iPhone Duo in New Hardware Push](#item-tech-news-1) ⭐️ 9.0/10
2. [OpenAI&\#x27;s unreleased model claimed to solve Navier-Stokes Millennium problem](#item-tech-news-2) ⭐️ 9.0/10
3. [vLLM v0.29.0 Makes Model Runner V2 Default, Adds New Models](#item-tech-news-3) ⭐️ 8.0/10
4. [Shopify acquires Tailwind CSS team and brand](#item-tech-news-4) ⭐️ 8.0/10
5. [Bypassing Google Ads Review to Advertise Malware](#item-tech-news-5) ⭐️ 8.0/10
6. [Autonomous Cars&\#x27; Life-Saving Evidence Debated](#item-tech-news-6) ⭐️ 7.0/10
7. [GPT-6 Astra and Looped Transformers: Analysis and Debate](#item-tech-news-7) ⭐️ 7.0/10
8. [How Anthropic envisions AI&\#x27;s economic future](#item-tech-news-8) ⭐️ 7.0/10
9. [Terence Tao Warns AI Rush on Open Problems Threatens Open Science](#item-tech-news-9) ⭐️ 7.0/10
10. [Pentagon reportedly requested OpenAI model with minimal military refusals](#item-tech-news-10) ⭐️ 7.0/10
11. [OpenAI Uses AI for Chip Design, Claims Cost Edge](#item-tech-news-11) ⭐️ 7.0/10

**Financial News**
1. [Adani Enterprises Airport Unit Announces $1 Billion Fundraising Deal](#item-finance-news-1) ⭐️ 8.0/10
2. [Chinese EV makers turn to humanoid robots as car sales slow](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Apple Unveils Foldable iPhone Duo in New Hardware Push](https://www.apple.com/iphone-duo/) ⭐️ 9.0/10

Apple has announced the iPhone Duo, a foldable iPhone that represents a major new hardware direction for the company. The announcement confirms Apple&\#x27;s entry into the foldable phone category and points to a significant shift in its product strategy. The product page at apple.com/iphone-duo provides little technical detail, so specifications, pricing, and availability are not yet disclosed. Apple&\#x27;s move matters because its scale and ecosystem influence could reshape consumer expectations and competition in the foldable smartphone market.

hackernews · thecosmicfrog · Sep 9, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49630931)

**「Background」** Apple announced the iPhone Duo at its September 2026 event, with CEO John Ternus revealing the first foldable iPhone — described by CNN as the biggest change to the iPhone in nearly 20 years. The device connects two halves into a continuous frame with a foldable inner display that unfolds to one 7.6-inch screen. It starts at $1,999 for 256GB of storage, with preorders beginning October 16 and availability on October 23.

**「Community Discussion」** Hacker News commenters are cautiously positive about the iPhone Duo: one praised the apparent lack of a crease and said Apple&\#x27;s presentation did not do the device justice, while another welcomed John Ternus&\#x27;s less Tim Cook-like keynote style. Others criticized the continuing trend toward larger phones and the rehearsed, emotionally flat delivery of the presenters.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnn.com/2026/09/09/business/live-news/apple-event-foldable-iphone-ternus">Apple event: CEO John Ternus reveals foldable iPhone Duo | CNN Business</a></li>
<li><a href="https://www.macrumors.com/2026/09/09/apple-announces-foldable-iphone-duo/">Apple Announces Foldable &#x27;iPhone Duo&#x27; - MacRumors</a></li>
<li><a href="https://www.ign.com/articles/apple-announces-foldable-iphone-duo">Apple&#x27;s Foldable iPhone Duo is Finally Real – Here&#x27;s Everything You Need to Know</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#iPhone Duo`, `#foldable phone`, `#consumer hardware`, `#product announcement`

---

<a id="item-tech-news-2"></a>
### [OpenAI&\#x27;s unreleased model claimed to solve Navier-Stokes Millennium problem](https://simonwillison.net/2026/Sep/8/on-navier-stokes/) ⭐️ 9.0/10

OpenAI says an unreleased internal model solved the Navier–Stokes existence and smoothness problem, a Clay Mathematics Institute Millennium Prize Problem carrying a $1,000,000 prize. According to OpenAI, agents began work on September 1 after hearing rumors and reached the solution on September 5, with Lean formalization and verification via GPT-6 Astra taking another 17 hours; the overall project used about 4.9 million messages and 300 billion output tokens, including 2.7 million messages and around 130 billion tokens for the Navier–Stokes result. The announcement is shadowed by accusations from NYU mathematician Tristan Buckmaster, who says he and Anthropic mathematician Levent Alpöge spent almost a year using Claude and Codex \(mainly GPT-5.6 Sol\) on related problems, had an August 15 breakthrough, and were then scooped by OpenAI after rumors spread. OpenAI denies seeing their work but says it cannot rule out that de-identified data derived from their product usage improved its models, and Alpöge was excluded as a co-author because of OpenAI&\#x27;s competitive relationship with Anthropic. The episode raises questions about whether rumor alone can trigger large AI-led research efforts and what it means for user data to be &quot;used to improve model performance.&quot;

rss · Simon Willison · Sep 8, 23:55

**「Background」** The Navier–Stokes existence and smoothness problem asks whether three-dimensional fluid flows described by the Navier–Stokes equations always have solutions that exist globally and remain smooth, or whether they can develop singularities. It is one of seven Millennium Prize Problems posed by the Clay Mathematics Institute in 2000, each with a $1 million reward, and has remained unsolved.

**「Impact」** If independently verified, it would be the first Millennium Prize resolution credited to AI agents, but the immediate result is a contested priority and authorship dispute among OpenAI, NYU, and Anthropic. The proof&\#x27;s validity is not yet independently established.

**Tags**: `#AI research`, `#mathematical breakthrough`, `#OpenAI`, `#Navier-Stokes`, `#Millennium Prize`

---

<a id="item-tech-news-3"></a>
### [vLLM v0.29.0 Makes Model Runner V2 Default, Adds New Models](https://github.com/vllm-project/vllm/releases/tag/v0.29.0) ⭐️ 8.0/10

vLLM v0.29.0, a 594-commit release from 277 contributors \(91 new\), makes Model Runner V2 the default execution path for all models, completing a rollout that started with pooling models. The release adds support for Hy4-preview, Qwen3.8-Flash-Next, GraniteSWA/GraniteMoeSWA, NemotronH\_Omni\_Reasoning\_V3, and Kimi K3 NVFP4 checkpoints, along with major MoE/MLA and speculative-decoding optimizations targeting Kimi-K3 and DeepSeek V4. New defaults enable FlashInfer all-reduce for tensor-parallel CUDA groups and deterministic prefix-cache hashing, while new admission-control flags \(\`--max-num-queued-reqs\` / \`--max-num-queued-tokens\`\) were introduced. Breaking changes include removal of ten deprecated model architectures, migration of FlexOlmo, Olmo3, and Hunyuan V1/VL to the Transformers backend, removal of the PyAV video decoder, and deprecation of \`python -m vllm.entrypoints.openai.api\_server\` in favor of \`vllm serve\`.

github · khluu · Sep 9, 08:54

**「Background」** vLLM is an open-source, high-throughput inference engine for large language models, commonly used to serve OpenAI-compatible APIs on GPU clusters. Model Runner V2 is vLLM&\#x27;s newer model execution framework introduced to replace the original Model Runner; it centralizes features such as sampling, CUDA graph capture, and prefix caching so optimizations can be applied consistently across model types.

**「Impact」** vLLM deployers upgrading to v0.29.0 should plan for behavior changes: Model Runner V2 becomes the default, ten deprecated architectures are removed, and the older OpenAI API Python entrypoint is deprecated, so launcher scripts and tooling relying on those paths need updates. Users staying on supported models and standard \`vllm serve\` workflows should otherwise benefit from the release&\#x27;s performance and memory optimizations without code changes.

**Tags**: `#vLLM`, `#LLM inference`, `#Model Runner`, `#GPU serving`, `#open source`

---

<a id="item-tech-news-4"></a>
### [Shopify acquires Tailwind CSS team and brand](https://tailwindcss.com/blog/tailwind-is-joining-shopify) ⭐️ 8.0/10

Shopify is acquiring the team and brand behind Tailwind CSS, a widely used open-source UI framework, per an announcement on the Tailwind site. The deal follows acknowledged AI-driven disruption to Tailwind Labs&\#x27; template business. Tailwind&\#x27;s tools help developers style web interfaces using utility classes. More specific terms or plans for Tailwind&\#x27;s roadmap have not been disclosed in the available materials.

hackernews · EdwinHoksberg · Sep 9, 13:27 · [Discussion](https://news.ycombinator.com/item?id=49626190)

**「Background」** Tailwind CSS is a popular open-source, utility-first CSS framework that lets developers style websites by applying pre-built utility classes directly in HTML. Shopify, a major e-commerce platform, has acquired Tailwind Labs, the company behind Tailwind CSS, with the stated goal of securing the framework&\#x27;s future under its existing MIT license.

**「Community Discussion」** Commenters mostly see the move as an acqui-hire of Tailwind&\#x27;s people and brand after AI undercut the template market; one cited earlier losses of 75% of the engineering team and a 40% drop in docs traffic. There is also debate over whether modern vanilla CSS reduces the need for Tailwind, alongside general appreciation for the framework and empathy for the team.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tradingview.com/news/seekingalpha:72d53b6e5094b:0-shopify-acquires-tailwind-labs/">Shopify acquires Tailwind Labs — TradingView News</a></li>
<li><a href="https://seekingalpha.com/news/4641301-shopify-acquires-tailwind-labs">Shopify acquires Tailwind Labs (SHOP:NASDAQ) | Seeking Alpha</a></li>

</ul>
</details>

**Tags**: `#acquisition`, `#tailwind`, `#css`, `#open-source`, `#shopify`, `#web-development`

---

<a id="item-tech-news-5"></a>
### [Bypassing Google Ads Review to Advertise Malware](https://xlii.space/eng/malicious-software-on-google-ads/) ⭐️ 8.0/10

A Hacker News submission by author xlii describes methods for advertising malicious software through Google Ads and getting it past Google&\#x27;s ad review process. The write-up highlights weaknesses in automated content moderation that can allow malvertising, stressing the practical security threat because Google Ads is one of the largest advertising platforms. It focuses on the systemic review gaps rather than simply the author&\#x27;s experience, and it argues that such attacks can reach users through trusted ad surfaces. The item demonstrates why platform integrity measures need stronger safeguards against adversarial ad content.

hackernews · xlii · Sep 9, 11:43 · [Discussion](https://news.ycombinator.com/item?id=49624856)

**「Background」** Google Ads is Google&\#x27;s paid advertising platform, and advertisers submit ads through an automated review process intended to filter out prohibited content, including sites that distribute malicious software. This item is a first-person explanation of how an attacker can work around those automated checks; in Hacker News comments, the author says the account was reinstated after the post gained public attention, and other users cite broader complaints about Google&\#x27;s over-reliance on automated moderation with little human recourse.

**「Community Discussion」** Hacker News commenters broadly criticized Google&\#x27;s moderation and review systems, sharing experiences showing both overly aggressive automated rejections and failures to catch fraudulent ads. The author also responded in the comments that their account was eventually reinstated after the post gained visibility through Hacker News and other complaints.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49624856">How I advertise malicious software on Google Ads | Hacker News</a></li>
<li><a href="https://news.ycombinator.com/item?id=49626346">I made an update, but I &#x27;ll post also here in comments. | Hacker News</a></li>
<li><a href="https://news.ycombinator.com/item?id=49627577">Another thing they apparently do is let business owners... | Hacker News</a></li>

</ul>
</details>

**Tags**: `#google-ads`, `#security`, `#malvertising`, `#ad-review-bypass`, `#platform-integrity`

---

<a id="item-tech-news-6"></a>
### [Autonomous Cars&\#x27; Life-Saving Evidence Debated](https://spectrum.ieee.org/are-self-driving-cars-safe) ⭐️ 7.0/10

An IEEE Spectrum report cites growing evidence that autonomous vehicles save lives, presenting a credible though incremental case that self-driving cars can reduce road deaths. The article highlights comparisons such as Waymo&\#x27;s accident rates against the average driver, a framing that has drawn scrutiny in online discussion. Commenters note that fatality data is complicated by seatbelt, speeding, alcohol, and vulnerable-road-user factors, and some question whether autonomous cars are the best way to improve safety. Overall, the piece adds to the evidence base for autonomous vehicle deployment but underscores the gap between data and societal acceptance.

hackernews · bookofjoe · Sep 9, 17:14 · [Discussion](https://news.ycombinator.com/item?id=49629886)

**「Background」** Autonomous vehicle \(AV\) safety has traditionally been measured against human drivers, with advocates pointing to the potential to prevent hundreds of thousands of deaths annually worldwide. Early data and studies, such as those referenced in the IEEE Spectrum report, suggest self-driving systems outperform humans in many routine driving scenarios, though exceptions and statistical caveats remain. Public debate often centers on how to compare AVs with human drivers, what baselines to use, and broader alternatives like public transit and stricter driving laws.

**「Community Discussion」** Commenters debate the persuasiveness of the statistics, with some criticizing Waymo for comparing its crash rates with average rather than rideshare drivers, while others point out that national fatality data is skewed by seatbelt, speeding, alcohol, and pedestrian or bicyclist deaths. A separate line of argument says resources would be better spent on public transit, and one commenter contends that a computer must never be allowed to kill anyone because it cannot be punished.

<details><summary>References</summary>
<ul>
<li><a href="https://spectrum.ieee.org/are-self-driving-cars-safe">Are Self Driving Cars Safe as Early Data Suggests? - IEEE Spectrum</a></li>
<li><a href="https://inspirega.bytes.news/78d7fc2-autonomous-vehicles-road-safety/">Self - Driving Cars Outperform Humans in Safety , with Some Exceptions</a></li>

</ul>
</details>

**Tags**: `#autonomous vehicles`, `#safety`, `#artificial intelligence`, `#transportation`, `#data analysis`

---

<a id="item-tech-news-7"></a>
### [GPT-6 Astra and Looped Transformers: Analysis and Debate](https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and) ⭐️ 7.0/10

An analysis piece discussing the purported GPT-6 Astra model links it to looped transformers and hidden reasoning, arguing that repeatedly feeding a transformer’s output back into itself at inference time effectively creates chain-of-thought reasoning that is not externally visible. The item has sparked an active practitioner debate about the computational trade-offs of chain-of-thought and whether such internal looping counts as hidden reasoning. However, the source presents an exploratory technical argument rather than confirmed product details, and no official announcement or benchmark evidence is cited in the available content. The discussion also draws on earlier universal-transformer research, with commenters comparing Astra to OpenAI&\#x27;s Sol and sharing anecdotal impressions of its capabilities and quality changes.

hackernews · ModelForge · Sep 9, 14:37 · [Discussion](https://news.ycombinator.com/item?id=49627370)

**「Background」** GPT-6 Astra is a reportedly upcoming AI model that, according to pre-release reporting cited in Sebastian Raschka&\#x27;s article, uses a technique called &\#x27;recurrent depth&\#x27; or &\#x27;looped transformers&\#x27;—reusing the transformer model&\#x27;s own output repeatedly instead of relying on an external chain-of-thought trace. This design is said to improve efficiency but also obscures some or all of the model&\#x27;s reasoning, raising concerns about transparency. A relevant theoretical reference is William Merrill and Ashish Sabharwal&\#x27;s 2023/2024 paper on the expressive power of transformers with chain-of-thought, which community commenters cite in discussions about the computational trade-offs of hidden versus visible reasoning.

**「Impact」** For AI/ML practitioners and evaluators, looped-transformer results indicate that hidden reasoning need not imply missing or degraded reasoning: because a looped model can refine a hidden-state vector rather than emitting readable tokens, it may carry out chain-of-thought-style computation without a textual trace. This shifts interpretability and evaluation work toward probing latent states, rather than treating an absent chain of thought as evidence of incomplete reasoning.

**「Community Discussion」** Commenters are split between technical framing and anecdotal experience: one links the problem to prior work on how much chain-of-thought is minimally required for computational tasks and notes that newer models are essentially “universal transformers” looping on themselves, while another argues that re-inputting a model’s own output at inference time is by definition hidden reasoning. Subjective reports diverge, with one user lamenting that Astra changed dramatically after a Tuesday update and now feels like Sol, another praising a real-time MSPAINT computer-use demo, and one asking how users can find Astra light worse than Sol High.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-6_Astra">GPT-6 Astra - Wikipedia</a></li>
<li><a href="https://magazine.sebastianraschka.com/p/gpt-6-astra-looped-transformers-and">GPT-6 Astra, Looped Transformers, and Hidden Reasoning</a></li>
<li><a href="https://ai-tldr.dev/releases/sebastian-raschka-looped-transformers-sep9/">Sebastian Raschka — looped transformers and what… | AI/TLDR</a></li>
<li><a href="https://arxiv.org/abs/2310.07923">[2310.07923] The Expressive Power of Transformers with Chain of Thought</a></li>
<li><a href="https://tosea.ai/blog/looped-transformer-recurrent-depth-astra-guide">What Is a Looped Transformer ? Complete Guide to... | Tosea. ai</a></li>
<li><a href="https://www.alphaxiv.org/abs/2502.17416">Reasoning with Latent Thoughts : On the Power of Looped ... | alphaXiv</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#transformer-architecture`, `#chain-of-thought`, `#GPT`

---

<a id="item-tech-news-8"></a>
### [How Anthropic envisions AI&\#x27;s economic future](https://www.anthropic.com/institute/econ-scenarios) ⭐️ 7.0/10

Anthropic&\#x27;s economic scenarios analysis, titled &quot;What will our economic future look like?&quot;, explores how AI could reshape work, productivity, and healthcare. The piece highlights potential productivity gains, such as nurses using AI to oversee more tasks while spending more time with patients, and argues that new tasks will emerge as AI takes over existing ones. However, the analysis has drawn criticism for its optimistic framing and for omitting plausible negative outcomes, including labor displacement under cost pressures, damage to education and trust, rising inequality, and the possibility of an economic crisis driven by overbuilt data centers.

hackernews · oumua\_don17 · Sep 9, 13:38 · [Discussion](https://news.ycombinator.com/item?id=49626373)

**「Background」** Anthropic&\#x27;s Economics Team released a working paper and an interactive web tool modeling how artificial intelligence might affect the U.S. and global economy by 2030. The report, “Economic Scenarios for Transformative AI,” is The Anthropic Institute Working Paper No. 2026-02, and the interactive explorer is version 1.0 dated September 2026. The model was developed by Anton Korinek, Charles I. Jones, Szymon Sacher, Tess Cotter, and Peter McCrory, with coordination by McCrory, Korinek, and Charles Yang, and direction from Jack Clark.

**「Community discussion」** Commenters largely challenge the article&\#x27;s economic assumptions, arguing that if AI lets one nurse do the work of two, the default in a cost-driven system is to reduce staffing, not to spend more time with patients. Others criticize the piece for ignoring damaging scenarios such as erosion of learning and trust, worsening inequality, and the risk that many data-center investments will belong to companies that do not survive the winner-take-all dynamics.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/institute/econ-scenarios">Scenarios for our Economic Future \ Anthropic</a></li>
<li><a href="https://www-cdn.anthropic.com/files/4zrzovbb/website/cf58f84d46a4a76bf5a5b039ac695fba6b80041c.pdf">Economic Scenarios for Transformative AI</a></li>
<li><a href="https://www.unite.ai/anthropic-releases-interactive-model-of-ais-possible-economic-futures/">Anthropic Releases Interactive Model of AI’s Possible Economic Futures</a></li>

</ul>
</details>

**Tags**: `#economics`, `#artificial-intelligence`, `#future-of-work`, `#anthropic`, `#analysis`

---

<a id="item-tech-news-9"></a>
### [Terence Tao Warns AI Rush on Open Problems Threatens Open Science](https://simonwillison.net/2026/Sep/9/terence-tao/) ⭐️ 7.0/10

Terence Tao has said that the collection of good, fruitful open mathematical problems is now being mined in a non-renewable fashion, potentially making such problems scarce. He observed that even the rumor of someone working on a problem can trigger a massive AI-powered effort to flatten it before the original research project reaches its full potential. Tao warned that current incentives may push researchers to stop sharing promising research directions, reversing centuries of open-science tradition and causing serious long-term damage to mathematics. The remarks were posted on Mathstodon and highlighted by Simon Willison on his blog.

rss · Simon Willison · Sep 9, 00:20

**「Background」** Terence Tao is a prominent mathematician who has publicly discussed how AI tools are changing mathematical research. He recently noted that the identification of promising open problems has become a scarce resource, because even a rumor that someone is working on a problem can trigger a large wave of AI-assisted effort to solve it before the original researcher&\#x27;s project matures. This creates incentives for researchers to stop sharing their promising research directions with the broader community, potentially reversing long-standing traditions of open science in mathematics.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Sep/9/terence-tao/">A quote from Terence Tao</a></li>
<li><a href="https://teorth.github.io/tao-web/ai-views.html">Terence Tao on AI — a living summary — Terence Tao</a></li>

</ul>
</details>

**Tags**: `#ai-ethics`, `#open-science`, `#mathematics`, `#research`, `#ai-impact`

---

<a id="item-tech-news-10"></a>
### [Pentagon reportedly requested OpenAI model with minimal military refusals](https://theintercept.com/2026/09/08/pentagon-openai-military-contract/) ⭐️ 7.0/10

Leaked documents reported by The Intercept allege that the U.S. Department of Defense requested a special version of OpenAI’s AI technology for the U.S. military that would refuse military commands as rarely as possible. The “lowest refusal rate” clause reportedly appeared in contract amendment “P00003,” which expanded a deal originally made with OpenAI last summer. Both OpenAI and the Pentagon deny agreeing to such language, saying the leaked P00003 document is a draft, not an executed contract. OpenAI spokesperson Nate Evans stated, “OpenAI has never agreed to contract language requiring the &\#x27;lowest refusal rate&\#x27;; that is not something that exists in the contracts we have executed.”

telegram · zaihuapd · Sep 9, 09:02

**「Background」** OpenAI&\#x27;s public position on military use has shifted significantly in recent years, moving from broadly prohibiting applications for warfare toward allowing national-security and defense work with the U.S. government. Last summer&\#x27;s prototype contract with the Pentagon, worth up to $200 million over its two-year duration, was later expanded by an amendment labeled &quot;P00003.&quot; The dispute reported here centers on whether that amendment sought to define &quot;mission models&quot; by a &quot;minimal refusal rate&quot; to military commands; OpenAI and the Pentagon say the phrase appeared only in draft language and not in the executed contract.

<details><summary>References</summary>
<ul>
<li><a href="https://theintercept.com/2026/09/08/pentagon-openai-military-contract/">The Pentagon Asked OpenAI for Artificial Intelligence Designed to...</a></li>
<li><a href="https://www.remio.ai/post/openai-pentagon-contract-records-reveal-a-disputed-demand-for-ai-that-rarely-say">OpenAI Pentagon Contract Records Reveal a Disputed Demand for...</a></li>
<li><a href="https://www.unite.ai/openai-pentagon-contract-defines-mission-models-by-minimal-refusal-rates/">OpenAI Pentagon Contract Defines ‘Mission Models’ by Minimal ...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#OpenAI`, `#military AI`, `#contracts`, `#policy`

---

<a id="item-tech-news-11"></a>
### [OpenAI Uses AI for Chip Design, Claims Cost Edge](https://www.reuters.com/world/china/openai-offers-ai-chip-design-touts-cost-advantage-over-open-source-cfo-says-2026-09-09/) ⭐️ 7.0/10

OpenAI CFO Sarah Friar said the company is expanding AI into chip design, life sciences, and financial services, and that deploying its low-cost Luna cloud model is cheaper than Chinese open-source alternatives. OpenAI said its in-house Jalapeno chip was finalized in nine months. After a reported 80% price cut for Luna, usage grew about tenfold. The claims come from company statements and Reuters coverage, without independent technical verification.

telegram · zaihuapd · Sep 9, 13:06

**「Background」** OpenAI CFO Sarah Friar said at the Goldman Sachs Communacopia conference that the company used its own AI models to help design its custom Jalapeno chip, which completed tape-out in under nine months. Tape-out is the chip-industry milestone when a design is locked and handed to a fabrication plant for manufacturing. In the same remarks, Friar said OpenAI&\#x27;s Luna cloud model undercuts Chinese open-source rivals on price after an 80% price cut, and the company also reported about 10 times higher usage after the reduction.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/openai-cfo-sarah-friar-says-123936035.html">OpenAI CFO Sarah Friar says Luna undercuts Chinese AI on price</a></li>
<li><a href="https://forkast.news/openai-used-its-own-ai-models-to-design-the-jalapeno-chip-the-compute-landlord-thesis-just-went-recursive/">OpenAI Used Its Own AI Models to Design the Jalapeno Chip – The Compute Landlord Thesis Just Went Recursive</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Chip Design`, `#AI Models`, `#Cost Optimization`, `#Open Source`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Adani Enterprises Airport Unit Announces $1 Billion Fundraising Deal](https://www.cnbc.com/2026/09/09/adani-enterprises-airport-fundraise-shares.html) ⭐️ 8.0/10

Shares of Adani Enterprises gained nearly 5% after its airport unit said it reached a binding deal to raise about 98.25 billion rupees \($1 billion\) from global and domestic investors at a pre-money valuation of about $18 billion.

rss · CNBC Finance · Sep 9, 06:26

**「Background」** Adani Airport Holdings operates eight Indian airports and handles more than 23% of the country’s passenger traffic, according to the company. The funds are intended to expand infrastructure and city-side developments and help increase capacity to about 200 million passengers a year; this deal follows a 150 billion rupee institutional share placement by Adani Enterprises in July.

**Tags**: `#Adani Enterprises`, `#airport infrastructure`, `#fundraising`, `#India`, `#Temasek`

---

<a id="item-finance-news-2"></a>
### [Chinese EV makers turn to humanoid robots as car sales slow](https://www.cnbc.com/2026/09/09/chinas-ev-makers-shift-gears-to-focus-on-humanoids-as-car-market-slows.html) ⭐️ 7.0/10

Chinese electric-vehicle makers are moving into human-shaped robots as car sales slow and profit margins shrink. Xpeng raised $900 million last month for its robotics unit—a round valuing that business at more than $6.3 billion—and says it will begin mass-producing the robots by the end of this year.

rss · CNBC Finance · Sep 9, 04:12

**「Background」** Chinese automakers make up more than half of nearly 20 global car companies that had entered humanoid robotics through in-house development, investment or incubation as of August, according to Counterpoint Research, and the average profit margin in China&\#x27;s vehicle-manufacturing sector was only 1.5% in the first half of 2026.

**Tags**: `#China EV`, `#Humanoid robots`, `#Xpeng`, `#Robotics financing`, `#Auto industry`

---