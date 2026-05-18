## Table of Contents
- [Apr 13 ~ Apr 19](#apr-13--apr-19)
- [Apr 6 ~ Apr 12](#apr-6--apr-12)
- [Mar 30 ~ Apr 5](#mar-30--apr-5)
- [Mar 23 ~ Mar 29](#mar-23--mar-29)
- [Mar 16 ~ Mar 22](#mar-16--mar-22)
- [Mar 9 ~ Mar 15](#mar-9--mar-15)
- [Mar 2 ~ Mar 8](#mar-2--mar-8)
- [Feb 23 ~ Mar 1](#feb-23--mar-1)
- [Feb 16 ~ Feb 22](#feb-16--feb-22)
- [Feb 9 ~ Feb 15](#feb-9--feb-15)
- [Feb 2 ~ Feb 8](#feb-2--feb-8)
- [Jan 26 ~ Feb 1](#jan-26--feb-1)
- [Jan 19 ~ Jan 25](#jan-19--jan-25)
- [Jan 12 ~ Jan 18](#jan-12--jan-18)
- [Jan 5 ~ Jan 11](#jan-5--jan-11)
- [Dec 29 ~ Jan 4](#dec-29--jan-4)
- [Dec 22 ~ Dec 28](#dec-22--dec-28)
- [Dec 15 ~ Dec 21](#dec-15--dec-21)
- [Dec 8 ~ Dec 14](#dec-8--dec-14)
- [Dec 1 ~ Dec 7](#dec-1--dec-7)
- [Nov 24 ~ Nov 30](#nov-24--nov-30)
- [Nov 17 ~ Nov 23](#nov-17--nov-23)
- [Nov 10 ~ Nov 16](#nov-10--nov-16)
- [Nov 3 ~ Nov 9](#nov-3--nov-9)
- [Oct 27 ~ Nov 2](#oct-27--nov-2)
- [Oct 20 ~ Oct 26](#oct-20--oct-26)
- [Oct 13 ~ Oct 19](#oct-13--oct-19)
- [Oct 6 ~ Oct 12](#oct-6--oct-12)
- [Sep 29 ~ Oct 5](#sep-29--oct-5)
- [Sep 22 ~ Sep 28](#sep-22--sep-28)
- [Sep 15 ~ Sep 21](#sep-15--sep-21)
- [Sep 8 ~ Sep 14](#sep-8--sep-14)
- [Sep 1 ~ Sep 7](#sep-1--sep-7)
- [Aug 25 ~ Aug 31](#aug-25--aug-31)
- [Aug 18 ~ Aug 24](#aug-18--aug-24)
- [Aug 11 ~ Aug 17](#aug-11--aug-17)
- [Aug 4 ~ Aug 10](#aug-4--aug-10)
- [Jul 28 ~ Aug 3](#jul-28--aug-3)
- [Jul 21 ~ Jul 27](#jul-21--jul-27)
- [Jul 14 ~ Jul 20](#jul-14--jul-20)
- [Jul 7 ~ Jul 13](#jul-7--jul-13)
- [Jun 30 ~ Jul 6](#jun-30--jul-6)
- [Jun 23 ~ Jun 29](#jun-23--jun-29)
- [Jun 16 ~ Jun 22](#jun-16--jun-22)
- [Jun 9 ~ Jun 15](#jun-9--jun-15)
- [Jun 2 ~ Jun 8](#jun-2--jun-8)
<br><br>



## Apr 13 ~ Apr 19
### Apr 17
- [Open-source] Ant Lingbo (灵波) open-sourced the streaming 3D reconstruction model Lingbo-Map, which uniquely runs on only an ordinary RGB camera. The model uses pure autoregressive modeling with a Geometric Context Attention (GCA) mechanism to achieve "see-and-build" real-time camera pose estimation and 3D scene reconstruction at approximately 20 FPS inference speed. As a key piece of embodied intelligence, it supports long-sequence continuous reasoning without accuracy degradation, providing stable spatial perception for robot navigation, obstacle avoidance, and interaction. See
https://www.modelscope.cn/models/Robbyant/lingbot-map

### Apr 16
- [Closed-source] Anthropic released Claude Opus 4.7, its most powerful generally available model to date, focused on complex reasoning and agentic coding. Pricing remains consistent with Opus 4.6 ($5/$25 per million tokens). The update includes capability improvements, new features, and a brand-new tokenizer; note there are API breaking changes relative to Opus 4.6. Claude Opus 4.7 and Haiku 4.5 are also available on a self-serve basis to all customers across 27 AWS regions on Amazon Bedrock. See
https://www.anthropic.com/news/claude-opus-4-7
Try it in China: https://nonelinear.com/static/models.html

### Apr 15
- [Open-source] Alibaba open-sourced Qwen3.6-35B-A3B, the first open-weight release of the Qwen3.6 series under the Apache 2.0 license. A sparse MoE model with 35B total parameters and only 3B activated, its agentic coding capabilities significantly surpass the previous generation Qwen3.5-35B-A3B. It natively supports 262K context, extendable to 1010K, and supports both multimodal thinking and non-thinking modes. See
https://qwen.ai/blog?id=qwen3.6-35b-a3b
Try it directly: https://nonelinear.com/static/models.html
- [Closed-source] Google launched the Gemini 3.1 Flash TTS preview text-to-speech model, focused on being economical, expressive, and controllable, offering developers cost-effective speech synthesis. See
https://ai.google.dev/gemini-api/docs/models/gemini-3.1-flash-tts-preview
- [Closed-source] The xAI Speech to Text API officially launched GA, supporting audio transcription in 25 languages, with both batch processing and streaming modes to meet diverse speech recognition needs. See
https://docs.x.ai/developers/model-capabilities/audio/speech-to-text

### Apr 14
- [Open-source] Baidu open-sourced the text-to-image generation model ERNIE-Image, based on a single-stream Diffusion Transformer (DiT) architecture. With only 8B parameters, it reaches industry-leading levels among open-weight text-to-image models. The model includes a built-in lightweight prompt enhancer that expands short inputs into structured descriptions. It excels at complex instruction following, text rendering, and structured image generation, particularly suited for commercial posters, comics, multi-panel layouts, and other controllability-demanding content creation scenarios. See
https://modelscope.cn/models/PaddlePaddle/ERNIE-Image
- [Closed-source] Google released an updated robotics model gemini-robotics-er-1.6-preview, adding musical instrument reading capability with significantly enhanced spatial and physical reasoning, further advancing embodied intelligence perception and decision-making in the real physical world. See
https://deepmind.google/blog/gemini-robotics-er-1-6/
<br><br>
## Apr 6 ~ Apr 12
### Apr 10
- [Open-source] Tencent Hunyuan and the Robotics X Lab jointly released the HY-Embodied-0.5 embodied intelligence model series, including two flagship models: MoT-2B targeting on-device deployment and real-time response, and MoE-32B pursuing complex reasoning and peak performance. See
https://modelscope.cn/models/Tencent-Hunyuan/HY-Embodied-0.5

### Apr 8
- [Closed-source] Anthropic launched the Claude Managed Agents public beta, a fully managed agent runtime framework that supports running Claude as an autonomous agent with secure sandboxing, built-in tools, and server-side event streaming. Developers can create agents, configure containers, and run sessions via the API; all endpoints require the managed-agents-2026-04-01 beta header. See
https://platform.claude.com/docs/en/managed-agents/overview

### Apr 7
- [Closed-source] Anthropic announced Claude Mythos Preview as part of Project Glasswing, opened to defensive cybersecurity work as an invite-only research preview. The project unites 12 giants including AWS, Apple, Google, Microsoft, and NVIDIA, dedicated to using frontier AI to protect critical software infrastructure. Claude Mythos Preview has already discovered thousands of high-severity vulnerabilities, including security defects in all major operating systems and browsers. See
https://www.anthropic.com/glasswing

### Apr 6
- [Open-source] Zhipu GLM released GLM-5.1, a new generation flagship agentic engineering model with a substantial leap in coding ability over its predecessor. It achieves SOTA on SWE-Bench Pro and significantly leads GLM-5 on NL2Repo and Terminal-Bench 2.0. Built for long-horizon agent tasks, it shows better judgment on ambiguous problems and continuously improves over hundreds of interaction rounds and thousands of tool calls — the longer it runs, the better the results. See
https://docs.bigmodel.cn/cn/guide/models/text/glm-5.1
Try it directly: https://nonelinear.com/static/models.html
<br><br>
## Mar 30 ~ Apr 5
### Apr 4
- [Open-source] JD.com open-sourced JoyAI-Image-Edit, a multimodal foundation model focused on instruction-guided image editing. Through a unified MLLM-MMDiT architecture, it unifies understanding, generation, and editing. It features strong spatial understanding (scene parsing, relational localization, instruction decomposition), supports high-quality long-text typography, multi-view generation, and structure-preserving controllable editing. See
https://modelscope.cn/models/jd-opensource/JoyAI-Image-Edit

### Apr 2
- [Open-source] Google released the Gemma 4 series of open-source models (gemma-4-26b-a4b-it, gemma-4-31b-it), built on the same research and tech stack as Gemini 3, spanning the full hardware range from phones to workstations. They support 140+ languages, text/image/video multimodal input, and built-in toggleable thinking mode. The entire series uses the Apache 2.0 license. See
https://ai.google.dev/gemma/docs/core?hl=zh-cn
Try it in China: https://nonelinear.com/static/models.html
- [Closed-source] Alibaba released Qwen3.6-Plus, the Tongyi Qianwen (Qwen) 3.6-Plus model, with major upgrades to code development capabilities (agentic coding, frontend programming, etc.) and significantly improved Vibe Coding experience; further enhanced general scenario reasoning; substantially improved multimodal recognition, OCR, and object localization; and fixes for known issues from Qwen3.5-Plus. See
https://help.aliyun.com/zh/model-studio/text-generation
Try it directly: https://nonelinear.com/static/models.html

### Apr 1
- [Closed-source] Alibaba released the Wanxiang 2.7 image generation and editing models (wan2.7-image-pro, wan2.7-image), supporting text-to-image, text-to-image-group, image-to-image-group, image editing, multi-image reference generation, and interactive editing. They perform better in text rendering, subject consistency, and complex instruction following. The Pro series supports 4K output; the accelerated version balances quality and response speed. See
https://help.aliyun.com/zh/model-studio/wan-image-generation-and-editing-api-reference
Try it directly: https://nonelinear.com/static/models.html
- [Open-source] Alibaba Tongyi Lab open-sourced the CoPaw-Flash series, lightweight models deeply optimized for CoPaw autonomous agent scenarios. Fine-tuned specifically for CoPaw tasks from the training stage, trained on high-quality agent trajectory data sampled from real CoPaw environments at scale, they exhibit stronger Agent performance in tool calling, command execution, memory management, and multi-step planning. Core features include active memory management, native file parsing, efficient information search, and intelligent guidance. See
https://modelscope.cn/collections/AgentScope/CoPaw-Flash
<br><br>
## Mar 23 ~ Mar 29
### Mar 26
- [Closed-source] Google released gemini-3.1-flash-live-preview, the latest generation audio-to-audio (A2A) model designed for real-time conversation and voice-first AI applications. Access via the Live API. See
https://ai.google.dev/gemini-api/docs/models/gemini-3.1-flash-live-preview

### Mar 25
- [Closed-source] Google released the Lyria 3 music generation model series: lyria-3-clip-preview (generates 30-second music clips) and lyria-3-pro-preview (generates complete songs). Both support text and image input and can produce high-quality 48kHz stereo audio. See
https://ai.google.dev/gemini-api/docs/music-generation

### Mar 24
- [Open-source] Alibaba Tongyi Lab open-sourced PrismAudio, a powerful video-to-audio (V2A) model. With only 518M parameters and 0.63s inference latency, it comprehensively surpasses existing 5B-scale methods across semantic, temporal, aesthetic, spatial, and subjective scoring. PrismAudio is the first V2A generation framework to combine reinforcement learning (RL) with specialized chain-of-thought (CoT) planning, decomposing reasoning into four specialized CoT modules — semantic, temporal, aesthetic, and spatial — each with its own reward function, guiding the model to improve reasoning quality from multiple viewpoints simultaneously. See
https://www.modelscope.cn/models/iic/PrismAudio

### Mar 23
- [Open-source] Mistral released Voxtral TTS (voxtral-tts-2603), its latest generation text-to-speech model, supporting zero-shot voice cloning, multilingual output, and real-time streaming generation, producing high-quality 48kHz stereo audio. Built on a 4B parameter core architecture, Apache 2.0 open-source. See
https://huggingface.co/mistralai/Voxtral-4B-TTS-2603
<br><br>
## Mar 16 ~ Mar 22
### Mar 18
- [Closed-source] MiniMax released MiniMax M2.7, the first commercial model to deeply participate in its own training iteration. Through building an Agent Harness, the model autonomously completes over 100 iteration loops (including failure analysis, code modification, and evaluation comparison), shouldering 30%-50% of the workload in some R&D scenarios, with internal evaluations improving by about 30%. It is globally launched on MiniMax Agent and the open platform, with API pricing matching M2.5. See
https://www.minimaxi.com/news/minimax-m27-zh
Try it directly: https://nonelinear.com/static/models.html
- [Closed-source] Xiaomi released Xiaomi MiMo-V2-Pro, a flagship base Model for the Agent era. Trillion-parameter scale with 1T total and 42B activated, using an innovative hybrid attention architecture (7:1 ratio) and supporting 1M ultra-long context. Previously tested anonymously under the codename "Hunter Alpha", its call volume surpassed 1T tokens and it topped OpenRouter's daily leaderboard for multiple days. See
https://mimo.xiaomi.com/mimo-v2-pro
Try it directly: https://nonelinear.com/static/models.html
- [Closed-source] Xiaomi released Xiaomi MiMo-V2-Omni, an omni-modal base model for the Agent era. Natively omni-modal perception supports precise cross-modal understanding of images, video, audio, and text, with native Agent and Browser Use capabilities — a foundation toward embodied intelligence. Ranked #1 in Pinchbench average during the Healer Alpha testing period. See
https://mimo.xiaomi.com/mimo-v2-omni
Try it directly: https://nonelinear.com/static/models.html
- [Closed-source] Xiaomi released Xiaomi MiMo-V2-TTS, a versatile voice agent base model that can speak and sing. End-to-end speech generation architecture built on a proprietary Audio Tokenizer and multi-codebook speech modeling, enabling more refined speech feature capture and reconstruction. Pre-trained at massive scale on hundreds of millions of hours of speech across diverse speaking styles and scenarios. Multi-dimensional reinforcement learning training delivers highly human-like, expressive speech generation, with unique abilities including singing and dialects (Sichuanese / Henanese / Cantonese / Taiwanese accent, etc.). See
https://mimo.xiaomi.com/mimo-v2-tts
Try it directly: https://nonelinear.com/static/models.html

### Mar 17
- [Closed-source] OpenAI released GPT-5.4 Mini and GPT-5.4 Nano, positioned as "the most powerful small models to date", designed for coding, subagents, and high-throughput workloads. GPT-5.4 Mini is an efficient model designed for coding assistants, subagents, and high-throughput workloads, with significant improvements over GPT-5 Mini in coding, reasoning, multimodal understanding, and tool use, while running more than 2x faster. GPT-5.4 Nano is the smallest and cheapest version in the GPT-5.4 family, built for speed- and cost-first scenarios, recommended for classification, data extraction, ranking, and coding subagents handling simple auxiliary tasks. See
https://openai.com/zh-Hans-CN/index/introducing-gpt-5-4-mini-and-nano/
Try it in China: https://nonelinear.com/static/models.html

### Mar 16
- [Closed-source] Zhipu GLM released GLM-5-Turbo, the world's first base model deeply optimized for OpenClaw Longxia (龙虾) scenarios. Specialized optimization for core Longxia (龙虾) task needs began at the training stage, enhancing tool calling, instruction following, scheduled and persistent tasks, long-chain execution, and supporting a 200K context window. See
https://docs.bigmodel.cn/cn/guide/models/text/glm-5-turbo
Try it directly: https://nonelinear.com/static/models.html
- [Open-source] Mistral released Mistral Small 4 (mistral-small-2603), the latest in the Mistral Small series, which for the first time unifies Mistral Small (instruction following), Magistral (reasoning), Pixtral (multimodal), and Devstral (coding agent) into a single model. MoE architecture with 4 of 128 experts activated per token, 119B total parameters and only 6B activated, supporting a 256K context window. Supports configurable reasoning strength (reasoning_effort parameter), with end-to-end response time reduced 40% versus Small 3 and throughput improved 3x. Apache 2.0 open-source. See
https://mistral.ai/news/mistral-small-4
- [Open-source] Mistral released Leanstral, the world's first open-source Lean 4 code Agent, designed for formal mathematical proof verification, with 6B core parameters. Apache 2.0 open-source, supports the MCP protocol, can be used zero-config in Mistral Vibe, and provides a free Labs API. See
https://mistral.ai/news/leanstral

<br><br>
## Mar 9 ~ Mar 15
### Mar 13
- [Closed-source] Anthropic announced that the 1M-token context windows for Claude Opus 4.6 and Sonnet 4.6 are now generally available (GA) at standard pricing with no long-context premium. Media limits have been increased from 100 to 600 images or PDF pages, and dedicated 1M rate limits have been removed. No beta header required — requests exceeding 200K take effect automatically. See
https://platform.claude.com/docs/en/build-with-claude/context-windows

### Mar 10
- [Closed-source] xAI released Grok 4.20 Beta and Grok 4.20 Multi-agent Beta, now callable via the xAI Enterprise API. Grok 4.20 uses a 4-agent parallel collaboration architecture (Grok/Harper/Benjamin/Lucas), analyzing problems from multiple angles, then cross-validating and synthesizing output. Hallucination rate dropped from about 12% to about 4.2%. Multi-agent Beta supports deep research, coordinated tool calling, and cross-task information synthesis. See
https://docs.x.ai/developers/model-capabilities/text/multi-agent
Try it in China: https://nonelinear.com/static/models.html
- [Closed-source] Google released gemini-embedding-2-preview, Google's first natively multimodal embedding model. It supports text, image, video, audio, and PDF input, mapping all modalities to a unified embedding space. Supports 100+ languages, defaults to outputting 3072-dim vectors, with flexible scaling to 1536 or 768 dimensions. Now publicly in preview via the Gemini API and Vertex AI. See
https://ai.google.dev/gemini-api/docs/embeddings?hl=zh-cn
<br><br>
## Mar 2 ~ Mar 8
### Mar 5
- [Closed-source] OpenAI released GPT-5.4, OpenAI's latest flagship model. The first general-purpose model with built-in native Computer Use, capable of autonomously operating desktop applications and executing multi-step workflows. Supports up to 1M-token context, with reasoning token efficiency substantially better than GPT-5.2 and factual error rate reduced by 33%. Introduces Tool Search to intelligently find and invoke tools. See
https://openai.com/zh-Hans-CN/index/introducing-gpt-5-4/
Try it in China: https://nonelinear.com/static/models.html

### Mar 3
- [Closed-source] OpenAI released GPT-5.3 Instant, a major update to ChatGPT's daily-use model. Hallucination rate dropped 26.8% (when online), conversation tone more natural with less "preachiness" and unnecessary refusal, and web search result quality is substantially improved. Supports a 400K-token context window. See
https://openai.com/zh-Hans-CN/index/gpt-5-3-instant/
Try it in China: https://nonelinear.com/static/models.html
- [Closed-source] Google released Gemini 3.1 Flash-Lite Preview, the first Flash-Lite model in the Gemini 3 series, designed for large-scale, high-frequency scenarios. Priced at just $0.25 per million input tokens + $1.50 per million output tokens — 1/8 the cost of Pro. Output speed is 45% faster than 2.5 Flash, with 2.5x faster time-to-first-token. Supports 1M-token context and multimodal input. See
https://ai.google.dev/gemini-api/docs/models/gemini-3.1-flash-lite-preview
Try it in China: https://nonelinear.com/static/models.html
- [Closed-source] Alibaba released the qwen-image-2.0 series (qwen-image-2.0-2026-03-03, qwen-image-2.0-pro, qwen-image-2.0-pro-2026-03-03), the Qwen Image 2.0 series supporting both image generation and editing. The Pro series offers stronger text rendering, photorealism, and semantic adherence; the accelerated version balances quality and response speed. See
https://help.aliyun.com/zh/model-studio/qwen-image-api
https://help.aliyun.com/zh/model-studio/qwen-image-edit-api
Try it directly: https://nonelinear.com/static/models.html

### Mar 2
- [Closed-source] Alibaba released CosyVoice 3.5 (cosyvoice-v3.5-plus, cosyvoice-v3.5-flash), the CosyVoice 3.5 speech synthesis model is now launched, focused on voice cloning and design, supporting instruction-controlled speech synthesis. See
https://help.aliyun.com/zh/model-studio/text-to-speech

<br><br>
## Feb 23 ~ Mar 1
### Mar 1
- [Open-source] Alibaba released Qwen3.5-0.8B / 2B / 4B / 9B, the Qwen3.5 series on-device small model family officially open-sourced. Using native multimodal training + hybrid attention architecture, designed for mobile and edge devices. See
https://www.modelscope.cn/collections/Qwen/Qwen35
### Feb 26
- [Closed-source] Google released Gemini 3.1 Flash Image Preview (codename Nano Banana 2), an efficient version of Gemini 3 Pro Image, offering mainstream pricing and low-latency image generation. Key updates: supports 0.5K/2K/4K output resolutions (default 1K); image search grounding integrating text and image search results; new aspect ratios 1:4/4:1/1:8/8:1; improved image quality consistency and internationalized text rendering. See
https://ai.google.dev/gemini-api/docs/models/gemini-3.1-flash-image-preview
Try it in China: https://nonelinear.com/static/models.html

### Feb 25
- [Open-source] Alibaba Tongyi released the Qwen3.5 mid-scale series: Qwen3.5-Flash (production-grade hosted, default 1M context), Qwen3.5-35B-A3B (small but powerful, already surpassing Qwen3-235B-A22B), Qwen3.5-122B-A10B (flagship open-source), and Qwen3.5-27B (optimized for Agent scenarios). All models support vision-language multimodal input, native 256K context extendable up to 1M tokens. See
https://modelscope.cn/collections/Qwen/Qwen35
Try it directly: https://nonelinear.com/static/models.html
<br><br>
## Feb 16 ~ Feb 22
### Feb 20
- [Open-source] Alibaba released qwen3-coder-next, a new-generation open-source code generation model in the Qwen3 series. It supports multi-turn tool interactions and significantly improves repository-level code understanding and adaptability to various AI coding tools. See
https://help.aliyun.com/zh/model-studio/qwen-coder
### Feb 19
- [Closed-source] Google released the Gemini 3.1 Pro preview, the latest iteration in the all-new Gemini 3 series. It offers stronger reasoning, higher token efficiency, and a more grounded, factually consistent experience. The model is optimized for software engineering behaviors and usability, with particular reinforcement of agent workflows requiring precise tool use and reliable multi-step execution in real-world domains. See
https://ai.google.dev/gemini-api/docs/models/gemini-3.1-pro-preview?hl=zh-cn
Try it in China: https://nonelinear.com/static/models.html

### Feb 16
- [Open-source] Alibaba launched the latest model qwen3.5-plus, supporting text, image, and video multimodal input. The model performs excellently across tasks including language understanding, logical reasoning, code generation, agentic tasks, image understanding, video understanding, and graphical user interfaces (GUI), with built-in tool calling support. See
https://help.aliyun.com/zh/model-studio/text-generation
Try it directly: https://nonelinear.com/static/models.html
- [Open-source] Ant Group's inclusionAI team released the new instant-model benchmark Ling-2.5-1T, the most powerful non-thinking (instruction) model in the Bailing (Ling) family to date. Striking the optimal balance between efficiency and quality, it approaches frontier thinking-model reasoning with about 1/4 the token consumption. Fully open-source (MIT license). See
https://modelscope.cn/models/inclusionAI/Ling-2.5-1T

<br><br>
## Feb 9 ~ Feb 15
### Feb 14
- [Closed-source] ByteDance released the Doubao Seed2.0 series, with three general Agent models (Pro, Lite, Mini) plus a dedicated Code model. The series focuses on improved visual and multimodal understanding, with more accurate parsing of complex documents, tables, and video content, and substantially improved reliability for multi-constraint, long-chain complex instruction execution. See
https://seed.bytedance.com/zh/blog?order_desc=true&offset=12
Try it directly: https://nonelinear.com/static/models.html

- [Open-source] Xiaohongshu's FireRedTeam released FireRed-Image-Edit-1.0, a general-purpose image editing model. It comprehensively surpasses existing open-source solutions across multiple mainstream benchmarks and, on certain dimensions, even approaches closed-source commercial models such as Nano-Banana. See
https://modelscope.cn/models/FireRedTeam/FireRed-Image-Edit-1.0

### Feb 13
- [Closed-source] ByteDance launched Seedream 5.0 Lite, an intelligent image creation model, introducing "deep thinking" and real-time search augmentation. Through a unified multimodal architecture, it substantially improves text-image alignment accuracy and adherence to physical laws, understanding ambiguous instructions like a designer and combining timely information into creation. See
https://seed.bytedance.com/en/seedream5_0_lite
Try it directly: https://nonelinear.com/static/models.html

### Feb 12
- [Closed-source] OpenAI released GPT-5.3-Codex-Spark, the first ultra-fast model designed for real-time programming, optimized for Cerebras WSE-3 hardware. Inference speed exceeds 1000 tokens/s, supports 128k context, and via WebSocket delivers substantially reduced latency. On tests like SWE-Bench Pro, it combines extreme speed with strong logic, now open to ChatGPT Pro users in preview. See
https://openai.com/index/introducing-gpt-5-3-codex-spark/
Try it in China: https://nonelinear.com/static/models.html

- [Open-source] MiniMax released MiniMax M2.5, continuing the MoE architecture's high-concurrency advantage while significantly enhancing general reasoning and long-text processing depth. Specially optimized for multi-turn dialogue and complex logic scenarios, aiming to provide an enterprise-grade, cost-effective solution combining extreme speed and intelligence. See
https://minimaxi.com/news/minimax-m25
Try it directly: https://nonelinear.com/static/models.html

- [Open-source] Zhipu AI released GLM-5, a new-generation pretrained model with substantially improved mathematical-logic reasoning, code writing, and multimodal understanding. Supports ultra-long context, excels at instruction following and complex task planning, and is deeply adapted to various inference frameworks to lower deployment barriers. See
https://z.ai/blog/glm-5
Try it directly: https://nonelinear.com/static/models.html

- [Closed-source] ByteDance released the new-generation video creation model Seedance 2.0, using a unified multimodal architecture that supports mixed text, image, audio, and video input. Generation quality reaches SOTA, supports 15-second long video generation and dual-channel audio output, substantially improving industrial-grade controllability and consistency. See
https://seed.bytedance.com/seedance2_0
Try it directly: https://nonelinear.com/static/models.html

### Feb 11
- [Open-source] inclusionAI (an Ant Group team) released Ring-2.5-1T, an upgrade to Ring-1T, with core highlights "fast, deep, long". Generation efficiency improved more than 3x, memory access overhead reduced 10x; with IMO gold-medal-level deep thinking capability, and able to continuously work for 2 hours to write a mini operating system. Fully open-source (MIT license). See
https://modelscope.cn/models/inclusionAI/Ring-2.5-1T

<br><br>
## Feb 2 ~ Feb 8
### Feb 7
- [Closed-source] Anthropic launched a fast mode research preview for Opus 4.6, achieving notably faster output token generation via the speed parameter. Fast mode delivers up to 2.5x faster speeds at premium pricing; interested users can join the waitlist. See
https://platform.claude.com/docs/en/build-with-claude/fast-mode

### Feb 5
- [Closed-source] Anthropic released Claude Opus 4.6, the most intelligent model, designed for complex agentic tasks and long-horizon work. Opus 4.6 recommends adaptive thinking mode; manual thinking mode (with budget_tokens) is deprecated, and prefilled assistant messages are not supported. See
https://www.anthropic.com/news/claude-opus-4-6

- [Closed-source] OpenAI released GPT-5.3-Codex, the most powerful agentic coding model. It is the first to combine the Codex + GPT-5 training stack, fusing top-tier code generation, reasoning, and general intelligence in one. About 25% faster, setting new highs on key benchmarks, marking the leap from code generation to actively steerable general-purpose coding agents. See
https://openai.com/zh-Hans-CN/index/introducing-gpt-5-3-codex/

### Feb 3
- [Open-source] Zhipu AI released GLM-OCR, a multimodal OCR model for complex document understanding, based on the GLM-V encoder-decoder architecture. It introduces multi-token prediction (MTP) loss and stable full-task reinforcement learning, improving training efficiency, recognition accuracy, and generalization. With only 0.9B parameters, it scored 94.62 on OmniDocBench V1.5, ranking #1. Supports vLLM, SGLang, and Ollama deployment, significantly reducing inference latency and compute cost, suitable for high-concurrency services and edge deployment. See
https://huggingface.co/zai-org/GLM-OCR

### Feb 2
- [Closed-source] Alibaba released wan2.6-r2v-flash, which generates multi-shot videos based on reference video and image character likenesses, with automatic dubbing support. See
https://help.aliyun.com/zh/model-studio/wan-video-to-video-api-reference

- [Open-source] StepFun released Step 3.5 Flash, a 196B-parameter high-speed base model for Agents. Sparse MoE architecture with 196B total parameters but only 11B activated, supporting 256K ultra-long context. Combined with proprietary MTP-3 technology (predicting 3 tokens per step), inference speed reaches up to 350 TPS, while preserving complex mathematical reasoning, greatly reducing response latency for agent applications. See
https://static.stepfun.com/blog/step-3.5-flash/

- [Closed-source] xAI released Grok Imagine 1.0, officially entering video generation. The model produces high-quality video up to 10 seconds at 720p resolution, with its core highlight being advanced joint audio-video modeling for precise sound-image alignment and emotionally expressive audio synthesis, providing X platform creators with powerful AI tools. See
https://x.ai/news/grok-imagine-api

<br><br>
## Jan 26 ~ Feb 1
### Feb 1
- [Open-source] Alibaba Tongyi released Qwen3-Coder-Next, a programming agent model using an 80B-total-parameter MoE architecture (only 3B activated per inference). On SWE-Bench Verified, the problem-solving rate exceeds 70%, perfectly balancing high performance with low compute cost, demonstrating the "small activated parameters, strong engineering capability" advantage — well suited for compute-sensitive local development scenarios. See
https://qwen.ai/blog?id=qwen3-coder-next
### Jan 29
- [Closed-source] Alibaba Tongyi released XiaoMi (晓蜜) customer-service conversation analysis models, including tongyi-xiaomi-analysis-flash and tongyi-xiaomi-analysis-pro, focused on conversation information extraction, scenario classification, and satisfaction assessment. They excel at handling complex business-logic quality inspection rules, support custom analysis standards, and provide strong multi-turn dialogue understanding and semantic reasoning, delivering specialized solutions for enterprise customer service quality inspection and conversation analysis. See
https://help.aliyun.com/zh/model-studio/dialogue-analysis

### Jan 28
- [Open-source] Moonshot open-sourced Kimi K2.5, a native multimodal agent model, built on Kimi-K2-Base through continued pretraining on about 15 trillion mixed vision and text tokens. Officials say it is Kimi's most intelligent model to date, achieving open-source SOTA on Agent, code, image, video, and a series of general intelligence tasks; it is also Kimi's most versatile model to date. Key features include: native multimodality with excellent visual knowledge, cross-modal reasoning, and agentic tool use based on visual input; vision-driven coding that generates code based on visual specs and autonomously orchestrates tools to process visual data; agent swarms, evolving from single-agent to a self-directed, collaborative swarm execution architecture that decomposes complex tasks into multiple parallel subtasks executed cooperatively by dynamically instantiated domain-specific agents. See
https://www.modelscope.cn/models/moonshotai/Kimi-K2.5

- [Open-source] Following the open-source release of Qwen3-TTS, the Qwen team released the Qwen3-ASR series, including Qwen3-ASR-1.7B and Qwen3-ASR-0.6B, supporting language and speech recognition (ASR) for 52 languages and dialects. The Qwen3-ASR series supports streaming/offline inference in a single unified model and can handle long audio. The complete model architecture and weights are open-sourced, with a vLLM-based inference framework provided supporting batching, async serving, streaming inference, and timestamp prediction. See
https://www.modelscope.cn/models/Qwen/Qwen3-ASR-0.6B
https://www.modelscope.cn/models/Qwen/Qwen3-ASR-1.7B

- [Closed-source] Alibaba Tongyi released the qwen3-asr-flash-filetrans series, including qwen3-asr-flash-filetrans and qwen3-asr-flash-filetrans-2025-11-17, now supporting word-level timestamps. By setting the new enable_words parameter, you can obtain millisecond-level word/character alignment and benefit from finer, more semantically meaningful sentence segmentation, providing more precise temporal localization for speech recognition applications. See
https://help.aliyun.com/zh/model-studio/qwen-speech-recognition

### Jan 27
- [Closed-source] Alibaba Tongyi released qwen3-max-2026-01-23. Compared to the September 23, 2025 version, it effectively integrates thinking mode and non-thinking mode, significantly improving overall performance. In thinking mode, the model integrates three tools — Web search, web information extraction, and code interpreter — providing higher accuracy on complex problems by introducing external tools during the thinking process, offering powerful support for scenarios requiring deep reasoning and multi-tool coordination. See
https://help.aliyun.com/zh/model-studio/compatibility-with-openai-responses-api

- [Closed-source] Mistral released Mistral Vibe 2.0, a major upgrade to the terminal-native coding agent, powered by the most advanced Devstral 2 model family. Supports building custom subagents, pre-execution clarification confirmations, loading skills via slash commands, and configuring custom workflows to match working styles, empowering teams to build, maintain, and deliver code faster. See
https://mistral.ai/news/mistral-vibe-2-0

<br><br>
## Jan 19 ~ Jan 25
### Jan 23
- [Open-source] The Qwen team open-sourced the Qwen3-TTS series of high-performance multilingual text-to-speech models, supporting 10 languages (including Chinese, English, Japanese, Korean, etc.) and dialect voices, designed for global applications. Core features include: efficient speech representation based on the proprietary Qwen3-TTS-Tokenizer-12Hz that preserves paralinguistic information and achieves high-fidelity reconstruction; a discrete multi-codebook end-to-end architecture that removes the information bottleneck and cascade error of traditional LM+DiT setups; extremely low-latency streaming generation with end-to-end latency of just 97ms, meeting real-time interaction needs. See
https://modelscope.cn/collections/Qwen/Qwen3-TTS

### Jan 22
- [Open-source] FlashLabs' Chroma-4B advanced multimodal model is officially released, aimed at understanding and generating content across multiple modalities including text and audio. As a virtual human model, Chroma can process auditory input and respond simultaneously in both text and synthetic speech, enabling natural voice interaction. See
https://modelscope.cn/models/FlashLabs/Chroma-4B

- [Closed-source] At the ERNIE Moment event, Baidu announced that the native omni-modal large model ERNIE 5.0 has officially launched. With 2.4 trillion parameters, it uses native omni-modal unified modeling technology, supporting input and output across text, image, audio, and video. Individual users can experience it on the ERNIE app or wenxinyiyan.com; enterprises and developers can call it via the Baidu Qianfan platform. See
https://ernie.baidu.com/blog/posts/ernie-5.0-0110-release-on-lmarena/

### Jan 20
- [Open-source] Zhipu AI released GLM-4.7-Flash, a hybrid thinking model with 30B total parameters and just 3B activated. As a SOTA model at its tier, it offers a new option balancing performance and efficiency for lightweight deployment. On mainstream benchmarks such as SWE-bench Verified and τ²-Bench, its overall performance surpasses gpt-oss-20b and Qwen3-30B-A3B-Thinking-2507, achieving open-source SOTA among similar and comparable-size model series — delivering the best performance with minimal activated parameters. See
https://modelscope.cn/models/ZhipuAI/GLM-4.7-Flash

- [Open-source] LightOn released LightOnOCR-2-1B, an efficient end-to-end 1-billion-parameter vision-language model for converting documents (PDFs, scans, images) into clean, naturally ordered text without fragile pipelines. The second version is trained on a larger, higher-quality corpus, enhances coverage of French documents, arXiv papers, and scans, improves LaTeX handling, and achieves cleaner normalization. Supports versatile parsing of tables, receipts, forms, multi-column layouts, and mathematical symbols, with integrated image bounding box prediction. See
https://www.modelscope.cn/models/lightonai/LightOnOCR-2-1B

<br><br>
## Jan 12 ~ Jan 18
### Jan 17
- [Closed-source] Alibaba Tongyi released the wan2.6-i2v-flash image-to-video model, supporting both audio and silent video generation, with independent billing rules for each type. It also features multi-shot storytelling and audio processing capabilities, offering richer expressive forms and more flexible creation tools for video creation. See
https://help.aliyun.com/zh/model-studio/image-to-video-api-reference

- [Closed-source] Alibaba Qwen released the image editing model Max series, including qwen-image-edit-max and qwen-image-edit-max-2026-01-16, with more stable and richer editing capabilities, enhanced industrial design and geometric reasoning, and improved character consistency and editing precision, providing stronger technical support for professional image editing. See
https://help.aliyun.com/zh/model-studio/qwen-image-edit-guide

### Jan 16
- [Open-source] StepFun's native speech reasoning model Step-Audio-R1.1 took the top spot in the latest Artificial Analysis Speech Reasoning, surpassing Grok, Gemini, GPT-Realtime, and other leading first-tier models with 96.4% accuracy, setting a new historical best. It leads comparable speech models on the trade-off between performance and speed, balancing stronger real-time conversation and complex speech reasoning. See
https://modelscope.cn/models/stepfun-ai/Step-Audio-R1.1

- [Open-source] Black Forest Labs open-sourced the FLUX.2 [klein] model family, including 4B and 9B sizes — currently the fastest image generation model series. The series unifies generation and editing in a single compact architecture, achieving end-to-end inference below 0.5 seconds on modern hardware, and running on consumer GPUs with just 13GB VRAM. The 4B version runs on consumer GPUs with only 13GB VRAM, while the 9B version's performance rivals models 5x larger. Officially provided FP8 and NVFP4 quantized versions deliver up to 1.6x and 2.7x inference speedup on RTX GPUs respectively, with VRAM usage reduced by 40% and 55%. See
https://modelscope.cn/collections/black-forest-labs/FLUX-2-Klein

- [Open-source] Meituan's LongCat team officially released and open-sourced LongCat-Flash-Thinking-2601, an upgrade to the previously released LongCat-Flash-Thinking. The 2601 version reaches open-source SOTA on core benchmarks including Agentic Search, Agentic Tool Use, and TIR (Tool-Integrated Reasoning). It is the first fully open-source model to support an online free "deep rethinking mode", simultaneously running 8 brains at full speed to ensure thorough thinking and reliable decision-making. See
https://www.modelscope.cn/models/meituan-longcat/LongCat-Flash-Thinking-2601

- [Closed-source] Alibaba Qwen released qwen3-tts-vc-realtime-2026-01-15, the latest snapshot of the real-time speech synthesis model. Voice cloning has been further optimized, becoming more natural and closer to the original voice compared to qwen3-tts-vc-realtime-2025-11-27, providing higher-quality voice cloning for real-time speech synthesis applications. See
https://help.aliyun.com/zh/model-studio/qwen-tts-voice-cloning

### Jan 14
- [Open-source] Baichuan launched Baichuan-M3-235B, an open-source medical-enhanced LLM. Its core innovation is explicitly modeling the clinical decision process rather than simply generating surface-level answers. Via Fact-Aware RL technology, it achieves a lower hallucination rate than GPT-5.2 without relying on external tools. For deployment, W4 quantization reduces memory usage to 26% of the original, and combined with Gated Eagle3 speculative decoding, inference speed improves 96%, significantly lowering the barrier to deploying medical AI. See
https://modelscope.cn/models/baichuan-inc/Baichuan-M3-235B

### Jan 13
- [Open-source] Zhipu AI and Huawei jointly open-sourced the new-generation image generation model GLM-Image. Built end-to-end (data to training) on Ascend Atlas 800T A2 hardware with the MindSpore AI framework, it is the first SOTA multimodal model completely trained on domestic chips. The model uses an innovative "autoregressive + diffusion encoder" hybrid architecture, balancing global instruction understanding with local detail rendering, effectively solving generation challenges for knowledge-intensive scenarios such as posters and slides. For text rendering, it ranks #1 open-source on CVTG-2K and LongText-Bench, particularly excelling at Chinese character generation, with API costs of only ¥0.1 per image. See
https://modelscope.cn/models/ZhipuAI/GLM-Image

- [Open-source] Tsinghua University, Renmin University of China, ModelBest, and the OpenBMB open-source community jointly released AgentCPM-Explore, a 4B on-device agent model capable of handling 8 long, hard agent tasks such as GAIA and Xbench, supporting over 100 unrepeated and stable environment interactions. The full toolchain is also open-sourced, including the tool sandbox orchestration platform AgentDock, the async RL framework AgentRL, and the agent benchmark platform AgentToLeaP, supporting community-complete reproduction and custom extension. See
https://modelscope.cn/models/OpenBMB/AgentCPM-Explore

### Jan 12
- [Closed-source] Alibaba Qwen released qwen-image-plus-2026-01-09, a new snapshot of the image generation model. As a distilled accelerated version of qwen-image-max, it supports rapid generation of high-quality images, substantially improving inference speed while preserving generation quality, providing an efficient solution for high-frequency image generation scenarios. See
https://help.aliyun.com/zh/model-studio/qwen-image-api

<br><br>

## Jan 5 ~ Jan 11
### Jan 8
- [Open-source] The Qwen team launched the family's newest members Qwen3-VL-Embedding and Qwen3-VL-Reranker, built on the recently open-sourced Qwen3-VL, designed for multimodal information retrieval and cross-modal understanding. The series delivers strong multimodal generality within a unified framework, efficiently handling text, images, screenshots, and video input, reaching industry-leading performance on image-text retrieval, video-text matching, VQA, and multimodal clustering. The Embedding model generates rich cross-modal vector representations within a shared semantic space, supporting efficient similarity computation; the Reranker accurately scores relevance for mixed-modal input pairs. Together they form a two-stage retrieval pipeline that significantly improves precision. The models inherit Qwen3-VL's 30+ language support and offer flexible vector dimensions, customizable instructions, and quantization-optimized performance — easy to integrate into globalized applications. See
https://modelscope.cn/collections/Qwen/Qwen3-VL-Embedding-and-Rerank

### Jan 7
- [Open-source] Tencent's Youtu team open-sourced Youtu-LLM-2B, a small LLM with only 1.96B parameters yet powerful, supporting 128k long context and with native agentic capabilities. See
https://modelscope.cn/models/Tencent-YouTu-Research/Youtu-LLM-2B

### Jan 6
- [Closed-source] Alibaba Qwen released the speech recognition models qwen3-asr-flash and qwen3-asr-flash-2025-09-08, supporting OpenAI-compatible mode, providing developers with a standardized speech file recognition interface to simplify integration and accelerate development of speech-to-text applications. See
https://help.aliyun.com/zh/model-studio/qwen-speech-recognition

### Jan 5
- [Closed-source] Alibaba Tongyi released the CosyVoice speech synthesis model cosyvoice-v3-flash, adding 24 voices covering diverse scenarios. New voices include: dialects (Longjiayi, Longlaotie); overseas marketing; poetry recitation (Longfei); voice assistants (Longxiaochun, Longxiaoxia, YUMI); social companionship (Longcheng, Longze, Longzhe, Longyan, Longxing, Longtian, Longwan, Longyan, Longfeifei, Longhao); audiobooks (Longsanshu, Longyuan, Longyue, Longxiu, Longnan); and news broadcasting (Longshu) — offering rich voice options for various applications. See
https://help.aliyun.com/zh/model-studio/cosyvoice-voice-list

<br><br>

## Dec 29 ~ Jan 4
### Dec 31
- [Closed-source] The Qwen team launched qwen-image-max-2025-12-30, the Qwen image generation Max series, which compared to the Plus series enhances image realism and naturalness, effectively reducing AI-synthesized artifacts and standing out in human textures, fine details, and text rendering. See
https://help.aliyun.com/zh/model-studio/qwen-image-api

### Dec 30
- [Open-source] Tencent Hunyuan officially open-sourced translation model version 1.5, containing two models: Tencent-HY-MT1.5-1.8B and Tencent-HY-MT1.5-7B, supporting mutual translation across 33 languages and 5 ethnic-Mandarin/dialect pairs. Beyond common languages such as Chinese, English, and Japanese, it includes minor languages such as Czech, Marathi, Estonian, and Icelandic. See
https://www.modelscope.cn/collections/Tencent-Hunyuan/HY-MT15

<br><br>

## Dec 22 ~ Dec 28
### Dec 24
- [Open-source] The Qwen team released Qwen-Image-Edit-2511. Compared to the previous Qwen-Image-Edit-2509, it achieves multiple enhancements in character consistency, LoRA capability integration (supporting relighting, multi-scene), industrial design, and geometric reasoning, providing a stronger technical foundation for image editing applications. See
https://modelscope.cn/models/Qwen/Qwen-Image-Edit-2511

- [Open-source] StepFun open-sourced the NextStep-1.1 image generation model. This version effectively solves the visualization failures in NextStep-1 and substantially improves image quality through extended training and Flow-based reinforcement learning (RL) post-training paradigms. See
https://huggingface.co/stepfun-ai/NextStep-1.1

### Dec 23
- [Closed-source] Qwen released qwen-image-edit-plus-2025-12-15, the latest snapshot of the image editing model. Compared to the previous version, it shows significant improvements in character consistency, industrial design capability, and geometric reasoning. Optimized alignment between edited image and original in spatial layout, texture, and style produces more precise and refined editing, providing more powerful tools for professional image processing. See
https://help.aliyun.com/zh/model-studio/qwen-image-edit-guide

- [Open-source] MiniMax officially open-sourced the M2 upgrade MiniMax-M2.1, focused on improving real-world complex task utility, with key optimizations in multi-language programming and office scenarios. Core highlights include: outstanding multilingual programming; enhanced Web and native App development with improved Android/iOS development and design aesthetics; upgraded compound instruction understanding, the first open-source series to introduce interleaved thinking; a more concise and efficient interaction experience with more refined replies and chains of thought and lower token consumption; and powerful Agent and tool generalization. See
https://www.modelscope.cn/models/MiniMax/MiniMax-M2.1

- [Open-source] Zhipu AI released and open-sourced GLM-4.7, focused on enhancing coding capabilities, long-horizon task planning, and tool coordination for coding scenarios, achieving leading open-source results on multiple mainstream public benchmarks. Breakthroughs in three dimensions of coding, reasoning, and agents: stronger coding capability with significant improvements in multi-language coding and terminal agent effectiveness, supporting the "think first, then act" mechanism for frameworks such as Claude Code, TRAE, Kilo Code, Cline, and Roo Code. See
https://modelscope.cn/models/ZhipuAI/GLM-4.7

<br><br>
## Dec 15 ~ Dec 21
### Dec 20
- [Open-source] The Qwen team released the latest research Qwen-Image-Layered, a model that can decompose images into multiple RGBA layers. This layered representation releases the inherent editability of images: each layer can be manipulated independently without affecting others. The layered representation also naturally supports high-fidelity basic operations — such as resizing, repositioning, and color recoloring. By physically isolating semantic or structural components into independent layers, this approach achieves high-fidelity and consistent editing effects, bringing a revolutionary breakthrough to image editing. See
https://www.modelscope.cn/models/Qwen/Qwen-Image-Layered

### Dec 18
- [Closed-source] Mistral released Mistral OCR 3, a document parsing model designed for extracting text and embedded images from various documents. Supports Markdown output and HTML-based table reconstruction, allowing downstream systems to understand not just document content but also structure. As a smaller model than most competitive offerings, it serves at industry-leading pricing of $2 per 1000 pages, with a 50% discount via Batch-API bringing costs down to $1 per 1000 pages — a highly cost-effective solution for enterprise document processing. See
https://mistral.ai/news/mistral-ocr-3

### Dec 17
- [Closed-source] Google launched the Gemini 3 Flash preview gemini-3-flash-preview, offering rapid frontier-level performance comparable to large models at far lower cost. Major upgrades to visual and spatial reasoning, plus agentic coding, providing developers with cost-effective AI solutions. See
https://ai.google.dev/gemini-api/docs/code-execution?hl=zh-cn#images

- [Closed-source] OpenAI released GPT-Image-1.5, the latest image generation model, designed for production-grade visuals and highly controllable creative workflows. Major improvements in realism, accuracy, and editability, supporting flexible quality-latency trade-offs for professional design tasks and iterative content creation. Core capabilities include: high-fidelity photorealism (natural lighting, accurate materials, rich color rendering), robust face and identity preservation, reliable text rendering (clear letters, consistent layout, strong contrast), complex structured visuals (infographics, charts, multi-panel compositions), precise style control and style transfer, and strong real-world knowledge and reasoning. See
https://platform.openai.com/docs/models/gpt-image-1.5

- [Open-source] Xiaomi released MiMo-V2-Flash, a Mixture-of-Experts (MoE) language model with 309B total and 15B activated parameters. Designed for high-speed inference and agentic workflows, it adopts a novel hybrid attention architecture and multi-token prediction (MTP), achieving state-of-the-art performance while significantly reducing inference costs — an efficient solution for large-scale model deployment. See
https://modelscope.cn/models/XiaomiMiMo/MiMo-V2-Flash

- [Closed-source] Tencent launched Tencent HY Vision 1.5 Instruct, an image-to-text fast-thinking model produced on the text TurboS base, with significant effectiveness improvements over the previous version across image basic recognition, image analysis, and reasoning. See
https://cloud.tencent.com/document/product/1729/104753
### Dec 16
- [Open-source] Tongyi Lab launched Fun-ASR, an end-to-end speech recognition model trained on tens of millions of hours of real speech data, with strong context understanding and industry adaptability. Supports low-latency real-time transcription, covering 31 languages, and excels in vertical domains such as Education and Finance, accurately recognizing professional terminology and industry expressions, effectively addressing "hallucination" generation and language confusion. Also open-sourced is the lightweight Fun-ASR-Nano with total parameters compressed to 0.8B, significantly reducing inference costs. See
https://modelscope.cn/models/FunAudioLLM/fun-asr-nano-2512

- [Closed-source] Qwen released qwen3-tts-vd-realtime-2025-12-16, a real-time speech synthesis snapshot model that can use voices generated by voice design for low-latency, high-stability real-time synthesis, supporting multilingual output, automatically adjusting tone based on text, and optimized performance for complex text. See
https://help.aliyun.com/zh/model-studio/qwen-tts-realtime

- [Closed-source] Qwen released qwen-voice-design, a voice design model that generates customized voices via text description. Combined with the qwen3-tts-vd-realtime-2025-12-16 model to generate speech, covering 10 languages, providing users with personalized speech synthesis solutions. See
https://help.aliyun.com/zh/model-studio/qwen-tts-voice-design

### Dec 15
- [Closed-source] ByteDance released Doubao doubao-seed-1-8-251215, achieving three breakthroughs in Agent capability, multimodal understanding, and context management. Tool Use, complex instruction following, and OS Agent capabilities are substantially enhanced; basic visual understanding is significantly improved, supporting low-frame-rate understanding of ultra-long video, with comprehensive upgrades in video motion understanding, complex spatial understanding, and document structure parsing. Native intelligent context management supports configurable context compression strategies, automatically clearing low-value historical information when task rounds grow too long to ensure stable completion of multi-step tasks. See
https://console.volcengine.com/ark/region:ark+cn-beijing/model/detail?Id=doubao-seed-1-8

- [Open-source] Tongyi Lab released Fun-CosyVoice 3.0, an advanced LLM-based TTS system that surpasses the previous CosyVoice 2.0 in content consistency, speaker similarity, and prosody naturalness. Also open-sourced Fun-CosyVoice3-0.5B, supporting zero-shot multilingual speech synthesis covering 9 common languages (Chinese, English, Japanese, Korean, German, Spanish, French, Italian, Russian) and 18+ Chinese dialects/accents, with pronunciation correction supporting Chinese Pinyin and English CMU phonemes, bidirectional stream processing, latency as low as 150ms, and instruction control over language, dialect, emotion, speed, and volume. See
https://modelscope.cn/models/FunAudioLLM/Fun-CosyVoice3-0.5B-2512

<br><br>
## Dec 8 ~ Dec 14
### Dec 12
- [Closed-source] Google launched a new native audio model gemini-2.5-flash-native-audio-preview-12-2025 for the Live API, substantially improving the model's ability to handle complex audio workflows and delivering stronger performance for real-time voice interaction applications. See
https://ai.google.dev/gemini-api/docs/models?hl=zh-cn#gemini-2.5-flash-live

### Dec 11
- [Closed-source] OpenAI released three upgrades to the GPT-5.2 series, including GPT-5.2 Instant, GPT-5.2 Thinking, and GPT-5.2 Pro. The entire series' knowledge cutoff is updated to August 2025. The Instant version delivers significant improvements in information retrieval, technical writing, and translation while preserving its warm conversational style; the Thinking version performs better on complex tasks such as spreadsheet modeling, code programming, and long-document summarization; the Pro version reduces major errors in complex domains like programming, providing the most reliable answers. See
https://openai.com/index/introducing-gpt-5-2/

- [Closed-source] Google released the Interactions API Beta, providing a unified interface for interacting with Gemini models and agents, simplifying developer integration and supporting more flexible application building. See
https://ai.google.dev/gemini-api/docs/interactions?hl=zh-cn

- [Closed-source] Google launched the Gemini Deep Research agent preview, capable of autonomously planning, executing, and integrating multi-step research task results, providing powerful support for scenarios requiring deep information collection and analysis. See
https://ai.google.dev/gemini-api/docs/deep-research?hl=zh-cn

### Dec 10
- [Closed-source] Google launched enhanced Gemini 2.5 text-to-speech models, including Gemini 2.5 Flash TTS preview (low-latency optimized) and Gemini 2.5 Pro TTS preview (quality optimized). The new versions deliver significant improvements in expressiveness, speed precision, and dialogue fluency, providing a more natural experience for real-time voice interaction. See
https://ai.google.dev/gemini-api/docs/speech-generation?hl=zh-cn

### Dec 9
- [Open-source] Mistral released Devstral 2 and Devstral Small 2, agent models designed for software engineering tasks. They excel on the SWE-bench benchmark, skilled at using tools to explore codebases, edit multiple files, and drive software engineering agents. Supports 256k ultra-long context windows, uses FP8 precision instruction fine-tuning, and comprehensively surpasses predecessors in agentic coding, performance, and generalization. See
https://huggingface.co/collections/mistralai/devstral-2

- [Open-source] Zhipu AI released the Open-AutoGLM mobile assistant framework, composed of the Phone Agent framework and AutoGLM-Phone-9B model. The system controls devices via ADB, perceives the screen with a vision-language model, and combines intelligent planning to automatically execute operation flows. Users only need to describe their needs in natural language, and the system automatically parses intent, understands the interface, plans actions, and completes tasks. Provides Chinese and English bilingual models — AutoGLM-Phone-9B optimized for Chinese applications, and a Multilingual version supporting multilingual scenarios. See
https://github.com/zai-org/Open-AutoGLM

### Dec 8
- [Open-source] Zhipu AI released the GLM-4.6V series of multimodal models, including GLM-4.6V (106B) cloud version and GLM-4.6V-Flash (9B) lightweight version. The models support 128k ultra-long context and achieve SOTA visual understanding performance at their parameter scale. The biggest highlight is the first integration of Function Call capability natively into a vision model architecture, opening the complete chain from "visual perception" to "executable action", providing a unified technical foundation for multimodal Agent applications. See
https://www.modelscope.cn/collections/GLM-46V-37fabc27818446
<br><br>
## Dec 1 ~ Dec 7
### Dec 5
- [Closed-source] Tencent Hunyuan released the latest language models Tencent HY 2.0 Think and Tencent HY 2.0 Instruct. HY 2.0 uses a Mixture-of-Experts (MoE) architecture with 406B total and 32B activated parameters, supports a 256K context window, with reasoning capability and efficiency ranking among China's top tier, and standout performance in practical scenarios such as text creation and complex instruction following. See
https://cloud.tencent.com/document/product/1729/104753

### Dec 4
- [Closed-source] Alibaba released qwen3-omni-flash-2025-12-01 and qwen-plus-2025-12-01. The former is the latest Qwen Omni snapshot, supporting up to 49 voices, with substantially upgraded instruction-following and efficient understanding across text, image, audio, and video. The latter is the latest version of the Qwen3 Plus series. See
https://help.aliyun.com/zh/model-studio/qwen-omni

- [Closed-source] Alibaba released qwen3-omni-flash-realtime-2025-12-01, the latest Qwen Omni real-time snapshot model, providing low-latency multimodal interaction with up to 49 voices and substantially upgraded instruction-following and interaction experience. See
https://help.aliyun.com/zh/model-studio/realtime

- [Closed-source] Alibaba released qwen3-livetranslate-flash and qwen3-livetranslate-flash-2025-12-01. Qwen3-LiveTranslate-Flash is an audio-video translation model supporting mutual translation across 18 languages (including Chinese, English, Russian, French, etc.), combining visual context to improve translation accuracy, outputting both text and speech. See
https://help.aliyun.com/zh/model-studio/qwen3-livetranslate-flash

### Dec 2
- [Open-source] Mistral AI released the new-generation Mistral 3 series, all under Apache 2.0. The flagship Mistral Large 3 uses an MoE architecture (41B activated / 675B total parameters), ranking second among open-source non-reasoning models, with image understanding and multilingual support; concurrently launched is the Ministral 3 series (3B/8B/14B) for edge scenarios, with base, instruct, and reasoning variants at each size — the 14B reasoning version achieves 85% accuracy on AIME '25. All models support multimodality and 40+ languages, now available on Hugging Face, Amazon Bedrock, Azure, and more. See
https://mistral.ai/news/mistral-3

- [Open-source] DeepSeek released two official models: DeepSeek-V3.2 and DeepSeek-V3.2-Speciale, balancing high computational efficiency with excellent reasoning and agentic performance. DeepSeek-V3.2 balances reasoning capability with output length, suitable for daily use, reaching GPT-5 levels on public reasoning benchmarks and only slightly below Gemini-3.0-Pro. DeepSeek-V3.2-Speciale is a long-thinking-enhanced version of V3.2, combined with DeepSeek-Math-V2's theorem-proving capability, featuring excellent instruction following and rigorous mathematical proof and logical verification, with performance rivaling Gemini-3.0-Pro. See
https://modelscope.cn/collections/DeepSeek-V32-29d54eab6f3a4d

### Dec 1
- [Open-source] StepFun open-sourced GELab-Zero, the first time a GUI Agent model and complete supporting infrastructure are released simultaneously, supporting one-click deployment. The 4B GUI Agent model comprehensively sets new performance records for same-size models on mobile, PC, and other GUI leaderboards, achieving SOTA. StepFun also open-sourced its self-built evaluation standard AndroidDaily based on real business scenarios, to promote GUI domain model evaluation toward consumer-grade, large-scale applications. See
https://modelscope.cn/models/stepfun-ai/GELab-Zero-4B-preview

- [Open-source] Meituan open-sourced the LongCat-Image series, containing a base generation model, an edit model, and a development intermediate model, providing developers with efficient bilingual image generation and editing. The core LongCat-Image base model uses only 6B parameters yet leads on multiple benchmarks, with key advantages in outstanding Chinese text rendering and excellent image realism. LongCat-Image-Edit supports precise image modifications based on Chinese/English instructions, achieving open-source SOTA performance while strictly preserving visual consistency in non-edited regions. The series includes production-ready full-stack training code, covering the complete flow from data preparation through fine-tuning to alignment, significantly lowering research and deployment barriers. See
https://modelscope.cn/collections/LongCat-Image-17ef53fc3b4042

<br><br>
## Nov 24 ~ Nov 30
### Nov 26
- [Open-source] Alibaba Tongyi Lab launched a 6B-parameter image generation series with three variants. The Turbo version is open-sourced, focused on extreme inference (8 NFEs, sub-second latency), runnable on consumer 16G VRAM, excelling at photorealistic imagery, Chinese-English bilingual rendering, and instruction following; the Base and Edit (image-to-image editing) versions will be open-sourced soon for community secondary development. See
https://www.modelscope.cn/models/Tongyi-MAI/Z-Image-Turbo
<br><br>


## Nov 17 ~ Nov 23
### Nov 22
- [Open-source] Xiaomi released MiMo-Embodied-7B, the first open-source cross-embodiment vision-language model integrating embodied AI and autonomous driving, significantly enhancing understanding and reasoning over dynamic physical environments. Across 37 benchmarks in embodied AI (task planning, affordance prediction, spatial understanding), autonomous driving (environment perception, state prediction, driving planning), and general visual understanding, it comprehensively surpasses existing open-source models and rivals or exceeds closed-source and proprietary models, demonstrating the enhancing effect of specialized training on general capability. See
https://www.modelscope.cn/models/XiaomiMiMo/MiMo-Embodied-7B

### Nov 21
- [Open-source] Tencent Hunyuan released HunyuanVideo 1.5, a lightweight yet powerful open-source video generation model. With only 8.3B parameters, it achieves leading visual quality and motion coherence in video generation, effectively lowering the barrier to video creation. The model aims to deliver video generation rivaling or surpassing top closed-source models, and supports running on consumer GPUs. See
https://github.com/Tencent-Hunyuan/HunyuanVideo-1.5

### Nov 20
- [Closed-source] Google released the Gemini 3 Pro Image preview gemini-3-pro-image-preview, the next generation of the Nano Banana model — Nano Banana Pro. See
https://ai.google.dev/gemini-api/docs/image-generation?hl=zh-cn

### Nov 19
- [Closed-source] xAI released Grok 4.1 Fast, now available via the Enterprise API. Grok 4.1 Fast now supports agentic tools, with agentic tool pricing slashed up to 50% to under $5 per 1000 successful calls. See
https://x.ai/news/grok-4-1-fast

- [Closed-source] OpenAI released GPT-5.1-Codex-Max, a frontier agentic coding model built for long-running project-level work. Faster, more powerful, and more token-efficient than GPT-5.1-Codex, using compression to work coherently across multiple context windows. Now available across Codex products including the CLI, IDE extensions, cloud, and code review, at the same price as GPT-5.1-Codex. See
https://openai.com/index/gpt-5-1-codex-max/

- [Open-source] Meta AI released Segment Anything Model 3 (SAM 3), the latest unified computer vision model aiming to enable precise detection, segmentation, and tracking of objects in images and video via text, example images, and visual prompts. Building on the prior SAM models, it enhances understanding and handling of conceptual prompts (such as noun phrases) and visual prompts (such as masks, bounding boxes, points). See
https://ai.meta.com/sam3/

- [Open-source] Meta AI released SAM 3D, an advanced 3D reconstruction model suite aimed at turning 2D images into precise 3D reconstructions. Includes two main submodels: SAM 3D Objects for 3D reconstruction of objects and scenes, and SAM 3D Body focused on human pose and shape estimation. SAM 3D extends the concept of "promptable" vision to capture and restore rich 3D information from single images, including geometry, texture, and layout, plus human mesh models. See
https://ai.meta.com/sam3d/

### Nov 18
- [Closed-source] Google launched the first Gemini 3 series model gemini-3-pro-preview, the most advanced reasoning and multimodal understanding model with powerful agentic and coding capabilities. Beyond improvements in intelligence and performance, the Gemini 3 Pro preview also introduces new behaviors such as media resolution, thought signatures, and thinking levels. See
https://ai.google.dev/gemini-api/docs/gemini-3?hl=zh-cn

### Nov 17
- [Closed-source | Speech Recognition] Alibaba released qwen3-asr-flash-filetrans and qwen3-asr-flash-filetrans-2025-11-17 (snapshot), Qwen's new recording file recognition model, designed for async transcription of audio files supporting up to 12-hour recordings. See
https://help.aliyun.com/zh/model-studio/qwen-speech-recognition
<br><br>

## Nov 10 ~ Nov 16
### Nov 13
- [Closed-source] Baidu released ERNIE-5.0-Preview (ERNIE 5.0 preview), using native omni-modal unified modeling to jointly model text, image, audio, and video with comprehensive omni-modal capabilities. Foundational capabilities are comprehensively upgraded, with particularly strong performance in multimodal understanding, instruction following, creative writing, factuality, agent planning, and tool use. See
https://console.bce.baidu.com/qianfan/modelcenter/model/buildIn/detail/am-3c0d4ca1f067

### Nov 12
- [Closed-source] OpenAI upgraded GPT-5 to GPT-5.1, releasing Instant and Thinking versions for smarter, more conversational answers. GPT-5.1 Instant uses lightweight adaptive reasoning, staying fast when facing hard problems; GPT-5.1 Thinking more precisely adjusts thinking time for complex tasks, with clearer responses and less jargon. See
https://openai.com/index/gpt-5-1/

### Nov 11
- [Closed-source] ByteDance released doubao-seed-code, an AI Coding model built for real development scenarios, with enhanced Bugfix and frontend capabilities. Supports input-transparent caching to effectively reduce usage costs. See
https://www.volcengine.com/docs/82379/1949118

- [Open-source] Baidu released ERNIE-4.5-VL-28B-A3B-Thinking, a deep-thinking model trained on top of ERNIE-4.5-VL-28B-A3B. As a lightweight model with only 3B activated, it closely follows industry-leading flagship models on various tests, achieving near-SOTA visual performance at a lightweight scale. See
https://modelscope.cn/models/PaddlePaddle/ERNIE-4.5-VL-28B-A3B-Thinking
<br><br>


## Nov 3 ~ Nov 9
### Nov 7
- [Open-source] Moonshot released Kimi-K2-Thinking, the latest and most powerful open-source thinking model. Built as a thinking agent capable of step-by-step reasoning while dynamically calling tools, it sets new state-of-the-art on benchmarks such as Humanity's Last Exam (HLE) and BrowseComp. See
https://modelscope.cn/models/moonshotai/Kimi-K2-Thinking

### Nov 3
- [Open-source] Meituan released LongCat-Flash-Omni-FP8, an open-source omni-modal model with 56B parameters (27B activated), excelling at real-time audio-video interaction. The model uses a high-performance shortcut-connected Mixture-of-Experts (MoE) architecture with zero-compute experts, combined with efficient multimodal perception and speech reconstruction modules. A curriculum-inspired progressive training strategy enables comprehensive multimodal capabilities while preserving strong unimodal capabilities. See
https://modelscope.cn/models/meituan-longcat/LongCat-Flash-Omni-FP8
<br><br>


## Oct 27 ~ Nov 2
### Oct 31
- [Closed-source] Alibaba released qwen-image-edit-plus-2025-10-30, which builds on qwen-image-edit to optimize inference performance and system stability, substantially reducing image generation and editing response times and supporting returning multiple images per request. See
https://help.aliyun.com/zh/model-studio/qwen-image-edit-guide

### Oct 27
- [Open-source] MiniMax released MiniMax-M2, a lightweight, fast, and highly cost-effective MoE model (230B total, 10B activated), built for Max-level coding and agents. With just 10B activated parameters, it delivers end-to-end tool-use performance, excelling on coding and agentic tool use benchmarks, and is easier to deploy and scale. See
https://modelscope.cn/models/MiniMax/MiniMax-M2
<br><br>


## Oct 20 ~ Oct 26
### Oct 26
- [Open-source] Meituan's LongCat team released the LongCat-Video video generation model based on the Diffusion Transformer architecture, innovatively distinguishing tasks via "number of condition frames" to natively support text-to-video, image-to-video, and video continuation — the three core tasks — enabling coherent minute-level long video generation that ensures cross-frame temporal consistency and physically plausible motion at the root. See
https://modelscope.cn/models/meituan-longcat/LongCat-Video
- [Open-source] Tsinghua CoAI Lab & Zhipu AI released the Glyph framework, which extends context length via visual-text compression — rendering the 240K-token "Jane Eyre" as images using about 80K visual tokens, achieving a 3x compression ratio. On MMLongBench-Doc, overall accuracy improved by 13% over the baseline VLM, with excellent results in real multimodal scenarios such as PDF document understanding. See
https://modelscope.cn/models/ZhipuAI/Glyph

### Oct 22
- [Open-source] Tencent Hunyuan released world model version 1.1 HunyuanWorld-Mirror, adding support for multi-view and video input, deployable on a single GPU, creating 3D worlds in seconds, simultaneously generating point clouds, multi-view depth, camera parameters, surface normals, 3D Gaussians, and other 3D representations in a single forward pass. See
https://modelscope.cn/models/Tencent-Hunyuan/HunyuanWorld-Mirror

### Oct 21
- [Closed-source] Alibaba released qwen3-vl-32b-thinking and qwen3-vl-32b-instruct, the 32B Dense models in the Qwen3-VL series. They excel in document recognition and understanding, spatial perception and general recognition, visual 2D detection and spatial reasoning, suitable for complex perception tasks in general scenarios. See
https://help.aliyun.com/zh/model-studio/vision
- [Open-source] DeepSeek released DeepSeek-OCR, proposing the new paradigm of "context optical compression" that renders long text as images compressed by a vision encoder into very few visual tokens. At ≤10x compression ratio, OCR accuracy reaches 97%; with just 100 tokens it surpasses GOT-OCR2.0, supports nearly 100 languages and chart parsing, with a single A100 processing 200K pages per day. See
https://modelscope.cn/models/deepseek-ai/DeepSeek-OCR
- [Open-source] iFlytek released Spark-Scilit-X1-13B, a large-scale language model tailored for academic research, excelling at paper-assisted reading, academic translation, English polishing, and review generation, combining a unified framework of long chain-of-thought reasoning and dual-process theory, supporting both fast and slow thinking modes. See
https://modelscope.cn/models/iflytek/Spark-Scilit-X1-13B
<br><br>


## Oct 13 ~ Oct 19
### Oct 16
- [Open-source] Baidu released PaddleOCR-VL-0.9B, a multimodal document parsing model that with only 0.9B parameters sets new records on multiple authoritative benchmarks. It supports 109 languages and precisely recognizes complex elements in images including text, handwritten Chinese characters, tables, formulas, and charts, processing 1881 tokens per second — 14.2% faster inference than MinerU. See https://www.modelscope.cn/models/PaddlePaddle/PaddleOCR-VL

### Oct 15
- [Closed-source] ByteDance Doubao released doubao-seed-1-6-lite-251015, supporting deep thinking (manually toggleable, adjustable thinking length), with text generation, image understanding, video understanding, and tool calling capabilities. See https://www.volcengine.com/docs/82379/1874969
- [Closed-source] Alibaba released qwen3-vl-flash-2025-10-15, a small-size visual understanding model in the Qwen3 series, effectively integrating thinking and non-thinking modes for better effects and faster response. See https://help.aliyun.com/zh/model-studio/vision
- [Closed-source] Google released Veo 3.1 and 3.1 Fast public previews, supporting extending videos, generating video from up to three reference images, first/last frame control, and adding 4-second, 6-second, and 8-second duration options. See https://ai.google.dev/gemini-api/docs/video#veo-3.1
- [Closed-source] Anthropic released Claude Haiku 4.5, the fastest and most intelligent Haiku model with near-frontier performance, suitable for real-time applications, high-volume processing, and cost-sensitive deployments. See https://docs.claude.com/en/docs/about-claude/models

### Oct 14
- [Closed-source] Tencent Hunyuan released the hunyuan-translation model, supporting mutual translation across 33 languages and 5 ethnic languages, with best-in-class effects among models of the same size — winning first place in 30 languages in the WMT25 competition and leading on the open-source Flores200 test set. See https://cloud.tencent.com/document/product/1729/104753

### Oct 13
- [Open-source] Alibaba open-sourced qwen3-vl-8b-thinking and qwen3-vl-8b-instruct, the 8B Dense models in the Qwen3-VL series. They use less VRAM, can perform multimodal understanding and reasoning, support ultra-long context such as long videos and documents, visual 2D/3D localization, and comprehensive spatial perception and general recognition. See https://modelscope.cn/collections/Qwen3-VL-5c7a94c8cb144b
<br><br>


## Oct 6 ~ Oct 12
### Oct 10
- [Closed-source] StepFun's step-tts-mini added three premium voices: graceful and gentle, lively and quick, and Energetic-Confident (English voice). See https://platform.stepfun.com/docs/guide/tts#step-tts-mini

### Oct 7
- [Closed-source] After OpenAI released Sora2, soon afterward the video generation model Sora 2 and Sora 2 Pro APIs officially launched. See https://platform.openai.com/docs/guides/video-generation
- [Closed-source] Google released the Gemini 2.5 Computer Use preview, supporting computer control via the API. See https://ai.google.dev/gemini-api/docs/computer-use

### Oct 6
- [Closed-source] OpenAI officially launched the GPT-5 pro model API. GPT-5 pro is available only via the Responses API, with a maximum output of 272,000 tokens and a 400,000-token context limit. Knowledge cutoff is September 30, 2024. See https://platform.openai.com/docs/models/gpt-5-pro
<br><br>


## Sep 29 ~ Oct 5
### Oct 4
- [Open-source] The Bailing model team released Ling-1T, a flagship non-thinking model with 1 trillion total parameters and about 50B activated per token, supporting 128K context length, achieving SOTA on multiple complex reasoning benchmarks. See https://modelscope.cn/models/inclusionAI/Ling-1T

### Oct 2
- [Closed-source] Google officially released the Gemini 2.5 Flash image generation model. See https://ai.google.dev/gemini-api/docs/image-generation

### Sep 30
- [Open-source] Zhipu released GLM-4.6, the strongest code model in the GLM series, with code capabilities improved 27% over GLM-4.5, comprehensive improvements in real-world programming, long-context handling, and reasoning. See https://www.modelscope.cn/models/ZhipuAI/GLM-4.6

### Sep 29
- [Closed-source] Anthropic released Claude Sonnet 4.5, performing best on complex agentic and coding tasks, with the highest intelligence on most tasks. See https://docs.claude.com/en/docs/about-claude/models/whats-new-sonnet-4.5
- [Open-source] DeepSeek released the experimental DeepSeek-V3.2-Exp, introducing DeepSeek Sparse Attention to significantly improve long-context processing efficiency. See https://modelscope.cn/models/deepseek-ai/DeepSeek-V3.2-Exp
<br><br>


## Sep 22 ~ Sep 28
### Sep 28
- [Open-source] Tencent Hunyuan released HunyuanImage 3.0, the first industrial-grade natively multimodal image generation model, with 80B parameters — currently the best-performing and largest open-source image generation model. See https://modelscope.cn/models/Tencent-Hunyuan/HunyuanImage-3.0

### Sep 26
- [Closed-source] Tencent Hunyuan released hunyuan-turbos-20250926, with science/engineering scores improved 10.9% on average (math up 13.8%, logical reasoning up 12.3%), and humanities areas such as writing, knowledge Q&A, and Agent improved by about 2%. See https://cloud.tencent.com/document/product/1729/104753

### Sep 25
- [Closed-source] Google released Gemini Robotics-ER 1.5 preview, designed for robotics applications. See https://ai.google.dev/gemini-api/docs/robotics-overview
- [Closed-source] Google released gemini-2.5-flash-preview-09-2025 and gemini-2.5-flash-lite-preview-09-2025 preview models. See https://ai.google.dev/gemini-api/docs/models

### Sep 23
- [Closed-source | Speech Recognition] Alibaba released the speech recognition model fun-asr-realtime, integrating innovative RAG technology, supporting large-scale hotword customization, ITN normalization, punctuation prediction, etc., significantly improving recognition accuracy and contextual fit, supporting free Chinese-English switching with stronger noise robustness. See https://help.aliyun.com/zh/model-studio/real-time-speech-recognition
- [Closed-source | Multimodal Embedding] Alibaba released the multimodal embedding models tongyi-embedding-vision-plus and tongyi-embedding-vision-flash, built on the Qwen series LLMs, enhancing visual vectorization with support for text, image, and video modalities. See https://help.aliyun.com/zh/model-studio/embedding
- [Closed-source | Code] Alibaba released the code model qwen3-coder-plus-2025-09-23, built on Qwen3, with improvements in downstream task effectiveness, tool-calling robustness, and code safety over the previous version. See https://help.aliyun.com/zh/model-studio/qwen-coder
- [Closed-source | Text-to-image] Alibaba released the text-to-image model qwen-image-plus, with outstanding complex text rendering supporting Chinese/English and complex mixed text-image layouts at better pricing than qwen-image. See https://help.aliyun.com/zh/model-studio/qwen-image-api
- [Closed-source | Text Generation] Alibaba released the text generation models qwen3-max and qwen3-max-2025-09-23. Compared with the preview version, they feature dedicated upgrades in agentic coding and tool calling directions, reaching SOTA in the field. See https://help.aliyun.com/zh/model-studio/models
- [Closed-source | Visual Reasoning] Alibaba released the visual reasoning models qwen3-vl-plus and qwen3-vl-plus-2025-09-23, integrating thinking / non-thinking modes, with world-class visual agent capabilities and comprehensive upgrades in visual coding, spatial perception, and multimodal thinking. See https://help.aliyun.com/zh/model-studio/vision
- [Closed-source | Text-to-image] Alibaba released the text-to-image model wan2.5-t2i-preview, removing single-side limits and allowing free choice of dimensions within total pixel area and aspect ratio constraints. See https://help.aliyun.com/zh/model-studio/text-to-image-v2-api-reference
- [Closed-source | Image Editing] Alibaba released the image editing model wan2.5-i2i-preview, supporting text, single-image, or multi-image input, enabling consistent subject editing, multi-image fusion, and image group generation. See https://help.aliyun.com/zh/model-studio/wan2-5-image-edit-api-reference
- [Closed-source | Text-to-video] Alibaba released the text-to-video model wan2.5-t2v-preview, adding audio capabilities, supporting auto-dubbing or custom audio files for audio-visual synchronization. See https://help.aliyun.com/zh/model-studio/text-to-video-api-reference
- [Closed-source | Image-to-video] Alibaba released the image-to-video model wan2.5-i2v-preview, adding audio capabilities supporting auto-dubbing or custom audio files for audio-visual synchronization. See https://help.aliyun.com/zh/model-studio/image-to-video-api-reference
- [Closed-source] Google released gemini-2.5-flash-native-audio-preview-09-2025, the Live API native audio model with improved function calling and voice interruption handling. See https://ai.google.dev/gemini-api/docs/live-guide
- [Open-source] Alibaba open-sourced Qwen3-VL-235B-A22B-Instruct and Qwen3-VL-235B-A22B-Thinking, the most powerful Qwen vision-language models to date, supporting 256K context extendable to 1M, adding visual agent and visual coding capabilities. See https://modelscope.cn/models/Qwen/Qwen3-VL-235B-A22B-Instruct and https://modelscope.cn/models/Qwen/Qwen3-VL-235B-A22B-Thinking

### Sep 22
- [Closed-source | Omni-modal] Alibaba released qwen3-omni-flash and qwen3-omni-flash-realtime, multimodal models in the Qwen3 series that efficiently understand text, image, audio, and video, supporting text interaction in 119 languages, with excellent instruction following and system prompt customization — suitable for voice assistants, multimedia analysis, content creation, and more. See https://help.aliyun.com/zh/model-studio/qwen-omni
- [Closed-source | Speech Synthesis] The Alibaba Tongyi team released qwen3-tts-flash and qwen3-tts-flash-realtime, the latest offline speech synthesis models, with 17 highly expressive human-like voices, low-latency stable synthesis, and multilingual/dialect support. See https://help.aliyun.com/zh/model-studio/qwen-tts
- [Closed-source | Audio-video Translation] Alibaba released the real-time audio-video translation model qwen3-livetranslate-flash-realtime-2025-09-22, which recognizes 18 languages and translates in real time into audio in 10 languages. See https://help.aliyun.com/zh/model-studio/qwen3-livetranslate-flash-realtime
- [Open-source] Meituan released the LongCat-Flash-Thinking efficient reasoning model, reaching global open-source SOTA in logic, math, code, and agents. It is China's first model to simultaneously possess "deep thinking + tool calling" and "informal + formal" reasoning capabilities. See https://github.com/meituan-longcat/LongCat-Flash-Thinking
<br><br>


## Sep 15 ~ Sep 21
### Sep 19
- [Closed-source] Baidu released ERNIE-4.5-21B-A3B-Thinking, a lightweight deep-thinking model focused on improving reasoning quality and depth, with significant performance gains on logical reasoning, math, science, coding, and text generation tasks. See https://cloud.baidu.com/doc/WENXINWORKSHOP/s/flxu4ej5u

### Sep 17
- [Open-source] The Qwen team fully open-sourced Tongyi-DeepResearch-30B-A3B, an agentic large language model specifically for long-horizon, deep information-seeking tasks, demonstrating advanced performance on agentic search benchmarks. See https://modelscope.cn/models/iic/Tongyi-DeepResearch-30B-A3B
- [Open-source] Alibaba Tongyi Wanxiang released Wan2.2-Animate-14B, a digital human generation model supporting two modes — Animation (motion capture) and Replacement (character replacement) — enabling transformation from static images to animated characters. See https://modelscope.cn/models/Wan-AI/Wan2.2-Animate-14B

### Sep 15
- [Closed-source] OpenAI released GPT-5-codex, a GPT-5 variant optimized for agentic programming, supporting fast interactive editing and long-horizon independent tasks, with image or screenshot input accepted for frontend/UI work. See https://openai.com/index/introducing-upgrades-to-codex/
<br><br>


## Sep 8 ~ Sep 14
### Sep 12
- [Open-source] Qwen released Qwen3-Next, integrating hybrid attention, high-sparsity MoE, and multi-token prediction. Qwen3-Next-80B-A3B's performance in both "thinking mode" and "non-thinking mode" matches the larger Qwen3-235B-A22B-2507, while substantially improving inference speed, especially in long-context scenarios. See https://modelscope.cn/collections/Qwen3-Next-c314f23bd0264a

### Sep 11
- [Closed-source] The reasoning model qwen-plus-2025-09-11 is part of the Qwen3 series. Compared to qwen-plus-2025-07-28, in thinking mode it improves instruction following and produces more concise summaries — see https://help.aliyun.com/zh/model-studio/deep-thinking. In non-thinking mode, Chinese understanding and logical reasoning are enhanced — see https://help.aliyun.com/zh/model-studio/text-generation.

### Sep 10
- [Open-source] Tencent Hunyuan released HunyuanImage 2.1, supporting prompts up to 1000 tokens with fine-grained text control, natively and efficiently generating 2K images, using a 17B-parameter single/dual-stream DiT model. See https://modelscope.cn/models/Tencent-Hunyuan/HunyuanImage-2.1

### Sep 9
- [Closed-source] Google released Veo 3 and Veo 3 Fast officially with lower pricing and added aspect ratio, resolution, and seed options. See https://ai.google.dev/gemini-api/docs/video

### Sep 8
- [Closed-source] Alibaba released the CosyVoice-v3-plus and CosyVoice-v3 speech synthesis models, with significant improvements in naturalness, audio quality, prosody, and emotional expressiveness. See https://help.aliyun.com/zh/model-studio/text-to-speech
- [Open-source] The Bilibili speech team released IndexTTS2, introducing a voice-emotion decoupled modeling mechanism, supporting separate specification of voice reference and emotion reference for more flexible speech synthesis control. See https://www.modelscope.cn/models/IndexTeam/IndexTTS-2
<br><br>


## Sep 1 ~ Sep 7
### Sep 5
- [Closed-source] Alibaba released qwen3-max-preview, a Qwen3-based preview model with substantially improved general capabilities and reduced knowledge hallucinations over the Qwen 2.5 series. See https://help.aliyun.com/zh/model-studio/model-announcements
- [Open-source] Moonshot updated Kimi-K2-Instruct-0905, an MoE-architecture language model with 32B activated parameters and 1 trillion total parameters, with the context window expanded from 128k to 256k. See https://modelscope.cn/models/moonshotai/Kimi-K2-Instruct-0905

### Sep 3
- [Open-source] Tencent Hunyuan released HunyuanWorld-Voyager, the industry's first ultra-long-roaming world model supporting native 3D reconstruction, topping the comprehensive capability leaderboard on Stanford WorldScore. See https://modelscope.cn/models/Tencent-Hunyuan/HunyuanWorld-Voyager

### Sep 2
- [Open-source] Tencent Hunyuan released Hunyuan-MT-7B translation model, winning first place in 30 of 31 WMT25 competition languages, supporting mutual translation of 33 languages and 5 ethnic-Mandarin languages/dialects. See https://modelscope.cn/models/Tencent-Hunyuan/Hunyuan-MT-7B

### Sep 1
- [Open-source] Meituan released LongCat-Flash-Chat, a language model with 560B total parameters using MoE architecture, with 18.6B-31.3B activated, achieving efficient inference of over 100 tokens per second. See https://modelscope.cn/models/meituan-longcat/LongCat-Flash-Chat
<br><br>


## Aug 25 ~ Aug 31
### Aug 28
- [Closed-source] MiniMax released the first/last frame video generation feature for the Hailuo-02 model, adding a "last_frame_image" parameter to control the start and end frames of generated video. See https://platform.minimaxi.com/document/video_generation
- [Open-source] Tencent Hunyuan open-sourced HunyuanVideo-Foley, an end-to-end video sound effects generation model — just input video and text to match cinematic sound effects, ending the silent era of AI video. See https://modelscope.cn/models/Tencent-Hunyuan/HunyuanVideo-Foley

### Aug 26
- [Closed-source] Google launched the Gemini 2.5 Image Preview native image generation model with stronger image generation capabilities. See https://ai.google.dev/gemini-api/docs/models#gemini-2.5-flash-image-preview
- [Closed-source] xAI released its first code model Grok Code Fast 1, designed specifically for use in code editors. See https://docs.x.ai/docs/release-notes#grok-code-fast-1-is-released
- [Open-source] Alibaba Tongyi Wanxiang open-sourced Wan2.2-S2V, an audio-driven video generation model (14B parameters), capable of generating cinematic-quality high-quality video supporting full-body and half-body character generation. See https://www.modelscope.cn/studios/Wan-AI/Wan2.2-S2V
- [Open-source] Microsoft released VibeVoice-1.5B, a text-to-speech model supporting 90 minutes of continuous natural speech in a single session, with concurrent synthesis of 4 different speakers. See https://www.modelscope.cn/models/microsoft/VibeVoice-1.5B
- [Open-source] ModelBest released MiniCPM-V 4.5, an 8B-parameter multimodal model, the first multimodal model with "high refresh rate" video understanding, surpassing Qwen2.5-VL 72B. See https://www.modelscope.cn/models/OpenBMB/MiniCPM-V-4_5


## Aug 18 ~ Aug 24
### Aug 22
- [Closed-source] Alibaba released qwen-mt-image, the Qwen image translation model, supporting translation of text on images in 11 languages into Chinese or English, accurately preserving original layout and content information, with features like terminology definition, sensitive word filtering, and image subject detection. See https://help.aliyun.com/zh/model-studio/qwen-mt-image-api
- [Closed-source] Alibaba released qwen-deep-research, the Qwen deep research model that decomposes complex problems, performs reasoning and analysis combined with internet search, and generates research reports. See https://help.aliyun.com/zh/model-studio/qwen-deep-research
- [Closed-source] Alibaba released the fun-asr speech recognition model (stable and snapshot versions). FunASR is an end-to-end speech recognition model from Tongyi Lab with excellent context awareness and high-accuracy transcription, supporting Chinese and English recording file recognition. See https://help.aliyun.com/zh/model-studio/recording-file-recognition

### Aug 21
- [Open-source] DeepSeek released DeepSeek-V3.1 post-trained model, post-training optimizations on DeepSeek-V3.1-Base, whose base checkpoint was built via a two-stage long-context extension. See https://modelscope.cn/models/deepseek-ai/DeepSeek-V3.1
- [Open-source] ByteDance's Seed team released the Seed-OSS series of open-source large language models, trained on 12T tokens, providing strong long-context, reasoning, agentic, and general capabilities. Three versions:
  - Seed-OSS-36B-Base (with synthetic data): https://modelscope.cn/models/ByteDance-Seed/Seed-OSS-36B-Base
  - Seed-OSS-36B-Base-woSyn (without synthetic data): https://modelscope.cn/models/ByteDance-Seed/Seed-OSS-36B-Base-woSyn
  - Seed-OSS-36B-Instruct: https://modelscope.cn/models/ByteDance-Seed/Seed-OSS-36B-Instruct

### Aug 20
- [Closed-source] Alibaba released qwen-tts-vc-realtime-2025-08-20, an August 20, 2025 snapshot of the qwen-tts-realtime model, supporting voice cloning and multilingual speech synthesis. See https://help.aliyun.com/zh/model-studio/qwen-tts-realtime
- [Open-source] DeepSeek released DeepSeek-V3.1-Base, a hybrid model supporting both thinking and non-thinking modes. See https://modelscope.cn/models/deepseek-ai/DeepSeek-V3.1-Base

### Aug 19
- [Open-source] Alibaba released Qwen-Image-Edit, a Qwen image editing model further trained from the 20B Qwen-Image model, supporting dual semantic/appearance editing and precise bilingual Chinese-English text editing, achieving SOTA on multiple public benchmarks. See https://www.modelscope.cn/models/Qwen/Qwen-Image-Edit

### Aug 18
- [Closed-source] Google officially released the URL context tool, which can provide URLs as additional context for prompts. Support for using URL context with gemini-2.0-flash will end in 1 month. See https://ai.google.dev/gemini-api/docs/url-context?hl=zh-cn
<br><br>


## Aug 11 ~ Aug 17
### Aug 15
- [Open-source] Tencent released Hunyuan-GameCraft 1.0, a novel framework for game environment high-dynamic interactive video generation. It unifies keyboard and mouse input into a shared camera representation space and uses a hybrid history conditioning training strategy, trained on a million-scale game recording dataset of over 100 AAA games. See https://modelscope.cn/models/Tencent-Hunyuan/Hunyuan-GameCraft-1.0/summary

### Aug 14
- [Closed-source] Google officially released the Imagen 4 series (Ultra, Standard, Fast), supporting 2K resolution generation. See https://ai.google.dev/gemini-api/docs/imagen?hl=zh-cn

### Aug 13
- [Closed-source] Alibaba released qwen-vl-max-2025-08-13, a visual understanding model with improved multilingual processing and text rendering. See https://help.aliyun.com/zh/model-studio/vision/
- [Open-source] Skywork AI released Matrix-Game 2.0, the first open-source real-time long-sequence interactive world model, supporting 25 FPS video generation. See https://modelscope.cn/models/Skywork/Matrix-Game-2.0/summary

### Aug 12
- [Closed-source] Anthropic launched a 1-million-token context window for Claude Sonnet 4, a 5x capacity increase supporting processing of over 75,000 lines of code. See https://docs.anthropic.com/en/docs/build-with-claude/context-windows#1m-token-context-window
- [Open-source] Baichuan released Baichuan-M2-32B, a medical-enhanced reasoning model built on Qwen2.5-32B using a large verification system and multi-stage reinforcement learning strategy, surpassing all open-source models on HealthBench and reaching medical capabilities close to GPT-5. See https://modelscope.cn/models/baichuan-inc/Baichuan-M2-32B/summary

### Aug 11
- [Closed-source] Alibaba released wan2.2-i2v-flash, the Wanxiang 2.2 turbo model. Compared to the 2.1 model, it shows significant improvements in visual detail and motion stability, with generation speed up to 50% faster. See https://help.aliyun.com/zh/model-studio/image-to-video-api-reference/
- [Open-source] Zhipu AI released GLM-4.5V, a vision-language model based on GLM-4.5-Air (106B parameters, 12B activated), achieving same-tier open-source SOTA on 42 public visual multimodal leaderboards, supporting image reasoning, video understanding, GUI tasks, and a thinking mode toggle. See https://modelscope.cn/models/ZhipuAI/GLM-4.5V/summary
<br><br>


## Aug 4 ~ Aug 10
### Aug 8
- [Closed-source] Search results content blocks are now generally available on the Anthropic API and Google Cloud's Vertex AI. This feature enables natural citations with proper source attribution for RAG applications. The June 9, 2025 beta header search-results-2025-06-09 is no longer required. See the search results documentation for more https://docs.anthropic.com/en/docs/build-with-claude/search-results.

### Aug 7
- [Closed-source] Google Gemini image-to-video generation allow-adult-content setting is now available in restricted regions. See the Veo page https://ai.google.dev/gemini-api/docs/video?example=dialogue#veo-model-parameters.
- [Closed-source] OpenAI released the new-generation flagship model GPT-5 (also includes mini/nano lightweight models), which is also the new default model for all signed-in users. It simplifies ChatGPT, integrating it into an automatically switching system that combines the strengths of previous models into one intelligent and efficient new model. All ChatGPT plan users can use GPT-5. Paid plan users (Plus, Pro, Team) can use the model selector to manually choose GPT-5 or GPT-5 Thinking. Pro and Team plan users can use GPT-5 Thinking Pro, which takes slightly longer to think but delivers the high precision needed for complex tasks. Learn more about GPT-5 in ChatGPT https://help.openai.com/en/articles/11909943.

### Aug 6
- [Closed-source] MiniMax released the Speech 2.5 voice model, a new-generation speech generation model with ultimate similarity and more language support.

### Aug 5
- [Open-source] OpenAI officially open-sourced the gpt-oss-120b / 20b series of large models, designed for powerful reasoning, agentic tasks, and versatile development scenarios. They can be deployed locally on a single H100 or 16 GB memory, supporting adjustable reasoning depth, full chain-of-thought, function calling, web browsing, and LoRA fine-tuning. The two models: gpt-oss-120b — suitable for production environments, general purposes, and high-reasoning-demand scenarios, fits in a single H100 GPU (117B parameters with 5.1B activated); gpt-oss-20b — suitable for low-latency and local or specific-purpose scenarios (21B parameters with 3.6B activated). Model links: [gpt-oss-120b](https://modelscope.cn/models/openai-mirror/gpt-oss-120b), [gpt-oss-20b](https://modelscope.cn/models/openai-mirror/gpt-oss-20b)
- [Closed-source] Anthropic introduced Claude Opus 4.1, an incremental update to Claude Opus 4 with enhanced capabilities and performance improvements. See the models and pricing docs https://docs.anthropic.com/en/docs/about-claude/models.

### Aug 4
- [Open-source | Image Generation] The Qwen team open-sourced its first image generation foundation model Qwen-Image, a 20B MMDiT model showing significant progress in complex text rendering and precise image editing. Key features include: outstanding text rendering — Qwen-Image excels at complex text rendering, supporting multi-line layout, paragraph-level text generation, and fine-grained detail, achieving high-fidelity output in both English and Chinese; consistent image editing (coming soon) — through enhanced multi-task training, Qwen-Image excellently maintains editing consistency during editing; strong cross-benchmark performance — evaluations on multiple public benchmarks show Qwen-Image achieves SOTA on various generation and editing tasks, making it a powerful image generation foundation model. The ModelScope community AIGC section now supports online inference and training for Qwen-Image. Model link: https://www.modelscope.cn/models/Qwen/Qwen-Image.
<br><br>


## Jul 28 ~ Aug 3
### Aug 1
- [Closed-source] The Kimi K2 high-speed model kimi-k2-turbo-preview is officially Released. (Note: kimi-k2 is open-source, but kimi-k2-turbo has no corresponding open-source version.)

### Jul 31
- [Open-source] StepFun released the step-3 model, which has powerful visual perception and complex reasoning, capable of accurately handling complex domain-knowledge understanding, cross analysis of math and real-world information, and various visual analysis problems in daily life. See https://platform.stepfun.com/docs/llm/reasoning.
- [Closed-source] Google released the Veo 3 preview model, adding an image-to-video feature for Veo 3 preview, and released Veo 3 Fast preview to further improve generation efficiency. For Veo 3 details, visit https://ai.google.dev/gemini-api/docs/video?hl=zh-cn&example=dialogue.

### Jul 30
- [Open-source] Tencent released on-device hybrid reasoning models: Hunyuan-0.5B, Hunyuan-1.8B, Hunyuan-4B, Hunyuan-7B — an open-source efficient LLM series designed for flexible deployment across diverse compute environments, supporting fast/slow thinking dual-mode reasoning, 256K ultra-long context understanding, and Grouped Query Attention (GQA) for efficient inference. See https://modelscope.cn/models/Tencent-Hunyuan/Hunyuan-1.8B-Instruct

### Jul 29
- [Closed-source] OpenAI launched the ChatGPT Study Mode feature, a new learning experience using Socratic questioning to guide understanding, personalized responses, and open-ended feedback checks, helping users build deep understanding of any topic. Currently open to Free, Plus, Pro, and Teams users. Official intro: https://help.openai.com/en/articles/6825453-chatgpt-release-notes

### Jul 28
- [Closed-source] Alibaba released qwen-flash-2025-07-28 and qwen3-coder-flash-2025-07-28
- [Closed-source] Alibaba released the wan2.2-i2v-plus image-to-video model. Compared to 2.1, the new version shows significant improvements in visual detail and motion stability, with generation speed up to 50% faster. For details, visit https://help.aliyun.com/zh/model-studio/image-to-video-api-reference.
- [Closed-source] Alibaba released the wan2.2-t2v-plus text-to-video model. The new version shows significant improvements in visual detail and motion stability, with generation speed up to 50% faster. See https://help.aliyun.com/zh/model-studio/text-to-video-api-reference.
- [Closed-source] Alibaba released wan2.2-t2i-flash and wan2.2-t2i-plus text-to-image models. Compared to 2.1, the new versions comprehensively upgrade creativity, stability, and photorealism, with generation speed up to 50% faster. See https://help.aliyun.com/zh/model-studio/text-to-image-v2-api-reference.
- [Open-source] Zhipu released the GLM-4.5 series. GLM-4.5 has 355B total parameters and 32B activated; GLM-4.5-Air uses a more compact design with 106B total and 12B activated. Both are hybrid reasoning models offering both a thinking mode for complex reasoning and tool use, and a non-thinking mode for instant responses. For details, see: https://docs.z.ai/guides/llm/glm-4.5
<br><br>


## Jul 21 ~ Jul 27
### Jul 27
- [Open-source | Multimodal Generation] Tencent released HunyuanWorld-1.0, the first open-source immersive 3D world generation model, supporting generation of roamable, interactive 360-degree virtual worlds from text or images. For more, visit https://3d-models.hunyuan.tencent.com/world/

### Jul 25
- [Closed-source] iFlytek released the upgraded version of Spark X1, xunfei-spark-x1-0725, a deep reasoning large model trained on fully domestic compute, with significant improvements in mathematical operations, logical reasoning, and hallucination handling, supporting 130+ languages. See the official introduction https://xinghuo.xfyun.cn/sparkapi.
- [Open-source] Alibaba released Qwen3-235B-A22B-Thinking-2507, a thinking-enhanced version of Qwen 3-235B-A22B with significant improvements on reasoning tasks such as logic, math, science, and coding, supporting 256K long context understanding. For more, visit https://modelscope.cn/models/Qwen/Qwen3-235B-A22B-Thinking-2507/summary.

### Jul 24
- [Open-source] Infinigence AI released Megrez2-3x7B-A3B-Preview, an MoE-architecture large model designed specifically for terminal devices, trained on 5T tokens. For more, visit https://modelscope.cn/models/InfiniAI/Megrez2-3x7B-A3B-Preview/summary.
- [Open-source] Shanghai AI Laboratory released the open-source multimodal scientific reasoning model Intern-S1, built on a 235B MoE language model and a 6B vision encoder, pretrained on 5T multimodal data. For more, visit https://modelscope.cn/models/Shanghai_AI_Laboratory/Intern-S1/summary.

### Jul 23
- [Closed-source | Multimodal Fusion] SenseTime released SenseNova-V6.5-Pro and SenseNova-V6.5-Turbo, the latest updates to the SenseNova fusion-modality model, focused on enhancing reasoning and improving training efficiency. For more, visit the model page https://console.sensecore.cn/micro/help/docs/model-as-a-service/nova/model/fusionllm/FusionLLMs/.
- [Open-source] Alibaba released Qwen3-Coder-480B-A35B-Instruct, which excels at foundational coding tasks such as agentic programming and agentic browser use, natively supporting 256K context extendable to 1M, optimized for repository-scale understanding, supporting agentic coding on most platforms including Qwen Code and CLINE. For more, visit https://modelscope.cn/models/Qwen/Qwen3-Coder-480B-A35B-Instruct/summary.

### Jul 22
- [Open-source] Kuaishou released KAT-V1-40B. Kwaipilot-AutoThink ranks first among all open-source models on LiveCodeBench Pro, a challenging benchmark designed to prevent data leakage, even surpassing powerful proprietary systems such as Seed and o3-mini. See https://modelscope.cn/models/Kwaipilot/KAT-V1-40B.
- [Closed-source] Google released gemini-2.5-flash-lite, the lightweight version of the Gemini 2.5 series, focused on the balance of speed, low cost, and high performance. For more on Gemini 2.5 Flash-Lite, visit the model page https://ai.google.dev/gemini-api/docs/models?hl=zh-cn#gemini-2.5-flash-lite.

### Jul 21
- [Open-source] Alibaba released Qwen3-235B-A22B-Instruct-2507, an updated non-thinking-mode version of Qwen 3 with significant improvements in general capability, logical reasoning, and 256K long-text understanding, with substantially expanded multilingual knowledge coverage. For more, visit https://modelscope.cn/models/Qwen/Qwen3-235B-A22B-Instruct-2507/summary.
<br><br>


## Jul 14 ~ Jul 20
### Jul 17
- [Closed-source | Multimodal Generation] Google released veo-3.0-generate-preview, the latest update to Veo, introducing video and audio generation. For more on Veo 3, visit the [model page](https://ai.google.dev/gemini-api/docs/models#veo-3).
- [Closed-source] Google increased the rate limits of Imagen 4 Standard and Ultra. For details, visit the [rate limits page](https://ai.google.dev/gemini-api/docs/rate-limits).
- [Closed-source] Anthropic has increased the Claude Sonnet 4 API rate limits, so you can more easily build and scale Claude applications. For customers on rate limit tiers 1-4, these changes are applied to your account immediately — no action required.
- [Open-source | Multimodal Generation] HiDream-E1-1: The HiDream team at Vivago AI recently open-sourced the latest iteration of its image editing model. Supports dynamic resolution, with significant improvements in image quality and editing precision over the previous HiDream-E1-Full. [Model link](https://www.modelscope.cn/models/HiDream-ai/HiDream-E1-1).

### Jul 16
- [Closed-source] Tencent released a new TurboS version hunyuan-turbos-20250716.
- [Open-source | Multimodal Understanding] The Voxtral series is the first open audio model released by Mistral AI. Built on Mistral Small 3, it adds powerful audio understanding capabilities.
  - Dedicated transcription mode: Can operate in pure speech transcription mode for maximum performance. By default, Voxtral automatically predicts the source audio language and transcribes accordingly.
  - Long-form content: With a 32k-token context length, it can handle up to 30 minutes of audio transcription or 40 minutes of understanding.
  - Built-in Q&A and summarization: Supports asking questions directly through audio. Analyzes audio and generates structured summaries without separate ASR and language models.
  - Native multilingual support: Automatic language detection and leading performance in the most widely used global languages (English, Spanish, French, Portuguese, Hindi, German, Dutch, Italian).
  - Function calls directly from speech: Trigger backend functions, workflows, or API calls based on user speech intent.
  - Strong text understanding: Retains the text understanding capabilities of its language model foundation Mistral Small 3.1.
  - Model links: [Voxtral-Small-24B-2507](https://modelscope.cn/models/mistralai/Voxtral-Small-24B-2507), [Voxtral-Mini-3B-2507](https://www.modelscope.cn/models/mistralai/Voxtral-Mini-3B-2507)

### Jul 15
  - [Closed-source | Multimodal Generation] Zhipu CogVideoX-3 video generation model is launched, a newly upgraded video generation large model supporting text-to-video and image-to-video, adding first/last frame generation, with significantly improved subjective clarity, natural and smooth large-motion subjects, and improved performance on HD realistic and 3D-style scenes. See [CogVideoX-3](https://bigmodel.cn/dev/howuse/video-generation-model/CogVideoX-3)
  - [Closed-source | Text] Doubao released doubao-seed-1-6-thinking-250715
  - [Closed-source | Text] Alibaba released qwen-turbo-2025-07-15

### Jul 14
  - [Closed-source | Text] Alibaba released qwen-plus-2025-07-14
  - [Closed-source | Embedding] Google released gemini-embedding-001, the stable version of the text embedding model. For more, see the [page](https://ai.google.dev/gemini-api/docs/embeddings). The gemini-embedding-exp-03-07 model will be deprecated on August 14, 2025.


<br><br>
## Jul 7 ~ Jul 13
### Jul 11
- [Open-source | Text] Kimi K2: the first trillion-parameter open-source model. The latest open-source release from Moonshot, an MoE-architecture base model with stronger coding ability and excelling at general Agent tasks, with 1T total parameters and 32B activated. On benchmarks such as SWE Bench Verified, Tau2, and AceBench, Kimi K2 achieves open-source SOTA, demonstrating leading capabilities in code, Agent, and math reasoning. API pricing: input ¥4 per million tokens, output ¥16 per million tokens. Model download: [Kimi-K2-Instruct](https://www.modelscope.cn/models/moonshotai/Kimi-K2-Instruct). Technical blog: [Kimi-K2](https://moonshotai.github.io/Kimi-K2/).
- [Open-source | Text] Phi-4-mini-flash-reasoning: a member of Microsoft's Phi-4 family, a lightweight open model built on synthetic data, focused on high-quality dense reasoning data, further fine-tuned to enhance advanced math reasoning, supporting 64K-token context. Designed for multi-step, logic-intensive math problem-solving tasks in memory/compute-constrained environments and latency-bound scenarios, excelling at maintaining context across steps, applying structured logic, and providing accurate and reliable solutions in domains requiring deep analytical thinking. Model download: [Phi-4-mini-flash-reasoning](https://modelscope.cn/models/LLM-Research/Phi-4-mini-flash-reasoning).
- [Closed-source | Text] Tencent released hunyuan-t1-20250711

### Jul 10
- [Closed-source] Grok4: Musk's xAI released what is dubbed the "strongest model in the universe", breaking multiple records. On the authoritative test "Humanity's Last Exam" (containing 2500 PhD-level difficult problems spanning math, science, and humanities), Grok 4 achieved 25.4% accuracy, surpassing Google Gemini 2.5 Pro (21.6%) and OpenAI o3 (21%). Musk said it "outperforms PhD level in all disciplines". Single/multi-agent collaboration: the basic version is single-agent; Grok 4 Heavy supports 4-agent parallel reasoning, improving complex problem-solving through collaboration. Subscription model: standard $30/month, Grok 4 Heavy $300/month (currently the most expensive AI subscription). API pricing: input $3 per million tokens, output $15 per million tokens. Official intro: [grok-4](https://x.ai/news/grok-4). [Launch link](https://x.com/xai/status/1943158495588815072).

### Jul 9
- [Open-source] SmolLM3: An open-source 3B-parameter language model by HuggingFace, aimed at pushing the boundaries of small models. It supports dual-mode reasoning, 6 languages, and long contexts, with context handling extendable from 64K to 128K. SmolLM3 is a fully open model offering strong performance at the 3B-4B scale. SmolLM3 not only publishes model weights but also fully open-sources the training data mix, training configuration, and code. Developers can obtain detailed materials from the HuggingFace smollm repository.
Model download: [SmolLM3-3B](https://modelscope.cn/models/HuggingFaceTB/SmolLM3-3B)
- [Open-source] Skywork-R1V3-38B: the latest and most powerful open-source multimodal reasoning model in the Kunlun Skywork-R1V series. Built on InternVL-38B, it significantly advances the frontier of multimodal and cross-disciplinary intelligence. Primarily through RL algorithms in post-training, R1V3's reasoning is enhanced, achieving open-source state-of-the-art (SOTA) performance on numerous multimodal reasoning benchmarks. Model download: [Skywork-R1V3-38B](https://modelscope.cn/models/Skywork/Skywork-R1V3-38B)

### Jul 7
- [Closed-source] Google launched the Gemini API batch mode. Requests can be batched and sent asynchronously.
<br><br>


## Jun 30 ~ Jul 6
### Jul 3
- [Closed-source] Claude introduced a beta for search results content blocks, enabling RAG applications to perform citations naturally. Tools can now return search results with proper source attribution, and Claude will automatically cite these sources in replies — with citation quality matching web search. This removes the need for document workarounds in custom knowledge-base applications. See the search results docs for details. To enable, use the beta header search-results-2025-06-09.

### Jul 2
- [Closed-source] Zhipu released the GLM-4.1V-Thinking series visual reasoning models. The GLM-4.1V-Thinking series is currently known to be the strongest 10B-scale visual reasoning model. It reaches comprehensive new SOTA on core capabilities like chart/video understanding, frontend coding, and GUI tasks, and introduces a chain-of-thought reasoning mechanism, significantly improving answer accuracy and interpretability in complex scenarios.
- [Open-source] Zhipu open-sourced GLM-4.1V-9B-Thinking, based on the GLM-4-9B-0414 base model — the new VLM open-source model GLM-4.1V-9B-Thinking. By introducing a thinking paradigm and using curriculum-sampled reinforcement learning (RLCS), it comprehensively improves capabilities to achieve the strongest performance at the 10B parameter scale, matching or surpassing the 8x-larger Qwen-2.5-VL-72B on 18 leaderboard tasks. The base model GLM-4.1V-9B-Base is also open-sourced, hoping to help more researchers explore the capability boundaries of vision-language models. Model download: [GLM-4.1V-9B-Thinking](https://modelscope.cn/models/ZhipuAI/GLM-4.1V-9B-Thinking).

### Jul 1
- [Open-source] Tongyi Lab open-sourced ThinkSound: chain-of-thought reasoning in multimodal LLMs for audio generation and editing. Although end-to-end video-to-audio generation has made great progress, generating high-fidelity audio that truly captures the nuances of visual content remains challenging. Like professionals in the creative industry, such generation requires complex reasoning about items such as visual dynamics, acoustic environments, and temporal relationships. ThinkSound is a novel framework that leverages chain-of-thought (CoT) reasoning to achieve step-by-step, interactive audio generation and editing. The approach decomposes the process into three complementary stages: foundational sound generation that creates semantically consistent soundscapes, object-centric refinement via precise user interaction, and targeted editing guided by natural language instructions. At each stage, multimodal LLMs generate context-aligned CoT reasoning to guide a unified audio foundation model. Additionally, AudioCoT is introduced — a comprehensive dataset with structured reasoning annotations establishing connections between visual content, textual descriptions, and sound synthesis. Experiments show ThinkSound achieves state-of-the-art performance in video-to-audio generation across both audio metrics and CoT metrics, and excels on out-of-distribution film-generated audio benchmarks. [Demo page](https://ThinkSound-Project.github.io), model download: [ThinkSound](https://modelscope.cn/models/iic/ThinkSound).

### Jun 30
- [Closed-source] Claude announced that the Claude Opus 3 model will soon be deprecated. See the [docs](https://docs.anthropic.com/en/docs/about-claude/model-deprecations) for details.
<br><br>


## Jun 23 ~ Jun 29
### Jun 29
- [Closed-source] ERNIE-4.5-Turbo-VL-Preview, with significantly improved image understanding, creation, translation, and code capabilities, supporting 128K context length and substantially reduced first-token latency.
- [Closed-source] Baidu ERNIE minor version upgrades: ERNIE-4.5-Turbo-VL-Preview and ERNIE-4.5-Turbo-128K-Preview.
- [Open-source] Baidu released open-source models: ERNIE-4.5-0.3B, ERNIE-4.5-21B-A3B, multimodal ERNIE-4.5-VL-28B-A3B, ERNIE-4.5-300B-A47B, multimodal ERNIE-4.5-VL-424B-A47B. Model download [ERNIE-4.5](https://modelscope.cn/collections/ERNIE-45-56f40e2777e348).

### Jun 27
- [Open-source] FLUX.1-Kontext-dev: FLUX.1 Kontext is a professional image generation and editing model open-sourced by Black Forest Labs, focused on precise image editing via context-aware technology. The model supports mixed text and image input, can intelligently understand image content and perform various editing tasks such as object modification, style transfer, and background replacement, while maintaining subject consistency well across multi-turn editing. Its core uses a flow matching architecture combined with a dual-stream and single-stream hybrid design, improving semantic association precision and generation speed. Flux.1 Kontext [dev] is now officially launched in the ModelScope AIGC section, supporting free online image editing. It also supports online GUI-based model training, allowing LoRA model training based on the Flux.1 Kontext [dev] base. Model download: [FLUX.1-Kontext-dev](https://modelscope.cn/models/black-forest-labs/FLUX.1-Kontext-dev).
- [Open-source] Google officially open-sourced Gemma 3n, an on-device multimodal model that runs natively on phones, tablets, and laptops, handling audio, text, image, and video data. Compared to the previous preview, the latest Gemma 3n full version further improves performance, supports local running on hardware with 2GB memory, and focuses on enhancing coding and reasoning. This open-source release provides two versions: 5B-parameter (E2B) and 8B-parameter (E4B), with actual memory footprint equivalent to 2B and 4B models respectively. It uses a MatFormer hierarchical nested architecture (like Russian dolls), supporting dynamic compute resource adjustment, combined with Per Layer Embeddings (PLE) and the MobileNet-v5 vision encoder, significantly improving memory efficiency and visual processing. The model enhances multilingual support (140 text languages, 35 multimodal understanding), math operations, code generation, and complex reasoning, suitable for offline intelligent assistants, real-time multimodal interaction, localized content generation, etc., balancing high performance and low power consumption. Model download: [gemma-3n-E2B-it](https://modelscope.cn/models/google/gemma-3n-E2B-it).

### Jun 26
- [Closed-source] Alibaba qwen-tts-2025-05-22, a May 22, 2025 snapshot of the qwen-tts model. Added three voices: Beijing dialect, Wu dialect, and Sichuan dialect.
- [Closed-source] The preview models gemini-2.5-pro-preview-05-06 and gemini-2.5-pro-preview-03-25 will now redirect to the latest stable version gemini-2.5-pro. gemini-2.5-pro-exp-03-25 has been deprecated.
- [Closed-source] OpenAI released two brand-new Deep Research APIs: o3-deep-research-2025-06-26 and o4-mini-deep-research-2025-06-26, designed for high-order analysis and deep information synthesis, enabling automated web search, data analysis, code execution, etc., supporting multi-step research and generating structured, cited reports.
- [Closed-source] Alibaba Qwen launched Qwen VLo, a multimodal unified understanding and generation model, introducing a top-to-bottom, left-to-right progressively clarifying generation process, suitable for long-paragraph text generation tasks requiring fine-grained control. See [qwen-vlo](https://qwenlm.github.io/zh/blog/qwen-vlo). Not open-source, no API released. [Try it](https://chat.qwen.ai).
- [Open-source] Kuaishou open-sourced the new multimodal large model Keye-VL-8B-Preview, able to convert video content into solutions, with intelligent thinking-mode selection balancing efficiency and creativity. Model download [Keye-VL-8B-Preview](https://huggingface.co/Kwai-Keye/Keye-VL-8B-Preview).

### Jun 25
- [Open-source] hunyuan-a13b is launched. Use cases: most scenarios, balancing performance and inference performance. Capabilities and features: Hunyuan's first hybrid reasoning model, an upgrade of hunyuan-standard-256K, 80B total parameters with 13B activated. Default is slow-thinking mode, supporting switching between fast/slow thinking via parameters or instructions; slow/fast thinking switching by prepending /no_think to the query. Overall capability comprehensively improved over the previous generation, particularly significant improvements in math, science, long-text understanding, and Agent capabilities. Model architecture: Hunyuan MoE structure. Tencent Hunyuan announced the open-sourcing of its first hybrid reasoning MoE model Hunyuan-A13B, with 80B total parameters and only 13B activated, comparable to leading open-source models with the same architecture, with faster inference and better cost-performance. Model download [Hunyuan-A13B-Instruct](https://modelscope.cn/models/Tencent-Hunyuan/Hunyuan-A13B-Instruct).
- [Closed-source] Baidu ERNIE-4.5-Turbo-128K-Preview comprehensively improves model capabilities, better serving multi-turn long-history dialogue handling and long-document understanding Q&A tasks. This version is the latest in this series.
- [Open-source] Jina AI officially open-sourced jina-embeddings-v4, a brand-new multimodal embedding model with 3.8 billion parameters, achieving simultaneous text and image processing for the first time. To maximize performance across various retrieval tasks, the model has built-in task-specific LoRA adapters, specifically enhancing performance on query-document retrieval, semantic matching, and code search. On benchmarks such as MTEB, MMTEB, CoIR, LongEmbed, STS, Jina-VDR, and ViDoRe, jina-embeddings-v4 demonstrates top performance on multimodal and multilingual retrieval. It particularly excels at interpreting visually rich content — whether tables, charts, or complex diagrams — precisely capturing deep semantics. The model also supports both single-vector and multi-vector representations, flexibly meeting various scenario needs. Model download: [jina-embeddings-v4](https://modelscope.cn/models/jinaai/jina-embeddings-v4).

### Jun 24
- [Closed-source] Google released Imagen 4 Ultra and Standard preview models. For more, see the [image generation page](https://ai.google.dev/gemini-api/docs/image-generation).

### Jun 23
- [Closed-source] Baidu ERNIE-X1-Turbo-32K-Preview, better effects and performance compared to ERNIE-X1-Turbo-32K.
- [Open-source] Moonshot AI open-sourced the multimodal model Kimi-VL-A3B-Thinking-2506. With 2.8B activated parameters, a 128K context window, and a Mixture-of-Experts architecture, it demonstrates strong visual understanding, reasoning, and long-text/long-video processing. Model download [Kimi-VL-A3B-Thinking-2506](https://modelscope.cn/models/moonshotai/Kimi-VL-A3B-Thinking-2506).
<br><br>


## Jun 16 ~ Jun 22
### Jun 22
- [Closed-source] MiniMax music model music-1.5 released, a new-generation music generation model supporting music generation from musical inspiration and lyrics.

### Jun 19
- [Closed-source] hunyuan-t1-vision-20250619 is launched. Features: Hunyuan's latest t1-vision multimodal-understanding deep-thinking model, supporting multimodal native long chain-of-thought, comprehensively improved over the previous default version.
- [Closed-source] hunyuan-turbos-vision-20250619 is launched. Features: Hunyuan's latest turbos-vision vision-language flagship large model, comprehensively improved on image-text understanding tasks (including image-based entity recognition, knowledge Q&A, copywriting, photo problem-solving, etc.) over the previous default version.

### Jun 18
- [Closed-source] Zhipu integrated two popular Vidu video generation models
  - Vidu Q1 focuses on high-quality video creation, with fixed output of 5 seconds, 24 frames, 1080P content. With deep clarity optimization, the visual quality has substantially improved; the realistic style approaches real scenes, the 2D animation style is precisely maintained, and first/last frame transitions are smoother — suitable for film, advertising, anime short drama, and other demanding creation scenarios.
  - Vidu 2 balances speed, quality, and cost, focusing on image-to-video and first/last frame features, supporting 720P resolution output at 4-second duration. The visuals are stable and controllable, suitable for e-commerce and other scenarios; first/last frame semantic understanding and multi-reference image consistency are enhanced, making it an efficient tool for pan-entertainment, internet, anime short drama, and large-scale ad production.
- [Closed-source] The MiniMax video model MiniMax Hailuo 02 is officially Released, a new-generation video generation model supporting 1080P HD and longer 10s videos.

### Jun 17
- [Closed-source] Google released gemini-2.5-pro, the stable version of the most powerful model, now with adaptive thinking. gemini-2.5-pro-preview-05-06 will redirect to gemini-2.5-pro on June 26, 2025.
- [Closed-source] Google released gemini-2.5-flash, the first stable 2.5 Flash model. gemini-2.5-flash-preview-04-17 will be deprecated on July 15, 2025.
- [Closed-source] Google released gemini-2.5-flash-lite-preview-06-17, a low-cost, high-performance Gemini 2.5 model.
- [Open-source] Kimi-Dev-72B is the latest open-source large coding language model from Kimi, designed for software engineering tasks. Through large-scale RL optimization, it can automatically fix vulnerabilities in real code repositories and pass test verification. It sets a new record for open-source models on the SWE-bench Verified dataset with 60.4% performance. Model download: [Kimi-Dev-72B](https://modelscope.cn/models/moonshotai/Kimi-Dev-72B).

### Jun 16
- [Open-source] MiniMax's reasoning model MiniMax-M1 is officially Released — global leadership: 80K chain-of-thought x 1M input, rivaling top overseas models. MiniMax-M1 is the world's first open-source large-scale hybrid-architecture reasoning model recently released by MiniMax, supporting million-level context input and up to 80K-token reasoning output, with 456B total parameters and 45.9B activated per token. It performs excellently on complex tasks such as long-context understanding, software engineering, and tool use, with extremely high cost-performance, and achieves efficient training via the innovative reinforcement learning algorithm CISPO. Model download: [MiniMax-M1-80k](https://modelscope.cn/models/MiniMax/MiniMax-M1-80k).
- [Open-source] Lingshu series: Lingshu-7B is an LLM open-sourced by Alibaba DAMO Academy focused on the medical domain, with two parameter versions of 7B and 32B. It achieves SOTA performance on most medical multimodal/text QA and report generation tasks, providing efficient support for medical text processing, clinical decision support, and medical Q&A. Lingshu-32B outperforms GPT-4.1 and Claude Sonnet 4 on most multimodal QA and report generation tasks. Lingshu supports over 12 medical imaging modalities including X-ray, CT, MRI, microscopy, ultrasound, histopathology, dermoscopy, fundus, OCT, digital photography, endoscopy, and PET. Model download: [Lingshu-32B](https://modelscope.cn/models/DAMO_Academy/Lingshu-32B).
<br><br>


## Jun 9 ~ Jun 15
### Jun 15
- [Closed-source] ByteDance Doubao-Seed-1.6-thinking has significantly enhanced thinking, with further improvements over Doubao-1.5-thinking-pro on Coding, Math, logical reasoning, and other fundamental capabilities.
- [Closed-source] Doubao-Seed-1.6, a brand-new multimodal deep-thinking model, supporting thinking/non-thinking/auto modes, with the non-thinking version substantially improved over Doubao-1.5-pro/250115.
- [Closed-source] Doubao-Seed-1.6-flash, a multimodal deep-thinking model with extreme inference speed, supporting both text and visual understanding, with text understanding surpassing the previous-generation lite and visual understanding rivaling competitors' pro series.

### Jun 13
- [Open-source] Nanonets-OCR-s is a powerful OCR model fine-tuned from Qwen2.5-VL-3B, runnable on 9G VRAM, capable of converting messy documents into clean, structured, and contextually rich Markdown format needed for modern AI applications through intelligent content recognition and semantic markup. Its capabilities go far beyond traditional text extraction, currently the SOTA model for image-to-Markdown. Model download: [Nanonets-OCR-s](https://modelscope.cn/models/nanonets/Nanonets-OCR-s).

### Jun 11
- [Open-source] Magistral-Small-2506 is an upgraded model based on Mistral Small 3.1 (2503), with reasoning significantly enhanced through supervised fine-tuning (SFT) on Magistral Medium trajectories combined with RL training. This efficient small reasoning model has 24B parameters and after quantization can be deployed locally on a single RTX 4090 or a 32GB MacBook. Magistral-Small-2506 has long-reasoning-chain capability, supporting English, French, Chinese, and dozens of other languages, under Apache 2.0 (commercial and non-commercial use allowed). Its 128k context window is actually recommended to be set at 40k — performance may degrade beyond that. Model download: [Magistral-Small-2506](https://modelscope.cn/models/mistralai/Magistral-Small-2506).

### Jun 10
- [Closed-source] OpenAI launched o3-pro. Like o1-pro, o3-pro is a version of the most intelligent model o3, designed for long-time thinking and providing the most reliable answers. Since o1-pro launched, users have favored it for performance in areas such as math, science, and programming, and o3-pro continues to perform excellently in these domains on academic evaluations. Like o3, o3-pro can use various tools that make ChatGPT more practical — it can search the web, analyze files, reason about visual inputs, use Python, leverage memory for personalized answers, and more.

### Jun 9
- [Open-source] MonkeyOCR is a document parsing model launched by Huazhong University of Science and Technology and Kingsoft Office, featuring high accuracy and strong generalization. The model supports text detection and recognition in multiple languages and scenarios, suitable for document digitization, content moderation, information extraction, and various other applications. Compared to traditional methods, MonkeyOCR averages 5.1% performance improvement on complex documents, with 15% and 8.6% improvements on formula and table parsing respectively. Model download: [MonkeyOCR](https://modelscope.cn/models/l1731396519/MonkeyOCR).


<br><br>
## Jun 2 ~ Jun 8
### Jun 7
- [Closed-source] OpenAI advanced voice mode update — upgraded advanced voice mode for paid users in ChatGPT, significantly improving tone and naturalness for smoother and more natural conversations.

### Jun 6
- [Closed-source] OpenAI o4-mini update — rolled back the o4-mini snapshot deployed less than a week earlier, originally intended to lengthen model responses but withdrawn after automated monitoring tools found an increase in content flags.
- [Closed-source] hunyuan-translation-lite model version update. Capabilities and features: Hunyuan translation-specific model, optimized for translation based on the Hunyuan 2B-Dense model, strengthening multilingual translation through iterative high-quality multilingual SFT data. Supports mutual translation across 18 languages including Simplified Chinese, Traditional Chinese, Cantonese, Indonesian, English, Japanese, French, Portuguese, Spanish, Turkish, Russian, Arabic, Korean, Italian, German, Vietnamese, Malay, and Indonesian. Architecture: Hunyuan Dense.
- [Open-source] dots.llm1 is a large-scale MoE model launched by Xiaohongshu's Hi lab team (Humane Intelligence Lab), activating 14B parameters out of a total of 142B, with performance comparable to current state-of-the-art open-source models. Through the rednote-hilab research team's carefully designed and efficient data processing pipeline, dots.llm1 — pretrained on a high-quality corpus without synthetic data — reaches performance comparable to Qwen2.5-72B. To further promote research, the team open-sourced intermediate training checkpoints throughout training and provides valuable insights into the learning dynamics of large language models. Model download: [dots.llm1.inst](https://modelscope.cn/models/rednote-hilab/dots.llm1.inst).

### Jun 5
- [Closed-source] Google released gemini-2.5-pro-preview-06-05, a new version of the most powerful model, now with adaptive thinking. For more, see Gemini 2.5 Pro preview and thinking. gemini-2.5-pro-preview-05-06 will redirect to gemini-2.5-pro on June 26, 2025.
- [Open-source] ModelBest unveiled MiniCPM 4.0 — an extremely efficient on-device large model. Through its proprietary CPM.cu inference framework, it achieves up to 220x speed improvement and 5x typical speedup. The open-source community release features two parameter scales — 8B and 0.5B — both achieving best-in-class performance among same-tier models. The MiniCPM4 series achieves extreme on-device inference efficiency through systematic technical innovation: it uses the trainable sparse attention architecture InfLLM v2, compressing token-association computation to under 5% on 128K long-text processing; combined with BitCPM ternary quantization for 90% bit-width compression, plus FP8 low-precision computation and multi-token prediction substantially reducing training costs; building a high-quality multidimensional training set via UltraClean data cleaning and UltraChat v2 synthesis; integrating the efficient CUDA framework CPM.cu on the inference side, fusing sparse attention, model quantization, and speculative decoding, and achieving flexible deployment via the cross-platform ArkInfer system. Model download: [MiniCPM4-0.5B](https://modelscope.cn/models/OpenBMB/MiniCPM4-0.5B).

### Jun 4
- [Closed-source] Tencent Hunyuan hunyuan-turbos-20250604 is launched. Capabilities and features: pretraining base upgrade, improved writing and reading comprehension, significantly improved code and STEM capabilities, continued improvement in complex instruction following, etc.
- [Closed-source] Alibaba released text-embedding-v4, an upgrade of text-embedding-v3, part of the Qwen3-Embedding series. Compared to the previous version, it covers more natural languages and multiple programming languages, and adds 2048 and 1536 vector dimension options.
- [Open-source] Alibaba Tongyi Lab open-sourced the Qwen3-Embedding series, a new member of the Qwen family. The series is designed for text representation, retrieval, and ranking tasks, trained on the Qwen3 base model, fully inheriting Qwen3's strengths in multilingual text understanding. Built on the Qwen3 base, the Embedding model and Reranker model use dual-tower and single-tower architectures respectively. Via LoRA fine-tuning, they maximally preserve and inherit the text understanding capabilities of the base model. Model download: [Qwen3-Embedding-8B](https://modelscope.cn/models/Qwen/Qwen3-Embedding-8B).

### Jun 3
- [Closed-source] Alibaba released qvq-max-2025-05-15, a visual reasoning model. Compared to the previous version, capabilities in math, programming, visual analysis, creation, and general tasks have been enhanced.
- [Closed-source] Alibaba released qvq-plus-2025-05-15, a visual reasoning model. Supports visual input and chain-of-thought output. As the plus version following the qvq-max model, qvq-plus has faster inference speed with a balanced trade-off between effect and cost.
- [Closed-source] SenseTime released the latest SenseNova Speech Large Model — Speech Synthesis (Voice Fusion). The SenseNova speech synthesis (voice fusion) large model is based on synchronous text-to-speech (TTS) functionality, supporting up to 10,000 characters per request, suitable for various scenarios such as short-sentence generation, voice dialogue, and online social interaction.




