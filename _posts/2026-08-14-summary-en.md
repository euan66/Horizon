---
layout: default
title: "Horizon Summary: 2026-08-14 (EN)"
date: 2026-08-14
lang: en
---

> From 39 items, 17 important content pieces were selected

---

**Technology News**
1. [GLM-5.3: Frontier coding with emergent cyber capabilities](#item-tech-news-1) ⭐️ 9.0/10
2. [Qwen 3.8 27B open-weight model wins praise for reasoning](#item-tech-news-2) ⭐️ 8.0/10
3. [Doom&\#x27;s Renderer Compiled into a 21B-Parameter Transformer Without Training](#item-tech-news-3) ⭐️ 8.0/10
4. [Xiaohongshu open-sources dots3-note: 280B MoE with 16B active params](#item-tech-news-4) ⭐️ 8.0/10
5. [PostgreSQL Patches High-Risk to\_char RCE Vulnerability CVE-2026-14669](#item-tech-news-5) ⭐️ 8.0/10
6. [Why Opus 5&\#x27;s Agent-Focused Post-Training May Make It Feel Worse](#item-tech-news-6) ⭐️ 7.0/10
7. [RustDesk adds true unattended remote access on Wayland](#item-tech-news-7) ⭐️ 7.0/10
8. [Firefox is now the last major browser supporting uBlock Origin](#item-tech-news-8) ⭐️ 7.0/10
9. [torch-preflight: A New Linter for PyTorch Training Bugs and VRAM Estimates](#item-tech-news-9) ⭐️ 7.0/10
10. [US Court Orders Google to Remove Play Store Hurdles for Third-Party App Stores](#item-tech-news-10) ⭐️ 7.0/10
11. [Apple Trains China-Exclusive AI Model with Alibaba Support](#item-tech-news-11) ⭐️ 7.0/10

**Technology Blog**
1. [DSpark adaptive verification makes vLLM speculative decoding load-aware](#item-tech-blog-1) ⭐️ 9.0/10

**Financial News**
1. [Apple Proposes App Store External Purchase Commissions of Up to 15%](#item-finance-news-1) ⭐️ 8.0/10
2. [Berkshire Hathaway boosts Alphabet to top-three holding, ends net-selling streak](#item-finance-news-2) ⭐️ 7.0/10
3. [Goldman Sachs profits from underwriting AI infrastructure boom](#item-finance-news-3) ⭐️ 7.0/10
4. [Premarket Movers: Reddit Jumps on S&amp;P 500 Inclusion; Applied Materials Drops After Earnings](#item-finance-news-4) ⭐️ 7.0/10
5. [CITIC Trustar Near $1.5 Billion Deal for Alibaba Gaming Unit Lingxi](#item-finance-news-5) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [GLM-5.3: Frontier coding with emergent cyber capabilities](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.ai has released GLM-5.3, a frontier coding model with emergent cyber capabilities that can autonomously conduct security research and uncover vulnerabilities at scale. According to the release analysis, the model demonstrates real-world red-team scenarios, 0-day discovery, and large-scale vulnerability disclosure. The release has drawn significant community engagement, with 1,021 points and 503 comments on Hacker News, highlighting its importance across AI, software engineering, and security. The model is positioned as a top-tier release, with some commenters noting it trails Sol and Fable on certain benchmarks but remains closely competitive, while others describe it as essentially a post-trained GLM 5.2.

hackernews · pella · Aug 14, 05:19 · [Discussion](https://news.ycombinator.com/item?id=49294997)

**「Background」** Z.ai released GLM-5.3 on August 14, 2026, as an update to its open-source GLM-5.2 model, with every capability gain attributed to scaled-up post-training rather than a new base model. The release emphasizes frontier coding improvements and emergent cybersecurity abilities, achieving state-of-the-art results on benchmarks such as CyberGym for vulnerability discovery while more than doubling GLM-5.2&\#x27;s performance on exploit benchmarks. These capabilities are positioned as a step toward democratizing advanced cyber-defense tools, though the model still lags in attack development compared to some proprietary alternatives.

**「Impact」** According to Hacker News commenters, GLM-5.3 is already being used for autonomous red-team research and Z.ai&\#x27;s CVD portal shows numerous CVEs from large-scale OSS scans, giving security teams a powerful new capability while adding disclosure workloads for maintainers of popular software.

**「Community Discussion」** Commenters report strong practical results—one user says GLM-5.3 executed a security research scenario seamlessly, including 0-days in WordPress plugins, RCE, and Linux kernel exploit adaptation—while others note it still trails Sol and Fable on some benchmarks and question the cost and disclosure process of scanning OSS at scale. Several commenters appreciate Z.ai&\#x27;s more research-focused, less marketing-driven communication style.

<details><summary>References</summary>
<ul>
<li><a href="https://www.devdiscourse.com/article/technology/3963858-zais-open-source-model-glm-53-challenges-cybersecurity-norms">Z.ai&#x27;s Open-Source Model GLM-5.3 Challenges Cybersecurity Norms | Technology</a></li>
<li><a href="https://www.unite.ai/z-ai-launches-glm-5-3-with-frontier-coding-and-a-cyber-capability-that-outgrew-its-training/">Z.ai Launches GLM-5.3 With Frontier Coding and a Cyber Capability That Outgrew Its Training – Unite.AI</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM-5.3 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**Tags**: `#artificial intelligence`, `#cybersecurity`, `#code generation`, `#GLM`, `#open source`

---

<a id="item-tech-news-2"></a>
### [Qwen 3.8 27B open-weight model wins praise for reasoning](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 8.0/10

Qwen 3.8 27B, an FP8 open-weight model from the Qwen family now on Hugging Face, is drawing attention for strong reasoning and local inference. Commenters report it is the second local model after Gemma 4 to solve a private reasoning benchmark, but took about 5x the tokens and 12m30s with MTP enabled, with less efficient VRAM usage than Gemma 4 or Glimmer. On an RTX 5090, one user measured ~138 tokens/second using the ninfer engine, roughly double a naive llama.cpp setup. Others note a changed, note-form thinking trace compared to Qwen 3.6 and praise the quality of local output, including a realistic pelican image. The release appears among a broader wave of capable open-weight models such as GLM 5.3 and Deepseek models.

hackernews · erdaltoprak · Aug 14, 15:00 · [Discussion](https://news.ycombinator.com/item?id=49299605)

**「Background」** Alibaba&\#x27;s Qwen family is a series of open-weight large language models widely used by developers for local inference. Qwen3.8, announced on August 3, 2026, is the latest generation and includes Qwen3.8-27B, a 27-billion-parameter model intended to run on consumer hardware such as laptops; Alibaba has committed to open weights for the release. The Qwen3.8 generation follows the widely adopted Qwen3.5 and Qwen3.6 series and is described as the most capable generation in the open-model family to date.

**「Community Discussion」** Commenters are broadly enthusiastic, calling the model &\#x27;so good&\#x27; and praising its explicit reasoning, while noting trade-offs like high token usage and VRAM inefficiency. One user recommends ninfer on RTX 5090 for ~138 tokens/s, and another observes the distinctive note-style thinking trace.

<details><summary>References</summary>
<ul>
<li><a href="https://www.yottalabs.ai/post/qwen-3-8-27b-specs-hardware-requirements-how-to-run-2026">Qwen 3.8 27B: Specs, Hardware Requirements, and How to Run It (2026) | Yotta Labs</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#Qwen`, `#language-model`, `#open-source`, `#local-inference`, `#AI-reasoning`

---

<a id="item-tech-news-3"></a>
### [Doom&\#x27;s Renderer Compiled into a 21B-Parameter Transformer Without Training](https://www.reddit.com/r/MachineLearning/comments/1voazhm/i_compiled_dooms_renderer_into_a_21bparameter/) ⭐️ 8.0/10

The author ported Doom&\#x27;s rendering algorithm into a 21B-parameter transformer by using a custom compiler that converts computation graphs into transformer weights, requiring no training on the resulting model. The checkpoint is a standard Hugging Face transformers file and can be loaded without trust\_remote\_code; the host program to load it, generate a frame, and parse pixel-drawing commands from the output is only 43 lines of Python. Rendering one E1M1 frame uses a 3,614-token prompt and generates 53,747 tokens, taking just over 40 minutes on a B200 GPU, which the author contrasts with Doom&\#x27;s original 35 FPS on a 486 versus this system&\#x27;s 35 frames per day. The project is positioned as a proof-of-concept for weight-programming, with a write-up, weights on Hugging Face, and source code on GitHub.

reddit · r/MachineLearning · /u/notforrob · Aug 14, 15:50

**「Background」** The approach relies on an emerging weight-programming technique: instead of training a transformer, a compiler computes weights directly from an existing computation graph, provided the graph has a schedule for when each intermediate variable exists. This was previously demonstrated in a tiny computer inside a transformer and in a calculator compiled into a Hugging Face Phi-3 checkpoint. The Doom project extends that pattern to a full rendering algorithm, producing standard transformers checkpoints with no training and no custom code.

**「Impact」** For ML researchers working on algorithmic transformers, the project demonstrates a practical pathway from an arbitrary computation graph to usable transformer weights, although at 35 frames per day it is not a viable real-time rendering method.

<details><summary>References</summary>
<ul>
<li><a href="https://towardsdatascience.com/i-built-a-tiny-computer-inside-a-transformer/">I Built a Tiny Computer Inside a Transformer | Towards Data Science</a></li>
<li><a href="https://ood.dev/posts/calculator/">A calculator, compiled into a transformer — Out of Distribution</a></li>

</ul>
</details>

**Tags**: `#transformers`, `#compilers`, `#computation graphs`, `#Doom`, `#neural rendering`

---

<a id="item-tech-news-4"></a>
### [Xiaohongshu open-sources dots3-note: 280B MoE with 16B active params](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

Xiaohongshu&\#x27;s dots lab has open-sourced dots3-note preview, the first open-weight model in the dots3 series. The model is a 280B-parameter mixture-of-experts \(MoE\) with only 16B active parameters per inference step, supports a 512K-token context, and handles text, images, video, and audio. It introduces TEMPO, a new reinforcement learning method that trains long-horizon agents using self-critique and test-time value estimation. The weights are available on Hugging Face, alongside two new real-scenario agent benchmarks, VibeSearchBench and VibeLifeBench.

telegram · zaihuapd · Aug 14, 08:27

**「Background」** dots3-note preview is the first open-weight model in Xiaohongshu&\#x27;s dots3 series, released by its dots lab as a Mixture-of-Experts \(MoE\) model with 280 billion total parameters but only 16 billion activated per inference, a design that reduces compute cost while retaining large capacity. It supports a 512K-token context and processes text, images, video, and audio, and it is trained with a new reinforcement learning method called TEMPO that uses self-critiquing and test-time value estimation for long-horizon agent tasks. The release also introduces two new real-world agent benchmarks, VibeSearchBench and VibeLifeBench, alongside open weights on Hugging Face and GitHub.

**「Impact」** Developers and researchers now have access to a large-scale open MoE from a major consumer platform, with multimodal input and a long 512K context, which should enable experimentation on long-document and agentic tasks at lower inference cost than a dense 280B model. The new TEMPO training method and the VibeSearchBench and VibeLifeBench benchmarks also provide a concrete recipe and evaluation tools for building and assessing real-world long-horizon agents.

<details><summary>References</summary>
<ul>
<li><a href="https://www.besthub.dev/articles/open-source-dots3-note-from-imo-full-score-math-to-real-world-long-term-tasks-0b606f67d951">Open‑Source Dots3‑Note: From IMO Full‑Score Math to Re… | BestHub</a></li>
<li><a href="https://github.com/studio-dots-ai/dots3-note-prev">GitHub - studio-dots-ai/dots3-note-prev: dots3 note preview</a></li>
<li><a href="https://huggingface.co/dots-studio/dots3-note-prev">dots-studio/dots3-note-prev · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#MoE`, `#large language models`, `#reinforcement learning`, `#benchmarks`

---

<a id="item-tech-news-5"></a>
### [PostgreSQL Patches High-Risk to\_char RCE Vulnerability CVE-2026-14669](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL disclosed and patched CVE-2026-14669, a high-severity heap buffer overflow in the to\_char\(timestamptz\) function triggered by overly long POSIX timezone abbreviations. The flaw allows database users with low-privileged accounts to execute arbitrary code with the operating-system permissions of the PostgreSQL service process. It has a CVSS score of 8.8, but it is not exploitable without authentication and requires a low-privilege database account. Affected versions are those before PostgreSQL 18.5, 17.11, 16.15, 15.19, and 14.24. Because 18.5 was not released due to a regression, 18-series users should upgrade directly to 18.6, while other users should upgrade to 17.11, 16.15, 15.19, or 14.24; the minor update requires only replacing program files and restarting the service, not dumping the database or running pg\_upgrade.

telegram · zaihuapd · Aug 14, 14:35

**「Background」** PostgreSQL&\#x27;s to\_char function converts timestamps into formatted strings, and its timestamptz variant processes timezone abbreviations when formatting timestamp-with-time-zone values. POSIX timezone abbreviations can be defined as long strings, and the heap buffer overflow occurs when such an overly long abbreviation is handled. Memory-safety issues of this kind can let malformed input be turned into arbitrary code execution within the database server process.

**「Impact」** Organizations running affected PostgreSQL versions should upgrade to 18.6, 17.11, 16.15, 15.19, or 14.24 depending on their major version, because the flaw can let a low-privileged database user take over the database server&\#x27;s operating-system account. The update is straightforward since it requires only a binary replacement and restart, with no database dump or pg\_upgrade needed.

**Tags**: `#postgresql`, `#security`, `#CVE`, `#database`, `#vulnerability`

---

<a id="item-tech-news-6"></a>
### [Why Opus 5&\#x27;s Agent-Focused Post-Training May Make It Feel Worse](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 7.0/10

A blog post and Hacker News discussion argue that Anthropic&\#x27;s Opus 5 feels worse to work with, speculating that its post-training now optimizes communication for other AI agents rather than human users. Commenters report that Opus 5 writes elliptically and abstractly, uses inanimate subjects, and repeatedly &\#x27;confesses&\#x27; mistakes, making interaction exhausting despite greater capability. Some users say they have switched to older models such as Claude 4.8 or to OpenAI&\#x27;s Sol to keep working. The debate suggests that as frontier models are increasingly tuned for agentic workflows, human readability may be deprioritized in ways that affect everyday use.

hackernews · numeri · Aug 14, 10:12 · [Discussion](https://news.ycombinator.com/item?id=49296740)

**「Background」** Claude Opus 5 is Anthropic&\#x27;s flagship Claude model, released on July 24, 2026, and positioned as a strong agentic coding model built for long-running, multi-step work. It is the successor to Opus 4.8 and is designed to deeply understand codebases and hold context across complex tasks. Its post-training appears optimized for agentic use cases, which may be why its communication style feels different to human users compared with earlier models.

**「Community Discussion」** Commenters largely agree with the &\#x27;agent-speak&\#x27; hypothesis, sharing concrete complaints about Opus 5&\#x27;s elliptical phrasing and exhausting meta-commentary, with at least two users reporting migration away from it \(back to Claude 4.8 or to OpenAI&\#x27;s Sol\). One comment quotes a particularly abstract Opus 5 line as evidence of the style problem, while another notes the model is &\#x27;definitely more capable&\#x27; but still off-putting.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/claude/opus">Claude Opus \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#language models`, `#user experience`, `#LLM communication`

---

<a id="item-tech-news-7"></a>
### [RustDesk adds true unattended remote access on Wayland](https://rustdesk.com/blog/unattended-remote-access-wayland/) ⭐️ 7.0/10

According to the RustDesk blog, RustDesk now supports true unattended remote access on Wayland, a significant improvement for Linux remote desktop users. The feature lets users connect to Wayland-based systems without requiring someone at the remote session to interact with the login screen or authorize the connection. This matters because Wayland&\#x27;s security model previously made such unattended remote control difficult for many remote desktop tools. The update addresses a practical limitation for administrators and users managing always-on or remote Linux machines.

hackernews · rustdesk · Aug 14, 16:12 · [Discussion](https://news.ycombinator.com/item?id=49300759)

**「Background」** Wayland is a display server protocol for Linux that restricts applications from capturing the screen or injecting input without explicit user permission, which has made remote-desktop support difficult. RustDesk is a remote-desktop application; previously, unattended sessions on Wayland required someone at the remote machine to approve each connection or required a workaround such as enabling display-manager autologin and locking the screen automatically. The RustDesk blog now reports that RustDesk supports true unattended remote access on Wayland, removing the need for such per-session approval.

**「Impact」** Linux administrators and users running RustDesk on Wayland can now set up persistent remote access without an attended local session, which is especially useful for headless or always-on systems.

**「Community discussion」** Commenters were positive about the fix, with one saying they encountered this exact limitation two days earlier and were glad to see it resolved. Other discussion noted remaining gaps and questions: RustDesk reportedly still lacks encrypted connections when self-hosting, and users asked how it compares with VNC, Remmina over SSH/Tailscale, and whether it would be faster than VNC for controlling a Raspberry Pi connected to a TV.

<details><summary>References</summary>
<ul>
<li><a href="https://rustdesk.com/blog/unattended-remote-access-wayland/">Unattended Remote Access on Wayland with RustDesk — RustDesk</a></li>
<li><a href="https://www.andotech.net/taming-rustdesk-on-wayland-how-to-fix-screensharing-and-input-issues/">Fix RustDesk on Wayland: Screen &amp; Input – AndoTech.net</a></li>

</ul>
</details>

**Tags**: `#RustDesk`, `#Wayland`, `#remote desktop`, `#Linux`, `#open source`

---

<a id="item-tech-news-8"></a>
### [Firefox is now the last major browser supporting uBlock Origin](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 7.0/10

Firefox has become the only major browser that still supports uBlock Origin, according to PCWorld. The change means users of Chromium-based browsers can no longer install the original uBlock Origin extension, which relies on APIs that browser vendors are phasing out or restricting under the Manifest V3 extension framework. Mozilla&\#x27;s continued support preserves full uBlock Origin functionality in Firefox, while competing browsers are left with less capable alternatives such as uBlock Origin Lite. The shift underscores how Manifest V3 changes are reshaping ad-blocking and privacy tools across the web ecosystem.

hackernews · DemiGuru · Aug 14, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49303202)

**「Background」** Google&\#x27;s Manifest V3 extension specification restricts the capabilities of browser extensions, particularly ad blockers that rely on blocking network requests before a page loads. As Chromium-based browsers—including Chrome, Edge, and others—transitioned to Manifest V3 and began disabling older extensions like uBlock Origin, Firefox has continued to support the full version of uBlock Origin, making it the last major browser where the original extension remains fully functional.

**「Impact」** Users who want to keep using the classic uBlock Origin extension must switch to Firefox, because Chromium-based browsers no longer support the full extension under Manifest V3.

**「Community discussion」** Some commenters defended Mozilla&\#x27;s extension vetting and warned that abandoning Firefox for volunteer-maintained forks could harm the ecosystem. Others criticized Google&\#x27;s Manifest V3 direction and shared early experiences with uBlock Origin Lite, with one user saying they had not noticed any ad-blocking deficiencies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html">Firefox is now the last major browser that still supports ...</a></li>
<li><a href="https://www.ofzenandcomputing.com/ublock-origin-is-no-longer-available-for-chrome-but-you-can-still-use-it-on-firefox/">uBlock Origin Chrome vs Firefox in 2026: Complete Migration Guide</a></li>

</ul>
</details>

**Tags**: `#web browsers`, `#ad blocking`, `#privacy`, `#uBlock Origin`, `#Firefox`

---

<a id="item-tech-news-9"></a>
### [torch-preflight: A New Linter for PyTorch Training Bugs and VRAM Estimates](https://www.reddit.com/r/MachineLearning/comments/1vo8vv0/a_linter_for_pytorch_torchpreflight_p/) ⭐️ 7.0/10

torch-preflight is a new linter that statically analyzes PyTorch training scripts to catch common GPU-hour-wasting bugs without importing or executing the code, so no GPU or torch install is required. It currently implements 13 rules, covering issues such as loss.append\(loss\) holding autograd graphs, missing zero\_grad\(\) in training loops, gradient accumulation without dividing the loss, and DDP usage without DistributedSampler. The tool also estimates VRAM usage for a given training script and GPU, reporting whether the run fits and listing changes with the GiB each one saves; the author reports memory estimates land within 4% of measured peaks from four models on one T4. It is available via pip install torch-preflight, with the repository at github.com/highwaterlabs/torch-preflight. The project is still a work in progress, has been tested primarily against the PyTorch source tree, and is open to contributions and feedback.

reddit · r/MachineLearning · /u/LeJanbandhu · Aug 14, 14:30

**「Background」** A linter is a static analysis tool that inspects source code for potential errors without running it. PyTorch training scripts often contain subtle mistakes that waste GPU hours, such as accidentally retaining autograd graphs through Python list appends, forgetting to call zero\_grad\(\), or misusing distributed data parallelism; these bugs are hard to spot manually and can be costly when discovered only after training starts.

**「Impact」** For PyTorch developers who train models on rented GPU instances, torch-preflight offers a practical way to catch expensive bugs and estimate memory requirements before paying for compute, potentially saving both time and money. However, its effectiveness is not yet independently validated, with the author noting limited test coverage and the need to gather feedback on false positives and memory accuracy.

**Tags**: `#PyTorch`, `#linter`, `#debugging`, `#machine-learning`, `#VRAM-estimation`

---

<a id="item-tech-news-10"></a>
### [US Court Orders Google to Remove Play Store Hurdles for Third-Party App Stores](https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/) ⭐️ 7.0/10

U.S. District Judge James Donato has ordered Google to simplify installation of rival Android app stores by removing extra warning steps and prompts from the Play Store, with a one-week deadline. The court found that multi-step flows—such as requiring users to tap “view” before an “install” button appears—were deliberately designed anti-competitive friction meant to discourage ordinary users. The ruling comes from the Epic v. Google antitrust case, following a jury verdict that Google illegally monopolized Android app distribution. Under the order, installing a third-party app store must become as direct as installing a regular Android app, which could lower barriers for alternative app stores and affect Android developers and users.

telegram · zaihuapd · Aug 14, 09:55

**「Context」** Epic Games v. Google is an antitrust case in which Epic accused Google of illegally monopolizing Android app distribution through the Play Store. A jury found Google liable, and the court imposed remedies requiring Google to ease access to competing app stores. Part of that remedy involves removing deliberately added warning prompts and extra installation steps for third-party app stores.

**「Impact」** Google must remove extra warning steps for third-party app store installation within one week, reducing anti-competitive friction and making rival stores more accessible to Android users. The change could increase visibility for stores such as Aptoide, which is currently the only third-party store listed in Google Play&\#x27;s new page.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://www.theverge.com/policy/979852/that-is-not-acceptable-judge-orders-google-to-make-rival-app-store-installs-easier">&#x27;That is not acceptable&#x27;: Judge orders Google to make rival app store ...</a></li>
<li><a href="https://arstechnica.com/gadgets/2026/08/google-ordered-to-make-it-easier-to-download-alternative-android-app-stores/">Judge gives Google one week to fix &quot;anticompetitive&quot; app store download ...</a></li>
<li><a href="https://www.androidauthority.com/google-play-store-remove-third-party-app-store-friction-3698697/">Google ordered to remove Android app store warning screens</a></li>
<li><a href="https://arstechnica.com/gadgets/2026/08/third-party-app-stores-are-rolling-out-in-google-play-but-theres-only-one-right-now/">Following Epic loss, Google has started hosting rival app stores in the...</a></li>

</ul>
</details>

**Tags**: `#Android`, `#antitrust`, `#Google Play Store`, `#app distribution`, `#legal`

---

<a id="item-tech-news-11"></a>
### [Apple Trains China-Exclusive AI Model with Alibaba Support](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 7.0/10

Apple is training a large language model specifically for the Chinese market with support from Alibaba, according to Reuters, marking a shift from its previous reliance on third-party models. The China-specific model is expected to power Apple Intelligence when it launches in the country via an iOS update in the coming months. China&\#x27;s Cyberspace Administration registered the generative AI service last month, and if approved, Apple would become the first foreign company authorized to offer its own AI model in China. The move aims to give Apple greater control over the AI experience for Chinese users.

telegram · zaihuapd · Aug 14, 14:47

**「Background」** Apple Intelligence is Apple&\#x27;s suite of AI features that has not yet launched in China, where generative AI services require registration with the Cyberspace Administration of China \(CAC\). Historically, Apple relied on third-party models in China to comply with local regulations; a China-specific model would give it more control over the experience.

**「Impact」** If approved, Apple would become the first foreign company permitted to offer its own AI model in China, giving Chinese iPhone users a directly controlled AI experience and potentially setting a precedent for other foreign tech firms.

**Tags**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Regulation`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [DSpark adaptive verification makes vLLM speculative decoding load-aware](https://vllm.ai/blog/2026-08-14-dspark-adaptive-verification) ⭐️ 9.0/10

rss · vLLM Blog · Aug 14, 00:00

**「Background」** Speculative decoding buys fewer decode steps with extra compute; that is nearly free at low batch size, but at high concurrency rejected draft tokens compete with real tokens and can cut throughput. Since acceptance decays per position and varies with load, no fixed speculation length is optimal across concurrency.

**「Solution」** DSpark adds a learned confidence head per drafted token and vLLM turns it into adaptive verification \(PR \#47808\). The scheduler converts confidences into survival probabilities, then picks the global top-B draft slots across requests—so a confident request&\#x27;s later token can beat a weak request&\#x27;s early one. B maximizes expected tokens per microsecond using a cumulative-sum numerator and profiled cost tables, computed on the CPU from one-step-old double-buffered confidences while allocation runs on the GPU against current values via torch.compile/Triton. New varlen decode CUDA graphs, enabled by DeepGEMM&\#x27;s varlen indexer, support variable verification sizes. The startup cost profile is median-of-five and forced monotonic; cudagraph padding makes costs a staircase and the jump outside the capture region encourages staying inside it. On DeepSeek-V4-Pro-0813 \(8×B300, TP=8, concurrency 1–256\), adaptive verification stays on the Pareto frontier with num\_speculative\_tokens=7, behaving like a long block at low concurrency and a short one at high concurrency. Eager mode, LoRA, pipeline parallelism, and output logprobs are unsupported.

**「Takeaway」** The post&\#x27;s core point is that speculation length should be a runtime decision rather than a deployment constant: confidence-scheduled verification extends speculative decoding&\#x27;s benefit across load while removing per-workload tuning, making it an easier on-by-default win.

**Tags**: `#speculative decoding`, `#vLLM`, `#adaptive verification`, `#CUDA graphs`, `#performance engineering`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Apple Proposes App Store External Purchase Commissions of Up to 15%](https://9to5mac.com/2026/08/13/apple-proposes-commissions-of-up-to-15-for-off-app-store-purchases-in-the-us/) ⭐️ 8.0/10

Apple has proposed in a U.S. court filing that App Store developers pay commissions of up to 15% for purchases made outside the App Store: 15% for standard apps, 10% for video and news partner projects and subscription renewals, and 5% for apps in the Small Business Program.

telegram · zaihuapd · Aug 14, 02:33

**「Background」** The filing is part of the Epic Games v. Apple antitrust dispute over App Store payment rules, after the U.S. Supreme Court declined to halt lower-court proceedings on the fee structure.

**「Impact」** If approved, the tiered rates would directly determine what U.S. App Store developers pay when customers complete purchases outside Apple’s payment system, with smaller developers in the Small Business Program paying the lowest rate.

**Tags**: `#Apple`, `#App Store`, `#antitrust`, `#Epic Games`, `#regulation`

---

<a id="item-finance-news-2"></a>
### [Berkshire Hathaway boosts Alphabet to top-three holding, ends net-selling streak](https://www.cnbc.com/2026/08/14/berkshire-hathaway-boosts-alphabet-to-a-top-three-holding-ups-delta-and-housing-bets.html) ⭐️ 7.0/10

Berkshire Hathaway increased its stake in Alphabet, Google’s parent, by 83% from the prior quarter to about 106 million shares worth $37.9 billion at the end of June, making it the third-largest U.S.-listed equity holding by market value, according to a regulatory filing. Berkshire also became a net buyer of stocks in the second quarter, with nearly $20 billion in net purchases, after 14 straight quarters of net selling.

rss · CNBC Finance · Aug 14, 21:06

**「Background」** The Alphabet increase largely reflects a $10 billion private stock purchase announced in early June, when Alphabet sought fresh capital to finance its artificial-intelligence infrastructure buildout.

**Tags**: `#Berkshire Hathaway`, `#Alphabet`, `#Delta Air Lines`, `#Homebuilders`, `#Portfolio Management`

---

<a id="item-finance-news-3"></a>
### [Goldman Sachs profits from underwriting AI infrastructure boom](https://www.cnbc.com/2026/08/14/goldmans-latest-cash-cow-is-all-about-funding-the-ai-infrastructure-boom.html) ⭐️ 7.0/10

Goldman Sachs is earning fees from funding the AI infrastructure boom, serving as a lead underwriter in Intel’s $20 billion stock sale and Alphabet’s $85 billion stock sale, while joining a non-binding Nvidia plan to raise $500 billion from six financial institutions for AI computing infrastructure.

rss · CNBC Finance · Aug 14, 20:05

**「Background」** Goldman Sachs is a major underwriter and facilitator for large AI-related capital raises. This week Nvidia announced a plan for Goldman and five other firms to help raise $500 billion in financing for AI infrastructure, and Intel launched a $20 billion stock offering \(upsized from $15 billion\) that Goldman is helping manage. Goldman also helped Alphabet sell $85 billion in stock in June. As a joint book-running manager, Goldman earns fees from structuring, underwriting, and placing these offerings.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/08/14/goldmans-latest-cash-cow-is-all-about-funding-the-ai-infrastructure-boom.html">Goldman’s latest cash cow is all about funding the AI infrastructure boom</a></li>

</ul>
</details>

**Tags**: `#Goldman Sachs`, `#AI infrastructure`, `#investment banking`, `#stock offering`, `#Nvidia`

---

<a id="item-finance-news-4"></a>
### [Premarket Movers: Reddit Jumps on S&amp;P 500 Inclusion; Applied Materials Drops After Earnings](https://www.cnbc.com/2026/08/14/stocks-making-the-biggest-moves-premarket-rddt-amat-sndk-w.html) ⭐️ 7.0/10

Reddit surged 12% premarket after S&amp;P Dow Jones Indices said it will join the S&amp;P 500 on Aug. 18, while Applied Materials fell more than 5% after reporting second-quarter adjusted earnings of $3.50 per share on revenue of $9.12 billion.

rss · CNBC Finance · Aug 14, 10:46

**「Background」** The S&amp;P 500 is a widely followed U.S. stock benchmark, and inclusion can prompt buying by index-tracking funds. Applied Materials&\#x27; semiconductor systems sales came in at $7.04 billion, only slightly above a FactSet consensus of $6.96 billion.

**Tags**: `#S&amp;P 500`, `#Earnings`, `#Mergers and Acquisitions`, `#Semiconductors`, `#Media`

---

<a id="item-finance-news-5"></a>
### [CITIC Trustar Near $1.5 Billion Deal for Alibaba Gaming Unit Lingxi](https://www.bloomberg.com/news/articles/2026-08-14/trustar-is-said-to-near-1-5-billion-deal-for-alibaba-gaming-arm) ⭐️ 7.0/10

Bloomberg reports that CITIC Group’s private equity arm Trustar Capital is close to buying Alibaba’s gaming unit Lingxi at a valuation that could top $1.5 billion, although talks are still ongoing and not final.

telegram · zaihuapd · Aug 14, 10:24

**「Background」** Lingxi, whose flagship game was co-developed with Japan’s Koei Tecmo, is among assets Alibaba is divesting as CEO Wu Yongming sharpens the company’s focus on AI and cloud computing.

**Tags**: `#M&amp;A`, `#Alibaba`, `#Gaming`, `#Private Equity`, `#Divestiture`

---