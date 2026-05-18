
# ReLE Benchmark: Chinese AI Model Capability Evaluation (continuously updated)
- ReLE (**R**eally R**e**liable **L**ive **E**valuation for LLM), formerly known as CLiB
- Currently covers 377 models, including commercial models such as chatgpt, gpt-5.5, Google gemini-3.1-pro, Claude-4.6, ERNIE-X1.1, ERNIE-5.1, qwen3.6-max, qwen3.6-plus, Baichuan, iFlytek Spark, SenseTime senseChat, and many more,
as well as open-source models such as step3.5-flash, kimi-k2.6, ernie4.5, MiniMax-M2.7, deepseek-v4, Qwen3.6, llama4, Zhipu GLM-5.1, MiMo-V2, LongCat, gemma4, and mistral.
- Supports multi-dimensional capability evaluation across 7 domains — Education, Medical & Mental Health, Finance, Law & Public Administration, Reasoning & Math, Language & Instruction Following, and Agent & Tool Use — plus around 300 fine-grained sub-dimensions (e.g., dentistry, high-school Chinese, etc.). See our technical report [ReLE: A Scalable System and Structured Benchmark for Diagnosing Capability Anisotropy in Chinese LLMs](https://www.arxiv.org/abs/2601.17399). Media coverage (Synced/Jiqizhixin): [Real-world testing of 304 Chinese LLMs worldwide: no "all-around champion"; ReLE breaks the evaluation deadlock with a 70% cost-reduction solution](https://www.jiqizhixin.com/articles/2026-02-03)
- Beyond the leaderboard, we also provide a **defect library with over 2 million model failures** to help the community study and improve LLMs.
- We offer free evaluation services for your private models. Contact us (Nonelinear AI ReLE benchmark team): [Add WeChat](#contact-us-nonelinear-ai-rele-benchmark-team)


# Table of Contents
- [Recent Updates](#recent-updates)
- [Popular LLM Evaluation Projects on GitHub](#popular-llm-evaluation-projects-on-github)
- [Basic Model Information](#basic-model-information)
- [Leaderboards](#-leaderboards)
  - [0. Multimodal Leaderboard](#0-multimodal-leaderboard)
  - [1. Overall Capability Leaderboard](#1-overall-capability-leaderboard)
    - [1.1 Reasoning Model Leaderboard](#11-reasoning-model-leaderboard)
    - [1.2 Commercial Model Leaderboard (including paid APIs of open-source models)](#12-commercial-model-leaderboard-including-paid-apis-of-open-source-models)
    - [1.3 Open-source Model Leaderboard](#13-open-source-model-leaderboard)
  - [2. Education Leaderboard](#2-education-leaderboard)
    - [2.1 Elementary School Subjects](#21-elementary-school-subjects) &nbsp;|&nbsp; [2.2 Middle School Subjects](#22-middle-school-subjects) &nbsp;|&nbsp; [2.3 High School Entrance Exam (TODO)](#23-high-school-entrance-exam-todo)
    - [2.4 High School Subjects](#24-high-school-subjects) &nbsp;|&nbsp; [2.5 Gaokao](#25-gaokao) &nbsp;|&nbsp; [2.6 Higher Education (TODO)](#26-higher-education-todo)
    - [2.7 Graduate Entrance Exam (TODO)](#27-graduate-entrance-exam-todo) &nbsp;|&nbsp; [2.8 Teacher Certification (TODO)](#28-teacher-certification-todo)
  - [3. Medical & Mental Health Leaderboard](#3-medical--mental-health-leaderboard)
    - [3.1 Physicians](#31-physicians) &nbsp;|&nbsp; [3.2 Nursing](#32-nursing) &nbsp;|&nbsp; [3.3 Pharmacy](#33-pharmacy)
    - [3.4 Medical Technology](#34-medical-technology) &nbsp;|&nbsp; [3.5 Basic Medical Knowledge](#35-basic-medical-knowledge) &nbsp;|&nbsp; [3.6 Medical Graduate Entrance Exam](#36-medical-graduate-entrance-exam)
    - [3.7 Mental Health](#37-mental-health)
  - [4. Finance Leaderboard](#4-finance-leaderboard)
    - [4.1 Accounting](#41-accounting) &nbsp;|&nbsp; [4.2 Banking](#42-banking) &nbsp;|&nbsp; [4.3 Insurance](#43-insurance)
    - [4.4 Securities](#44-securities) &nbsp;|&nbsp; [4.5 Other Financial Qualification Exams](#45-other-financial-qualification-exams) &nbsp;|&nbsp; [4.6 Basic Financial Knowledge](#46-basic-financial-knowledge)
    - [4.7 Financial Applications](#47-financial-applications)
  - [5. Law & Public Administration Leaderboard](#5-law--public-administration-leaderboard)
    - [5.1 Bar Examination](#51-bar-examination)
    - [5.2 Civil Service Examination](#52-civil-service-examination)
  - [6. Reasoning & Math Leaderboard](#6-reasoning--math-leaderboard)
    - [6.1 Deductive Reasoning](#61-deductive-reasoning) &nbsp;|&nbsp; [6.2 Commonsense Reasoning](#62-commonsense-reasoning) &nbsp;|&nbsp; [6.3 Symbolic Reasoning (BBH)](#63-symbolic-reasoning-bbh)
    - [6.4 Arithmetic](#64-arithmetic) &nbsp;|&nbsp; [6.5 Table QA](#65-table-qa) &nbsp;|&nbsp; [6.6 Table Summarization](#66-table-summarization)
    - [6.7 High School Math Olympiad](#67-high-school-math-olympiad) &nbsp;|&nbsp; [6.8 Middle School Math Olympiad (TODO)](#68-middle-school-math-olympiad-todo) &nbsp;|&nbsp; [6.9 Elementary School Math Olympiad](#69-elementary-school-math-olympiad)
    - [6.10 Map Reasoning (TODO)](#610-map-reasoning-todo) &nbsp;|&nbsp; [6.11 Spatial Reasoning (TODO)](#611-spatial-reasoning-todo) &nbsp;|&nbsp; [6.12 Sudoku](#612-sudoku)
    - [6.13 Amount Numeric-to-Text Conversion (TODO)](#613-amount-numeric-to-text-conversion-todo) &nbsp;|&nbsp; [6.14 Date Calculation (TODO)](#614-date-calculation-todo)
  - [7. Language & Instruction Following Leaderboard](#7-language--instruction-following-leaderboard)
    - [7.1 Idiom Understanding](#71-idiom-understanding) &nbsp;|&nbsp; [7.2 Sentiment Analysis](#72-sentiment-analysis) &nbsp;|&nbsp; [7.3 Textual Entailment](#73-textual-entailment)
    - [7.4 Text Classification](#74-text-classification) &nbsp;|&nbsp; [7.5 Information Extraction](#75-information-extraction) &nbsp;|&nbsp; [7.6 Reading Comprehension](#76-reading-comprehension)
    - [7.7 Pronoun Resolution](#77-pronoun-resolution) &nbsp;|&nbsp; [7.8 Poetry Matching](#78-poetry-matching) &nbsp;|&nbsp; [7.9 Chinese Instruction Following](#79-chinese-instruction-following)
    - [7.10 Chinese Character Glyphs](#710-chinese-character-glyphs) &nbsp;|&nbsp; [7.11 Pinyin (TODO)](#711-pinyin-todo) &nbsp;|&nbsp; [7.12 Typo Detection (TODO)](#712-typo-detection-todo)
    - [7.13 Sentence Understanding (TODO)](#713-sentence-understanding-todo) &nbsp;|&nbsp; [7.14 Punctuation (TODO)](#714-punctuation-todo) &nbsp;|&nbsp; [7.15 Traditional/Simplified Conversion (TODO)](#715-traditionalsimplified-conversion-todo)
    - [7.16 Language Identification (TODO)](#716-language-identification-todo)
  - [8. Agent & Tool Use Leaderboard](#8-agent--tool-use-leaderboard)
    - [8.1 TAU](#81-tau)
    - [8.2 BFCL-V3](#82-bfcl-v3)
  - [9. Coding Leaderboard](#9-coding-leaderboard)
    - [9.1 LiveCodeBench](#91-livecodebench)
    - [9.2 Terminal-Bench-2.0](#92-terminal-bench-20)
  - [10. Combined LMArena and AA Scores](#10-combined-lmarena-and-aa-scores)
- [Capability Scores by Dimension](#-capability-scores-by-dimension)
- [Why this leaderboard?](#why-this-leaderboard)
- [Model Selection & Evaluation Community](#model-evaluation-community)
- [Cite Us](#how-to-cite-rele-cite-us)

# Recent Updates
- [2026/5/13] v5.10.5
  - New model: ernie-5.1
- [2026/5/1] v5.10.4
  - New model: qwen3.6-27b
- [2026/4/25] v5.10.3
  - New models: deepseek-v4-flash, deepseek-v4-pro, gpt-5.5
- [2026/4/23] v5.10.2
  - New models: mimo-v2.5, mimo-v2.5-pro
- [2026/4/21] v5.10.1
  - New models: qwen3.6-max-preview, kimi-k2.6
  - Updated models: refreshed kimi-k2.5 results (fixed a bug where reasoning_content was not passed in tool calls); scores and ranks changed accordingly
- [2026/4/18] v5.10
  - Coding capability is now folded into general capability and counted in the total score; rankings have shifted
  - New model: Qwen3.6-35B-A3B
  - Removed legacy models: Llama-4-Maverick-17B-128E-Instruct-FP8, DeepSeek-R1-0528-Qwen3-8B, ERNIE-4.5-0.3B,
ERNIE-4.5-21B-A3B, ERNIE-4.5-300B-A47B, Hunyuan-A13B-Instruct, Hunyuan-A13B-Instruct-nothink, step-3,
mistral-medium-2508, Mistral-Small-3.2-24B-Instruct-2506, Baichuan4-Air, gemma-3-27b-it,
gemma-3-4b-it, gemma-3-12b-it, Qwen3-1.7B, Qwen3-0.6B, Qwen3-0.6B-nothink, Qwen3-1.7B-nothink
- [2026/4/15] v5.9
  - Added the [Terminal-Bench 2.0 leaderboard](#92-terminal-bench-20) under the coding category
  - First-ever release of the [overall coding leaderboard](#9-coding-leaderboard)
  - Removed legacy models: DeepSeek-V3.2-Exp, DeepSeek-V3.2-Exp-Think, xunfei-spark-x1-0725, doubao-seed-1-6-flash-250615,
doubao-seed-1-6-flash-thinking-250615, doubao-seed-1-6-250615, grok-4-0709, GLM-4.5, GLM-4.5-nothink, GLM-4.6, MiniMax-M2,
qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, grok-3-mini, gemini-3-pro-preview
- [2026/4/8] v5.8.23
  - New model: GLM-5.1
- [2026/4/6] v5.8.22
  - New models: gemma-4-31b-it, gemma-4-26b-a4b-it
- [2026/4/3] v5.8.21
  - New model: qwen3.6-plus
- [2026/3/19] v5.8.20
  - New models: MiMo-V2-Pro, MiMo-V2-Omni
- [2026/3/18] v5.8.19
  - New models: gpt-5.4-mini, gpt-5.4-mini-high, gpt-5.4-nano, gpt-5.4-nano-high, MiniMax-M2.7
  - Removed legacy models: ERNIE-Lite-8K, MiniMax-Text-01, Doubao-1.5-lite-32k-250115, MiniMax-M1, kimi-k2-0711-preview, doubao-seed-1-6-thinking-250715
- [2026/3/17] v5.8.18
  - New model: GLM-5-Turbo
- [2026/3/5] v5.8.17
  - New models: gemini-3.1-flash-lite-preview, gpt-5.3-chat, gpt-5.4, gpt-5.4-high
- [2026/2/25] v5.8.16
  - New models: qwen3.5-flash, Qwen3.5-27B, Qwen3.5-122B-A10B
  - Removed legacy models: qwen-long-2025-01-25, 360zhinao2-o1, Magistral-Small-2507
- [2026/2/20] v5.8.15
  - New models: qwen3.5-plus, gemini-3.1-pro-preview
- [2026/2/14] v5.8.14
  - New models: Doubao-Seed-2.0-pro, Doubao-Seed-2.0-lite, Doubao-Seed-2.0-mini
- [2026/2/9] v5.8.13
  - New models: claude-opus-4.6, GLM-5, MiniMax-M2.5, LongCat-Flash-Lite, MiMo-V2-Flash-0204, MiMo-V2-Flash-think-0204
- [2026/2/2] v5.8.12
  - New model: step-3.5-flash
- [2026/1/27] v5.8.11
  - New models: qwen3-max-2026-01-23, qwen3-max-think-2026-01-23 (qwen3-max-2026-01-23 with thinking mode enabled), Kimi-K2.5-Thinking
- [2026/1/22] v5.8.10
  - New models: GLM-4.7-Flash, LongCat-Flash-Thinking-2601, ERNIE-5.0
- [2025/12/24] v5.8.9, [2025/12/23] v5.8.8, [2025/12/18] v5.8.7, [2025/12/13] v5.8.6, [2025/12/6] v5.8.5, [2025/12/3] v5.8.4, [2025/11/3] v5.8, [2025/10/24] v5.7, [2025/10/13] v5.6, [2025/9/30] v5.5, [2025/9/22] v5.4, [2025/9/14] v5.3, [2025/9/10] v5.2, [2025/9/6] v5.1, [2025/9/1] v5.0, [2025/8/26] v4.13, [2025/8/20] v4.12, [2025/8/15] v4.11, [2025/8/10] v4.10, [2025/8/7] v4.9, [2025/8/1] v4.8, [2025/7/29] v4.7, [2025/7/26] v4.6, [2025/7/23] v4.5, [2025/7/17] v4.4, [2025/7/13] v4.3, [2025/7/12] v4.2, [2025/7/9] v4.1, [2025/7/2] v4.0, [2025/6/23] v3.33, [2025/6/18] v3.32, [2025/6/16] v3.31, [2025/6/13] v3.30, [2025/6/9] v3.29, [2025/6/4] v3.28, [2025/5/29] v3.27, [2025/5/23] v3.26, [2025/5/18] v3.25, [2025/5/15] v3.24, [2025/5/10] v3.23, [2025/5/5] v3.22, [2025/5/2] v3.21, [2025/4/30] v3.20, [2025/4/28] v3.19, [2025/4/22] v3.18, [2025/4/17] v3.17, [2025/4/9] v3.16, [2025/4/5] v3.15, [2025/4/3] v3.14, [2025/3/31] v3.13, [2025/3/29] v3.12, [2025/3/27] v3.11, [2025/3/25] v3.10, [2025/3/23] v3.9, [2025/3/21] v3.8, [2025/3/19] v3.7, [2025/3/17] v3.6, [2025/3/15] v3.5, [2025/3/13] v3.4, [2025/3/11] v3.3, [2025/3/10] v3.2, [2025/3/7] v3.1, [2025/3/4] v3.0, [2025/3/3] v2.22, [2025/2/28] v2.21, [2025/2/24] v2.20, [2025/2/22] v2.19, [2025/2/18] v2.18, [2025/2/14] v2.17, [2025/2/13] v2.16, [2025/2/12] v2.15, [2025/2/10] v2.14, [2025/1/29] v2.13, [2025/1/25] v2.12, [2025/1/23] v2.11, [2025/1/22] v2.10, [2025/1/20] v2.9, [2025/1/17] v2.8, [2025/1/7] v2.7
- 2024: [2024/12/28] v2.6, [2024/12/27] v2.5, [2024/12/25] v2.4, [2024/10/20] v2.3, [2024/9/29] v2.2, [2024/8/27] v2.1, [2024/8/7] v2.0, [2024/7/26] v1.21, [2024/7/15] v1.20, [2024/6/29] v1.19, [2024/6/2] v1.18, [2024/5/8] v1.17, [2024/4/13] v1.16, [2024/3/20] v1.15, [2024/2/28] v1.14, [2024/1/29] v1.13
- 2023: [2023/12/10] v1.12, [2023/11/22] v1.11, [2023/11/5] v1.10, [2023/10/11] v1.9, [2023/9/13] v1.8, [2023/8/29] v1.7, [2023/8/13] v1.6, [2023/7/26] v1.5, [2023/7/18] v1.4, [2023/7/2] v1.3, [2023/6/17] v1.2, [2023/6/10] v1.1, [2023/6/4] v1

Full update history: [CHANGELOG](CHANGELOG-EN.md)
<br><br>


# Popular LLM Evaluation Projects on GitHub
| repo                                                                               | star  | area   | about                                                                                                                                                                                                                                                                   |
|------------------------------------------------------------------------------------|-------|--------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [langfuse](https://github.com/langfuse/langfuse)                                   | 23.6k | Overseas | Open source LLM engineering platform: LLM Observability, metrics, evals, prompt management, playground, datasets. Integrates with OpenTelemetry, Langchain, OpenAI SDK, LiteLLM, and more. YC W23                                                                       |
| [opik](https://github.com/comet-ml/opik)                                           | 18.4k | Overseas | Debug, evaluate, and monitor your LLM applications, RAG systems, and agentic workflows with comprehensive tracing, automated evaluations, and production-ready dashboards.                                                                                              |
| [deepeval](https://github.com/confident-ai/deepeval)                               | 14.2k | Overseas | The LLM Evaluation Framework                                                                                                                                                                                                                                            |
| ……                                                                                 | ……    | ……     | ……                                                                                                                                                                                                                                                                      |
| [chinese-llm-benchmark (ours)](https://github.com/jeinlee1991/chinese-llm-benchmark) | 5.7k  | **China** | ReLE Chinese LLM Capability Benchmark (continuously updated) |
| ……                                                                                 | ……    | ……     | ……                                                                                                                                                                                                                                                                      |

See [hot50](GitHub热门评测repo-EN.md) for the full list.
<br><br>


# Basic Model Information
- [Newest models each week](每周最新模型-EN.md)
    - [May 4–May 10](每周最新模型-EN.md)
    - [Apr 27–May 3](每周最新模型-EN.md)
    - [Apr 20–Apr 26](每周最新模型-EN.md)
    - [Apr 13–Apr 19](每周最新模型-EN.md)
- For more, see the [model list](https://nonelinear.com/static/models.html)
<br><br>

# Unified LLM Gateway
Introducing the one-stop AI Model Marketplace, offering the most comprehensive lineup of LLMs available so you always stay one step ahead.
- Global models, all in one place: GPT-5.5, Gemini-3.1-Pro, Claude-4.7, DeepSeek-v4, Kimi-k2.5 ……
- Smart load balancing and high concurrency: we aggregate multiple top-tier providers and use intelligent routing for automatic load balancing. Say goodbye to annoying rate-limit errors and handle traffic spikes with ease.
- Automatic failover: if a single provider's API has a hiccup, our system seamlessly switches to a healthy backup channel in milliseconds, ensuring 99.9999% availability and sparing your users any "service unavailable" embarrassment.
- Online monitoring and intelligent model selection: integrated with online performance monitoring tools to close the loop between model selection and evaluation. Let real data guide you to the best-performing, most cost-effective model.
[How to integrate online performance monitoring](https://nonelinear.com/static/online-eval.html), [How to integrate model-selection evaluation](https://nonelinear.com/static/task-create.html)
- Excellent value! [See all models and prices](https://nonelinear.com/static/models.html)
```
from openai import OpenAI
base_url = "https://api.nonelinear.com/v1"
api_key = "<your api key>" # Get one at https://nonelinear.com/static/apikey.html
client = OpenAI(api_key=api_key, base_url=base_url)
client.chat.completions.create(
    model="<model id>", # Model list: https://nonelinear.com/static/models.html
    messages=[{"role": "user", "content": "<your prompt>"}],
)
```
<br><br>


# Model Selection: Target 90% Cost Reduction
Say no to "blind picking" of LLMs! Upload your own test data, and in 5 minutes you'll know which model performs best and is most cost-effective for your scenario. Pick the right model and cut costs by up to 90%! [Try it now >>](https://nonelinear.com/static/task-create.html)
![link](docs/modelSelection/img/task-result-html.png)
<video controls src="docs/modelSelection/img/modelsel.mp4"></video>

Examples:
- [Table summarization for WeChat article writing](docs/modelSelection/微信文章撰写之表格总结-EN.md)
- [Converting MathML to LaTeX format](docs/modelSelection/MathML转LaTeX格式-EN.md)
<br><br>


# Leaderboards
## 0. Multimodal Leaderboard
See [Multimodal Evaluation](README-多模态评测-EN.md) for details.<br>
<br><br>


## 1. Overall Capability Leaderboard
"Overall capability" scoring: "Overall capability" is the weighted sum of "Professional capability" and "General capability", with weights of 0.3 and 0.7 respectively. "Professional capability" is the average of 4 domains — Education, Medical & Mental Health, Finance, and Law & Public Administration — while "General capability" is the average of 4 domains — Reasoning & Math, Language & Instruction Following, Agent & Tool Use, and Coding.
![link](pic/总分.png)

|Category|Organization|Model|[Total Score] Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|Alibaba|qwen3.6-max-preview(new)|75.4%|80s|2789|139.2|1|
|Commercial|OpenAI|gpt-5.5(new)|75.3%|15s|955|158.5|2|


Full data: [Overall Capability Leaderboard](leaderboard/总分-EN.md) | [General Capability Leaderboard](leaderboard/通用能力-EN.md) | [Professional Capability Leaderboard](leaderboard/专业能力-EN.md)
<br><br>

#### 1.1 Reasoning Model Leaderboard
See [Reasoning Model Leaderboard](leaderboard/reasonmodel-EN.md).<br>
<br>
#### 1.2 Commercial Model Leaderboard (including paid APIs of open-source models)
[Commercial models with Output Price >= ¥5](leaderboard/commerce1-EN.md) | [Commercial models with Output Price ¥1–5](leaderboard/commerce2-EN.md) | [Commercial models with Output Price < ¥1](leaderboard/commerce3-EN.md)<br>
DIY custom-dimension leaderboard: [link](https://nonelinear.com/static/benchmarking.html)
<br>
<br>
#### 1.3 Open-source Model Leaderboard
[Open-source models < 5B](leaderboard/opensource1-EN.md) | [Open-source models 5B–20B](leaderboard/opensource2-EN.md) | [Open-source models > 20B](leaderboard/opensource3-EN.md)<br>
DIY custom-dimension leaderboard: [link](https://nonelinear.com/static/benchmarking.html)

<br><br>



## 2. Education Leaderboard
Full leaderboard: [Education](leaderboard/教育-EN.md)<br>

### 2.1 Elementary School Subjects
Full leaderboard: [Elementary School Subjects](leaderboard/小学学科-EN.md).<br>
Chinese: [Leaderboard](leaderboard/PrimarySchoolChinese-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=PrimarySchoolChinese),
English: [Leaderboard](leaderboard/PrimarySchoolEnglish-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=PrimarySchoolEnglish),
Math: [Leaderboard](leaderboard/PrimarySchoolMathematics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=PrimarySchoolMathematics),
Ethics & Rule of Law: [Leaderboard](leaderboard/PrimarySchoolEthics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=PrimarySchoolEthics),
Science: [Leaderboard](leaderboard/PrimarySchoolScience-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=PrimarySchoolScience)
<br><br>


### 2.2 Middle School Subjects
Full leaderboard: [Middle School Subjects](leaderboard/初中学科-EN.md).<br>
Biology: [Leaderboard](leaderboard/MiddleSchoolBiology-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=MiddleSchoolBiology),
Chemistry: [Leaderboard](leaderboard/MiddleSchoolChemistry-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=MiddleSchoolChemistry),
Chinese: [Leaderboard](leaderboard/MiddleSchoolChinese-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=MiddleSchoolChinese),
English: [Leaderboard](leaderboard/MiddleSchoolEnglish-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=MiddleSchoolEnglish),
Geography: [Leaderboard](leaderboard/MiddleSchoolGeography-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=MiddleSchoolGeography),
History: [Leaderboard](leaderboard/MiddleSchoolHistory-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=MiddleSchoolHistory),
Math: [Leaderboard](leaderboard/MiddleSchoolMathematics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=MiddleSchoolMathematics),
Physics: [Leaderboard](leaderboard/MiddleSchoolPhysics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=MiddleSchoolPhysics),
Politics: [Leaderboard](leaderboard/MiddleSchoolPolitics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=MiddleSchoolPolitics)
<br><br>


### 2.3 High School Entrance Exam (TODO)

### 2.4 High School Subjects
Full leaderboard: [High School Subjects](leaderboard/高中学科-EN.md).<br>
Biology: [Leaderboard](leaderboard/HighSchoolBiology-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=HighSchoolBiology),
Chemistry: [Leaderboard](leaderboard/HighSchoolChemistry-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=HighSchoolChemistry),
Chinese: [Leaderboard](leaderboard/HighSchoolChinese-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=HighSchoolChinese),
English: [Leaderboard](leaderboard/HighSchoolEnglish-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=HighSchoolEnglish),
Geography: [Leaderboard](leaderboard/HighSchoolGeography-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=HighSchoolGeography),
History: [Leaderboard](leaderboard/HighSchoolHistory-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=HighSchoolHistory),
Math: [Leaderboard](leaderboard/HighSchoolMathematics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=HighSchoolMathematics),
Physics: [Leaderboard](leaderboard/HighSchoolPhysics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=HighSchoolPhysics),
Politics: [Leaderboard](leaderboard/HighSchoolPolitics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=HighSchoolPolitics)
<br><br>


### 2.5 Gaokao
Real past Gaokao (Chinese college entrance exam) questions, including short-answer, fill-in-the-blank, multiple-choice, etc., keeping only objective questions. All scores are accuracy; 100% means all questions answered correctly. For example, a math score of 100 means every question was answered correctly. Full leaderboard: [Gaokao](leaderboard/高考-EN.md).<br>
(1) 2025 Gaokao<br>
Biology: [Leaderboard](leaderboard/2025高考生物-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=2025高考生物),
Chemistry: [Leaderboard](leaderboard/2025高考化学-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=2025高考化学),
Chinese: [Leaderboard](leaderboard/2025高考语文-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=2025高考语文),
English: [Leaderboard](leaderboard/2025高考英语-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=2025高考英语),
Geography: [Leaderboard](leaderboard/2025高考地理-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=2025高考地理),
History: [Leaderboard](leaderboard/2025高考历史-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=2025高考历史),
Math: [Leaderboard](leaderboard/2025高考数学-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=2025高考数学),
Physics: [Leaderboard](leaderboard/2025高考物理-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=2025高考物理),
Politics: [Leaderboard](leaderboard/2025高考政治-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=2025高考政治).

(2) Gaokao 2024 and earlier<br>
Biology: [Leaderboard](leaderboard/gaokao-biology-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=gaokao-biology),
Chemistry: [Leaderboard](leaderboard/gaokao-chemistry-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=gaokao-chemistry),
Chinese: [Leaderboard](leaderboard/gaokao-chinese-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=gaokao-chinese),
Geography: [Leaderboard](leaderboard/gaokao-geography-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=gaokao-geography),
History: [Leaderboard](leaderboard/gaokao-history-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=gaokao-history),
Math: [Leaderboard](leaderboard/gaokao-math-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=gaokao-math),
Physics: [Leaderboard](leaderboard/gaokao-physics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=gaokao-physics),
Politics: [Leaderboard](leaderboard/gaokao-politics-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=gaokao-politics).
<br><br>


### 2.6 Higher Education (TODO)
### 2.7 Graduate Entrance Exam (TODO)
### 2.8 Teacher Certification (TODO)
<br><br><br>



## 3. Medical & Mental Health Leaderboard
Full leaderboard: [Medical & Mental Health](leaderboard/医疗与心理健康-EN.md)<br>

### 3.1 Physicians
Full leaderboard: [Physicians](leaderboard/医师-EN.md)<br>
(1) Internal Medicine, [Leaderboard](leaderboard/内科-EN.md)<br>
Internal Medicine Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-内科),
TCM Internal Medicine Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医内科主治医师),
Internal Medicine Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=内科主治医师),
Cardiology & Pulmonology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=心血管内科与呼吸内科主治医师),
Nephrology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=肾内科主治医师),
Gastroenterology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=消化内科主治医师),
Integrated TCM-Western Internal Medicine Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中西医结合内科主治医师),
Gastroenterology Senior Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=消化内科高级职称),
General Internal Medicine Senior Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=普通内科高级职称),
Pulmonology Senior Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=呼吸内科高级职称),
Cardiology Senior Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=心内科高级职称),
Tuberculosis Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=结核病主治医师),
Endocrinology Senior Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=内分泌科高级职称)
<br>

(2) Surgery, [Leaderboard](leaderboard/外科-EN.md)<br>
Surgery Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-外科),
Oral & Maxillofacial Surgery Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=口腔颌面外科主治医师),
Plastic Surgery Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=整形外科主治医师),
Surgery Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=外科主治医师),
General Surgery Senior Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=普通外科高级职称),
Orthopedics Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-骨科),
Orthopedics Intermediate Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=骨科中级职称),
Orthopedics Senior Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=骨科高级职称)
<br>

(3) Obstetrics & Gynecology, [Leaderboard](leaderboard/妇产科-EN.md)<br>
Obstetrics & Gynecology Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-妇产科),
Obstetrics & Gynecology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=妇产科主治医师),
Obstetrics & Gynecology Deputy Chief / Chief Physician Title Exam: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=妇产科学副主任、主任医师职称考试)
<br>

(4) Pediatrics, [Leaderboard](leaderboard/儿科-EN.md)<br>
Pediatrics Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-儿科),
Pediatrics Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=儿科主治医师),
Pediatric Surgery Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-小儿外科)
<br>

(5) Ophthalmology, [Leaderboard](leaderboard/眼科-EN.md)<br>
Ophthalmology Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-眼科),
Ophthalmology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=眼科主治医师)
<br>

(6) Dentistry, [Leaderboard](leaderboard/口腔科-EN.md)<br>
Dentistry Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-口腔科),
Dental Assistant Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=口腔执业助理医师),
Dental Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=口腔执业医师),
Operative Dentistry Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=口腔内科主治医师),
Dental Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=口腔科主治医师),
Prosthodontics Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=口腔修复科主治医师),
Orthodontics Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=口腔正畸学主治医师)
<br>

(7) Otorhinolaryngology, [Leaderboard](leaderboard/耳鼻咽喉科-EN.md)<br>
ENT Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-耳鼻咽喉科),
ENT Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=耳鼻咽喉科主治医师)
<br>

(8) Neurology & Psychiatry, [Leaderboard](leaderboard/脑系科-EN.md)<br>
Neurology Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-神经内科),
Neurology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=神经内科主治医师),
Psychiatry Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-精神科),
Psychiatry Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=精神病学主治医师),
Psychotherapy Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=心理治疗学主治医师考试),
Psychological Counselor: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=心理咨询师考试)
<br>

(9) Dermatology, [Leaderboard](leaderboard/皮肤科-EN.md)<br>
Dermatology Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-皮肤科),
Dermatology Intermediate Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=皮肤科中级职称),
Dermatology & Venereology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=皮肤与性病学主治医师)
<br>

(10) Traditional Chinese Medicine and TCM-Western Integration, [Leaderboard](leaderboard/中医与中西医结合-EN.md)<br>
Integrated TCM-Western Assistant Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中西医结合执业助理医师),
TCM Assistant Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医执业助理医师),
Integrated TCM-Western Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中西医结合执业医师),
TCM Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医执业医师),
TCM Acupuncture Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医针灸主治医师)
<br>

(11) Rehabilitation Medicine, [Leaderboard](leaderboard/康复医学科-EN.md)<br>
Rehabilitation Medicine Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-康复医学科),
Rehabilitation Medicine Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=康复医学主治医师)
<br>

(12) General Practice, [Leaderboard](leaderboard/全科医学科-EN.md)<br>
General Practice Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-全科医学科),
General Practice Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=全科主治医师)
<br>

(13) Clinical Nutrition and Critical Care Medicine, [Leaderboard](leaderboard/临床营养与重症医学-EN.md)<br>
Clinical Assistant Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床执业助理医师),
Clinical Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床执业医师),
Rheumatology & Clinical Immunology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=风湿与临床免疫主治医师),
Critical Care Medicine Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=重症医学主治医师),
Nutrition Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=营养学主治医师),
Clinical Pathology Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-临床病理科)
<br>

(14) Oncology, [Leaderboard](leaderboard/肿瘤科-EN.md)<br>
Oncology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=肿瘤学主治医师)
<br>

(15) Anesthesiology and Pain Management, [Leaderboard](leaderboard/麻醉疼痛科-EN.md)<br>
Anesthesiology Residency Completion: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-麻醉科),
Anesthesiology Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=麻醉科主治医师),
Pain Management Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=疼痛科主治医师)
<br>

(16) Public Health and Occupational Diseases, [Leaderboard](leaderboard/公共卫生与职业病-EN.md)<br>
Public Health Assistant Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=公共卫生执业助理医师),
Public Health Practitioner: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=公共卫生执业医师),
Hospital Infection Intermediate Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=医院感染中级职称),
Infectious Diseases Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=传染病主治医师),
Preventive Medicine Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=预防医学主治医师),
Infectious Diseases Intermediate Title: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=传染病学中级职称),
Occupational Diseases Attending Physician: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=职业病主治医师)
<br><br>


### 3.2 Nursing
Full leaderboard: [Nursing](leaderboard/护理-EN.md)<br>
Nurse Practitioner Qualification Exam: [Leaderboard](leaderboard/护士执业资格考试-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=护士执业资格考试),
Nurse Qualification Exam: [Leaderboard](leaderboard/护师资格考试-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=护师资格考试),
Pediatric Charge Nurse: [Leaderboard](leaderboard/儿科主管护师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=儿科主管护师),
Internal Medicine Nursing: [Leaderboard](leaderboard/主管护师-内科护理学-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=主管护师-内科护理学),
Obstetrics & Gynecology Nursing: [Leaderboard](leaderboard/主管护师-妇产科护理学-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=主管护师-妇产科护理学),
Obstetrics & Gynecology Charge Nurse: [Leaderboard](leaderboard/妇产科主管护师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=妇产科主管护师),
Surgical Charge Nurse: [Leaderboard](leaderboard/外科主管护师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=外科主管护师),
Charge Nurse Qualification Exam: [Leaderboard](leaderboard/主管护师资格考试-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=主管护师资格考试),
Internal Medicine Charge Nurse: [Leaderboard](leaderboard/内科主管护师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=内科主管护师),
Deputy / Chief Nurse Qualification Exam: [Leaderboard](leaderboard/高级护师-副主任、主任护师资格考试-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=高级护师-副主任、主任护师资格考试)
<br><br>


### 3.3 Pharmacy
Full leaderboard: [Pharmacy](leaderboard/药师-EN.md)<br>
Licensed Western Pharmacist: [Leaderboard](leaderboard/执业西药师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=执业西药师),
Licensed TCM Pharmacist: [Leaderboard](leaderboard/执业中药师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=执业中药师),
Junior Pharmacy Technician Exam: [Leaderboard](leaderboard/药士初级考试-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=药士初级考试),
Junior Pharmacist Exam: [Leaderboard](leaderboard/药师初级考试-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=药师初级考试),
TCM Pharmacy (Technician): [Leaderboard](leaderboard/初级中药士-中药学（士）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=初级中药士-中药学（士）),
TCM Pharmacy (Pharmacist): [Leaderboard](leaderboard/初级中药师-中药学（师）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=初级中药师-中药学（师）),
Charge Pharmacist Qualification Exam: [Leaderboard](leaderboard/主管药师资格考试-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=主管药师资格考试),
Charge TCM Pharmacist: [Leaderboard](leaderboard/主管中药师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=主管中药师)
<br><br>


### 3.4 Medical Technology
Full leaderboard: [Medical Technology](leaderboard/医技-EN.md)<br>
Ultrasound: [Leaderboard](leaderboard/规培结业-超声科-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-超声科),
Ultrasound Attending Physician: [Leaderboard](leaderboard/超声波医学主治医师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=超声波医学主治医师),
Ultrasound Charge Technician: [Leaderboard](leaderboard/超声波医学主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=超声波医学主管技师),
Electrocardiography Charge Technician: [Leaderboard](leaderboard/心电学主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=心电学主管技师),
Medical Imaging Residency Completion: [Leaderboard](leaderboard/规培结业-医学影像科-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=规培结业-医学影像科),
Nuclear Medicine Attending Physician: [Leaderboard](leaderboard/核医学主治医师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=核医学主治医师),
Nuclear Medicine Charge Technician: [Leaderboard](leaderboard/核医学主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=核医学主管技师),
Radiology Attending Physician: [Leaderboard](leaderboard/放射科主治医师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=放射科主治医师),
Radiology Technology (Technician): [Leaderboard](leaderboard/放射学技术（士）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=放射学技术（士）),
Radiology Technology (Senior Technician): [Leaderboard](leaderboard/放射学技术（师）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=放射学技术（师）),
Radiation Medicine Charge Technician: [Leaderboard](leaderboard/放射医学主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=放射医学主管技师),
Laboratory Technology (Technician): [Leaderboard](leaderboard/检验技术（士）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=检验技术（士）),
Laboratory Technology (Senior Technician): [Leaderboard](leaderboard/检验技术（师）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=检验技术（师）),
Microbiology Lab Charge Technician: [Leaderboard](leaderboard/微生物检验主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=微生物检验主管技师),
Physical & Chemical Lab Charge Technician: [Leaderboard](leaderboard/理化检验主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=理化检验主管技师),
Clinical Lab Charge Technician: [Leaderboard](leaderboard/临床医学检验主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学检验主管技师),
Pathology Attending Physician: [Leaderboard](leaderboard/病理科主治医师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=病理科主治医师),
Pathology Charge Technician: [Leaderboard](leaderboard/病理学主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=病理学主管技师),
Pathology Technology: [Leaderboard](leaderboard/主管技师-病理学技术-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=主管技师-病理学技术),
Rehabilitation Medicine Technology (Technician): [Leaderboard](leaderboard/康复医学治疗技术（士）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=康复医学治疗技术（士）),
Rehabilitation Medicine Technology (Senior Technician): [Leaderboard](leaderboard/康复医学治疗技术（师）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=康复医学治疗技术（师）),
Rehabilitation Medicine & Therapy Charge Technician: [Leaderboard](leaderboard/康复医学与治疗主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=康复医学与治疗主管技师),
Oncology Technology (Technician): [Leaderboard](leaderboard/肿瘤学技术（士）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=肿瘤学技术（士）),
Oncology Technology (Senior Technician): [Leaderboard](leaderboard/肿瘤学技术（师）-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=肿瘤学技术（师）),
Radiation Oncology Charge Technician: [Leaderboard](leaderboard/肿瘤放射治疗主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=肿瘤放射治疗主管技师),
Transfusion Technology Charge Technician: [Leaderboard](leaderboard/输血技术主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=输血技术主管技师),
Sterilization Technology Charge Technician: [Leaderboard](leaderboard/消毒技术主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=消毒技术主管技师),
Medical Records Information Charge Technician: [Leaderboard](leaderboard/病案信息主管技师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=病案信息主管技师)
<br><br>


### 3.5 Basic Medical Knowledge
(1) Basic Medicine, [Leaderboard](leaderboard/基础医学-EN.md)<br>
Medical Three Basics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=医学三基),
Medical Psychology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-医学心理学),
Biochemistry & Molecular Biology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=生物化学与分子生物学),
Cell Biology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-细胞生物学),
Medical Immunology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-医学免疫学),
Immunology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-免疫学),
Pathophysiology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-病理生理学),
Pathology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-病理学),
Medical Genetics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-医学遗传学),
Parasitology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-寄生虫学),
Human Parasitology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-人体寄生虫学),
Systematic Anatomy: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-系统解剖学),
Anatomy: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-解剖学),
Regional Anatomy: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-局部解剖学),
Bioinformatics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-生物信息学),
Physiology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-生理学),
Pharmacology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-药理学),
Pharmaceutical Analysis: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-药物分析学),
Medical Microbiology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-医学微生物学),
Histology & Embryology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-组织学与胚胎学),
Medical Statistics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-医学统计学)
<br>

(2) Clinical Medicine, [Leaderboard](leaderboard/临床医学-EN.md)<br>
Clinical Medicine: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学综合),
Medical Imaging: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-医学影像学),
Radiology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-放射学),
Laboratory Diagnostics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-实验诊断学),
Neurology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-神经病学),
Surgery: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-外科学),
Dermatology & Venereology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-皮肤性病学),
Pediatrics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-儿科学),
Nuclear Medicine: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-核医学),
Physical Diagnostics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-物理诊断学),
Endodontics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-牙体牙髓病学),
Fundamentals of Nursing: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-护理学基础),
Nursing: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-护理学基础),
Basic Nursing: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-基础护理学),
Diagnostics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-诊断学),
Ultrasound Medicine: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-超声医学),
Dental Nursing: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-口腔护理学),
Evidence-Based Medicine: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-循证医学),
Epidemiology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-流行病学),
Oral Histopathology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-口腔组织病理学),
Infectious Diseases: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-传染病学),
Oral Anatomy & Physiology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-口腔解剖生理学),
Anesthesiology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-麻醉学),
Interventional Radiology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=临床医学-介入放射学)
<br>

(3) Preventive Medicine and Public Health, [Leaderboard](leaderboard/预防医学与公共卫生学-EN.md)<br>
Preventive Medicine: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=预防医学),
Hygiene: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=卫生学),
Medical Ethics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=医学伦理学)
<br>

(4) TCM and Chinese Materia Medica, [Leaderboard](leaderboard/中医学与中药学-EN.md)<br>
TCM Ophthalmology: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医眼科学),
Synopsis of Golden Chamber: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金匮要略讲义),
Foundations of TCM Theory: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医基础理论),
TCM Diagnostics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医诊断学),
TCM: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医学),
Warm Diseases: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=温病学),
History of Chinese Medicine: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中国医学史),
TCM Internal Medicine: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医内科学),
TCM Pediatrics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中医儿科学),
Treatise on Cold Damage: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=伤寒论),
Inner Canon Lectures: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=内经讲义)
<br><br>


### 3.6 Medical Graduate Entrance Exam
Medical graduate entrance exam covering 5 directions, including Surgical Nursing, Fundamentals of Nursing, Western Medicine Comprehensive, etc. See [CMB](https://github.com/FreedomIntelligence/CMB) for reference. Full leaderboard: [Medical Graduate Entrance Exam](leaderboard/医学考研-EN.md).<br>
(1) Surgical Nursing: [Leaderboard](leaderboard/医学考研-外科护理学-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=医学考研-外科护理学),
(2) Fundamentals of Nursing: [Leaderboard](leaderboard/医学考研-基础护理学-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=医学考研-基础护理学),
(3) Graduate Entrance Exam Politics: [Leaderboard](leaderboard/考研政治-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=考研政治),
(4) Western Medicine Comprehensive: [Leaderboard](leaderboard/医学考研-西医综合-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=医学考研-西医综合),
(5) TCM Comprehensive: [Leaderboard](leaderboard/医学考研-中医综合-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=医学考研-中医综合)
<br><br>


### 3.7 Mental Health
Currently includes 4 subcategories: Psychology Comprehensive, Psychotherapy Attending Physician, Psychological Counselor, and Medical Psychology. Full leaderboard: [Mental Health](leaderboard/心理健康-EN.md).<br>
(1) Psychology Comprehensive: [Leaderboard](leaderboard/心理综合-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=心理综合),
(2) Psychotherapy Attending Physician: [Leaderboard](leaderboard/心理治疗学主治医师考试.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=心理治疗学主治医师考试),
(3) Psychological Counselor: [Leaderboard](leaderboard/心理咨询师考试.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=心理咨询师考试),
(4) Medical Psychology: [Leaderboard](leaderboard/基础医学-医学心理学.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基础医学-医学心理学)
<br><br><br>



## 4. Finance Leaderboard
Full leaderboard: [Finance](leaderboard/金融-EN.md)<br>

### 4.1 Accounting
Full leaderboard: [Accounting](leaderboard/财务-EN.md).<br>
Junior Accounting Title: [Leaderboard](leaderboard/初级会计职称-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=初级会计职称),
Certified Public Accountant (CPA): [Leaderboard](leaderboard/注册会计师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=注册会计师),
Accounting Qualification: [Leaderboard](leaderboard/会计从业资格.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=会计从业资格),
Auditor Exam: [Leaderboard](leaderboard/审计师考试.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=审计师考试),
Certified Tax Agent: [Leaderboard](leaderboard/注册税务师.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=注册税务师),
Certified Management Accountant: [Leaderboard](leaderboard/注册管理会计师.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=注册管理会计师)

### 4.2 Banking
Full leaderboard: [Banking](leaderboard/银行-EN.md).<br>
Junior Banking Qualification: [Leaderboard](leaderboard/银行初级资格-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=银行初级资格),
Intermediate Banking Qualification: [Leaderboard](leaderboard/银从中级资格-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=银从中级资格),
Banking Qualification: [Leaderboard](leaderboard/银行从业资格.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=银行从业资格)

### 4.3 Insurance
Full leaderboard: [Insurance](leaderboard/保险-EN.md).<br>
Insurance Qualification: [Leaderboard](leaderboard/保险从业资格-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=保险从业资格)

### 4.4 Securities
Full leaderboard: [Securities](leaderboard/证券-EN.md).<br>
Securities Specialist Exam: [Leaderboard](leaderboard/证券专项考试-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=证券专项考试),
Securities Qualification: [Leaderboard](leaderboard/证券从业资格-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=证券从业资格)

### 4.5 Other Financial Qualification Exams
Full leaderboard: [Other Financial Qualification Exams](leaderboard/其他金融资格考试-EN.md).<br>
Junior Economist: [Leaderboard](leaderboard/初级经济师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=初级经济师),
Intermediate Economist: [Leaderboard](leaderboard/中级经济师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中级经济师),
Anti-Counterfeit Currency Knowledge: [Leaderboard](leaderboard/反假货币知识-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=反假货币知识),
Futures Qualification: [Leaderboard](leaderboard/期货从业资格-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=期货从业资格),
Associate Financial Planner (AFP): [Leaderboard](leaderboard/金融理财师AFP-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融理财师AFP),
Fund Qualification: [Leaderboard](leaderboard/基金从业资格-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=基金从业资格),
Gold Qualification: [Leaderboard](leaderboard/黄金从业资格-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=黄金从业资格),
China Actuary: [Leaderboard](leaderboard/中国精算师-EN.md) | [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中国精算师)

### 4.6 Basic Financial Knowledge
Full leaderboard: [Basic Financial Knowledge](leaderboard/金融基础知识-EN.md).<br>
Finance: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融学),
Corporate Strategy & Risk Management: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=公司战略与风险管理),
Macroeconomics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=宏观经济学),
Financial Markets: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融市场学),
Accounting: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=会计学),
Cost Accounting: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=成本会计学),
Monetary & Financial Economics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=货币金融学),
Political Economy: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=政治经济学),
Investments: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=投资学),
Econometrics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=计量经济学),
Corporate Finance: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=公司金融学),
Public Finance: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=财政学),
Commercial Banking Finance: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=商业银行金融学),
Management Accounting: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=管理会计学),
Central Banking: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中央银行学),
Auditing: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=审计学),
International Economics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=国际经济学),
Intermediate Financial Accounting: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中级财务会计),
Financial Management: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=财务管理学),
Microeconomics: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=微观经济学),
International Finance: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=国际金融学),
Financial Engineering: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融工程学),
Economic Law: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=经济法),
Advanced Financial Accounting: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=高级财务会计),
Insurance: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=保险学)

### 4.7 Financial Applications
Full leaderboard: [Financial Applications](leaderboard/金融应用-EN.md).<br>
Insurance Knowledge Interpretation: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=保险知识解读),
Financial Terminology Explanation: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融术语解释),
Practicing Physician Qualification Exam: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融知识-执业医师资格考试),
Financial Planning Knowledge Interpretation: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=理财知识解读),
Licensed Pharmacist Qualification Exam: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融知识-执业药师资格考试),
Financial Document Extraction: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融文档抽取),
Analyst View Extraction: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融认知-研判观点提取),
Financial Sentiment Recognition: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融情绪识别),
Insurance Slot Recognition: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=保险槽位识别),
Insurance Intent Understanding: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=保险意图理解),
Financial Intent Understanding: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融意图理解),
Insurance Attribute Extraction: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=保险属性抽取),
Insurance Clause Interpretation: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=保险条款解读),
Financial Product Analysis: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融产品分析),
Financial Numerical Computation: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融数值计算),
Financial Event Interpretation: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融事件解读),
Content Generation – Investor Education Script: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融投教话术生成),
Content Generation – Text Summarization: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融文本总结归纳),
Content Generation – Marketing Copy: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融营销文案生成),
Content Generation – News Headline: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融资讯标题生成),
Safety & Compliance – Financial Compliance: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融合规性),
Safety & Compliance – Financial Issue Detection: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融问题识别),
Safety & Compliance – Information Security Compliance: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融信息安全合规),
Safety & Compliance – Financial Factuality: [badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=金融事实性)
<br><br><br>


## 5. Law & Public Administration Leaderboard
Full leaderboard: [Law & Public Administration](leaderboard/法律与行政公务-EN.md)<br>

### 5.1 Bar Examination
#### (1) JEC-QA-KD
Multiple-choice questions, 1000 in total. See [AGIEval](https://github.com/ruixiangcui/AGIEval).<br>
Full leaderboard: [JEC-QA-KD](leaderboard/JEC-QA-KD-EN.md). See [JEC-QA-KD: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=JEC-QA-KD)
<br>

#### (2) JEC-QA-CA
Multiple-choice questions, 1000 in total. See [AGIEval](https://github.com/ruixiangcui/AGIEval).<br>
Full leaderboard: [JEC-QA-CA](leaderboard/JEC-QA-CA-EN.md). See [JEC-QA-CA: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=JEC-QA-CA)
<br>

#### (3) Comprehensive Law
Full leaderboard: [Comprehensive Law](leaderboard/法律综合-EN.md). See [Comprehensive Law: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=法律综合)
<br><br><br>


### 5.2 Civil Service Examination
Multiple-choice questions from the Chinese civil service exam (Xingce), 651 in total. See [AGIEval](https://github.com/ruixiangcui/AGIEval).
Example evaluation sample:
> A township is planning a new district. It has decided to build four themed communities — Culture, Leisure, Commerce, and Administrative Services — to the east, south, west, and north of the citizens' park at the center. It is known that the Administrative Services district is to the southwest of the Culture district, and the Culture district is to the southeast of the Leisure district.
Based on the above, which of the following can be concluded?
(A) The citizens' park is to the north of the Administrative Services district  (B) The Leisure district is to the southwest of the Culture district  (C) The Culture district is to the northeast of the Commerce district  (D) The Commerce district is to the southeast of the Leisure district
>

Full leaderboard: [Civil Service Examination](leaderboard/考公-EN.md)<br>
See [Civil Service Examination: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=kaogong-so)
<br><br><br>



## 6. Reasoning & Math Leaderboard
Full leaderboard: [Reasoning & Math](leaderboard/推理与数学计算-EN.md)<br>

### 6.1 Deductive Reasoning
Deductive reasoning (modus tollens) multiple-choice questions, 123 in total. See [ISP](https://arxiv.org/abs/2306.09479).

Example evaluation sample:
> Consider the following statements:
1. If John is a good parent, then John is strict but fair. 2. John is not strict but fair. Conclusion: Therefore, John is not a good parent.
Question: Based on statements 1 and 2, is the conclusion correct?
Answer: (A) No   (B) Yes
>

Full leaderboard: [Deductive Reasoning](leaderboard/演绎推理-EN.md)<br>
See [Deductive Reasoning: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=演绎推理)
<br><br>


### 6.2 Commonsense Reasoning
Commonsense reasoning multiple-choice questions, 99 in total. See [ISP](https://arxiv.org/abs/2306.09479).

Example evaluation sample:
> The following is a multiple-choice question about common sense.
Question: When someone places a potato into the embers next to a campfire, at that moment the embers are not
A. releasing heat  B. absorbing heat
>

Full leaderboard: [Commonsense Reasoning](leaderboard/常识推理-EN.md)<br>
See [Commonsense Reasoning: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=常识推理)
<br><br>


### 6.3 Symbolic Reasoning (BBH)
The most widely used symbolic reasoning benchmark in academia, containing 23 sub-tasks. See [BBH](https://nonelinear.com/static/benchmarks.html) for details.
Example evaluation sample:
> Task description: Answer questions about which times certain events could have occurred.
Q: Today, Emily went to the museum. Between what times could they have gone?
We know that:
Emily woke up at 1pm.
Elizabeth saw Emily reading at the library from 2pm to 4pm.
Jessica saw Emily watching a movie at the theater from 4pm to 5pm.
Leslie saw Emily waiting at the airport from 5pm to 6pm.
William saw Emily buying clothes at the mall from 6pm to 7pm.
The museum was closed after 7pm.
Between what times could Emily have gone to the museum?
Options:
(A) 1pm to 2pm   (B) 6pm to 7pm   (C) 5pm to 6pm   (D) 2pm to 4pm
A:
>

Full leaderboard: [BBH](leaderboard/bbh-EN.md)<br>
See [BBH Symbolic Reasoning: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=BBH)
<br><br>


### 6.4 Arithmetic
Tests the basic arithmetic capability of LLMs. Test items include integer addition and subtraction within 1000, and addition, subtraction, multiplication, and division of floating-point numbers with up to 2 significant figures.
Examples: 166 + 215 + 53 = ?, 0.97 + 0.4 / 4.51 = ?

Full leaderboard: [Arithmetic](leaderboard/算术能力-EN.md)<br>
See [Arithmetic: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=算术能力)
<br><br>


### 6.5 Table QA
Specifically evaluates LLMs' ability to understand and analyze tables, commonly used in data analysis.
Example evaluation sample:
> Name,Age,Gender,Nationality,Height(cm),Weight(kg),Education
Zhang San,28,Male,China,180,70,Bachelor's
Lisa,33,Female,USA,165,58,Master's
Paulo,41,Male,Brazil,175,80,PhD
Miyuki,25,Female,Japan,160,50,Associate's
Ahmed,30,Male,Egypt,175,68,Bachelor's
Maria,29,Female,Mexico,170,65,Master's
Antonio,36,Male,Spain,182,75,PhD
Based on this table, answer: Which nationality has the lowest level of education?
>

Full leaderboard: [Table QA](leaderboard/表格问答-EN.md)<br>
See [Table QA: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=表格问答)
<br><br>


### 6.6 Table Summarization
Specifically evaluates LLMs' ability to analyze and summarize tables, commonly used in data analysis and article writing. There is no single fixed correct answer, but quality differences are still relatively easy to judge objectively.
Example evaluation sample (some data omitted due to length):
> |Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
> |---|---|-----|-------------------|-------|-----------|-----------|-----------|
> |Commercial|Doubao|doubao-seed-1-6-thinking-250715|87.5|37s|1976|14.6|1|
> |Commercial|Baidu|ERNIE-4.5-Turbo-32K|84.7|33s|676|1.8|2|
> |Commercial|Tencent|hunyuan-t1-20250711|84.7|37s|2465|9.2|3|
> |Commercial|Tencent|hunyuan-turbos-20250716|83.9|24s|1288|2.3|4|
> |……|……|……|……|……|……|……|……|
> -------------------------
> The new models are: GLM-4.5, GLM-4.5-Air, GLM-4.5-Flash, step-3.
> Based on the table above, write a summary in the format: "Org xx, Org xx … occupy the top 5 (do not repeat organization names), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx … (from highest to lowest)". Strictly follow the model and organization names from the table.
>

Full leaderboard: [Table Summarization](leaderboard/表格总结-EN.md)<br>
See [Table Summarization: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=表格总结)
<br><br>


### 6.7 High School Math Olympiad
2024 preliminary exam questions. See [Math24o](https://github.com/CLUEbenchmark/Math24o).
Example evaluation sample:
> Let the set $S=\{1, 2, 3, \cdots, 9 9 7, 9 9 8 \}$. Suppose $k$ subsets of $S$ each having 499 elements, $A_{1}, A_{2}, \cdots, A_{k}$, satisfy: for any 2-element subset $B$ of $S$, there exists $i \in \{1, 2, \cdots, k\}$ such that $B \subset A_{i}$. Find the minimum value of $k$.
>

Full leaderboard: [High School Math Olympiad](leaderboard/高中奥数-EN.md)<br>
See [High School Math Olympiad: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=高中奥数)
<br><br>


### 6.8 Middle School Math Olympiad (TODO)
<br>


### 6.9 Elementary School Math Olympiad
Full leaderboard: [Elementary School Math Olympiad](leaderboard/小学奥数-EN.md)<br>
See [Elementary School Math Olympiad: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=小学奥数一年级)
<br><br>


### 6.10 Map Reasoning (TODO)
### 6.11 Spatial Reasoning (TODO)
<br>


### 6.12 Sudoku
Full leaderboard: [Sudoku](leaderboard/数独-EN.md)<br>
See [Sudoku: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=数独入门)
<br>


### 6.13 Amount Numeric-to-Text Conversion (TODO)
### 6.14 Date Calculation (TODO)
<br><br><br>



## 7. Language & Instruction Following Leaderboard
Full leaderboard: [Language & Instruction Following](leaderboard/语言与指令遵从-EN.md)<br>

### 7.1 Idiom Understanding
Given a context, select the best-matching idiom.

Example evaluation sample:
> Having talked about the strengths of the work, let's discuss why its ending is said to be ____. The topic the film raises is very sharp; the "younger-brother-spoiler" has become an uncertain factor in many young people's marriages. So for such a sensitive issue, the film's ending merely uses the younger brother's cuteness to resolve the sister's worries, and in the end she chooses to stay and take care of him...
Choose the most fitting idiom or saying for the blank above:
(A) orderly and well-organized   (B) listening to only one side   (C) a poor sequel to a great work   (D) half of the empire   (E) life and family   (F) timid as a mouse   (G) keeping oneself untainted
>

Full leaderboard: [Idiom Understanding](leaderboard/成语理解-EN.md)<br>
See [Idiom Understanding: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=成语理解)
<br><br>


### 7.2 Sentiment Analysis
Analyze the sentiment of user reviews — positive or negative.

Example evaluation sample:
> After using it for a few days, I found many problems: the wireless network drops easily, the screen scratches easily, and web pages crash often. Not worth buying.
Is the above user review positive or negative?
(A) Negative   (B) Positive
>

Full leaderboard: [Sentiment Analysis](leaderboard/情感分析-EN.md)<br>
See [Sentiment Analysis: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=情感分析)
<br><br>


### 7.3 Textual Entailment
Textual entailment — determining the semantic relationship between two sentences: entailment, neutral, or contradiction. See [OCNLI](https://arxiv.org/abs/2010.05444).

Example evaluation sample:
> Sentence 1: Subsidies for purchasing agricultural machinery now cover all agricultural and pastoral counties (farms) nationwide; the central government plans to allocate 13 billion yuan, an increase of 9 billion yuan from the previous year.
Sentence 2: Subsidies are distributed based on the number of farmers.
What is the relationship between these two sentences?
(A) Entailment  (B) Neutral  (C) Contradiction
>

Full leaderboard: [Textual Entailment](leaderboard/文本蕴含-EN.md)<br>
See [Textual Entailment: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=文本蕴含)
<br><br>


### 7.4 Text Classification
Example evaluation sample:
> Classify the following words by part of speech.
> Dog, chase, run, adult, happy, tree

Full leaderboard: [Text Classification](leaderboard/文本分类-EN.md)<br>
See [Text Classification: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=文本分类)
<br><br>


### 7.5 Information Extraction
Example evaluation sample:
> "CITIC Bank 300 million yuan, Bank of Communications grew by approximately 2.7 billion yuan, Everbright Bank approximately 1 billion yuan."
> Extract all organization names from the text above.

Full leaderboard: [Information Extraction](leaderboard/信息抽取-EN.md)<br>
See [Information Extraction: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=信息抽取)
<br><br>


### 7.6 Reading Comprehension
Reading comprehension is a composite ability, testing the understanding of given information.
Depending on the type of information given, it can be subdivided into article QA, table QA, dialog QA, and so on.
Example evaluation sample:
> Dentist: OK, let me take a look at your teeth. Based on your description and our examination, you might have some gum disease, which has irritated the nerves and caused sensitivity. In addition, these black spots may be cavities.
Patient: Oh, really? What should I do?
Dentist: Don't worry, we can create a treatment plan for you. We need to first treat the gum disease, then remove the decay and fill the cavities. During the process, we'll make sure you're comfortable and use the latest techniques and materials for best results.
Patient: OK, thank you, doctor. So when can I start treatment?
Dentist: Let's schedule an appointment. Your treatment will begin in two days. In the meantime, please continue brushing, flossing, and avoiding overly sweet or acidic food and drink.
Patient: OK, I will. Thanks again, doctor.
Dentist: You're welcome. We'll do our best to help you restore healthy teeth.
Based on the dialog above, answer: What dental issues did the patient have detected during the examination?
>

Full leaderboard: [Reading Comprehension](leaderboard/阅读理解-EN.md)<br>
See [Reading Comprehension: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=阅读理解)
<br><br>


### 7.7 Pronoun Resolution
Chinese coreference resolution task. See [CLUEWSC2020](https://github.com/CLUEbenchmark/CLUEWSC2020).
Example evaluation sample:
> Shaoping still didn't know how to explain his brother-in-law's situation to grandma, so he just said offhandedly: "He made a mistake — they sent him to labor reeducation!"
In the sentence "He made a mistake" above, does "he" refer to Shaoping? Options: (A) Yes   (B) No
>

Full leaderboard: [Pronoun Resolution](leaderboard/代词理解-EN.md)<br>
See [Pronoun Resolution: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=代词理解)
<br><br>


### 7.8 Poetry Matching
Classical Chinese poetry matching. Given a modern-language description of a classical Chinese poem, select the line from four candidate verses whose meaning best matches the description.
Correct options are constructed from parallel corpora of classical poetry and modern translations, while incorrect options are generated by similarity-retrieval against a classical poetry corpus.
See [CCPM](https://github.com/THUNLP-AIPoet/CCPM).
Example evaluation sample:
> A dim lamp went out and was rekindled.
Which of the following lines best matches the above:
(A) The fishing lamp went out then lit again   (B) The waning lamp died out then burned again   (C) The waning lamp dimmed then brightened again   (D) The waning lamp went out then shone again
>

Full leaderboard: [Poetry Matching](leaderboard/诗词匹配-EN.md)<br>
See [Poetry Matching: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=诗词匹配)
<br><br>


### 7.9 Chinese Instruction Following
Adapted from Google's IFEval, translated and tailored to Chinese, with 25 carefully chosen instructions across 9 categories, as illustrated below:
![lin](pic/IFEval.jpg)

Full leaderboard: [IFEval](leaderboard/中文指令遵从-EN.md)<br>
See [Chinese Instruction Following: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=中文指令遵从)
<br><br>


### 7.10 Chinese Character Glyphs
Full leaderboard: [Chinese Character Glyphs](leaderboard/汉字字形-EN.md)<br>
See [Chinese Character Glyphs: badcase](https://nonelinear.com/static/badcase/badcase-of-benchmark.html?benchmark=汉字字形)
<br><br>


### 7.11 Pinyin (TODO)
### 7.12 Typo Detection (TODO)
### 7.13 Sentence Understanding (TODO)
### 7.14 Punctuation (TODO)
### 7.15 Traditional/Simplified Conversion (TODO)
### 7.16 Language Identification (TODO)
<br><br><br>


## 8. Agent & Tool Use Leaderboard
Averages the TAU and BFCL-V3 scores.<br>
Full leaderboard: [Agent & Tool Use Leaderboard](leaderboard/agent与工具调用-EN.md)<br>

### 8.1 TAU
Full leaderboard: [TAU](leaderboard/TAU-EN.md)<br>
#### (1) TAU-airline
Full leaderboard: [TAU-airline](leaderboard/TAU-airline-EN.md)<br>

#### (2) TAU-retail
Full leaderboard: [TAU-retail](leaderboard/TAU-retail-EN.md)
<br><br>


### 8.2 BFCL-V3
BFCL-V3 is a tool-call evaluation benchmark released by UC Berkeley. It is the first to introduce multi-turn, multi-step function-calling scenarios and to evaluate a model's true interaction capability via API state verification. It is currently one of the most authoritative tool-use benchmarks for LLMs.
<br>Full leaderboard: [BFCL-V3](leaderboard/BFCL-V3-EN.md)
<br><br><br>



## 9. Coding Leaderboard
Evaluates LLM coding capability. Full leaderboard: [Coding](leaderboard/coding-EN.md)<br>

### 9.1 LiveCodeBench
[LiveCodeBench](https://github.com/LiveCodeBench/LiveCodeBench) provides a comprehensive, contamination-free evaluation of LLM coding capability. Specifically, LiveCodeBench continuously collects new problems over time from three major competitive-programming platforms: LeetCode, AtCoder, and CodeForces.
<br>Full leaderboard: [LiveCodeBench](leaderboard/livecodebench-EN.md)
<br><br>


### 9.2 Terminal-Bench-2.0
[Terminal-Bench](https://github.com/harbor-framework/terminal-bench-2) is a popular benchmark that evaluates the ability of agents and LLMs to perform valuable work in containerized environments. Tasks include things like protein-synthesis assembly, asynchronous code debugging, and security-vulnerability fixes.
<br>Full leaderboard: [Terminal-Bench-2.0](leaderboard/Terminal-Bench-2.0-EN.md)
<br><br><br>


## 10. Combined LMArena and AA Scores
Combines data from our ReLE benchmark (Chinese), LMArena (English), and Artificial Analysis (AA, English) leaderboards.

| Model                                  | ReLE (Chinese) |    | AA-Intelligence (English) | AA-Coding (English) | AA-Math (English) |    | LMArena-Text-overall (English) | LMArena-Text-coding (English) | LMArena-WebDev (English) |
|:---------------------------------------|:---------------|:---|:--------------------------|:--------------------|:------------------|:---|:-------------------------------|:------------------------------|:-------------------------|
| gemini-3-pro-preview(new)              | 72.5           |    | 72.8                      | 62.3                | 95.7              |    | 1495                           | 1541                          | 1487                     |
| gpt-5.1-high(new)                      | 69.7           |    | 69.7                      | 57.5                | 94.0              |    | 1454                           | 1496                          | /                        |
| gpt-5.1-medium(new)                    | 69.3           |    | /                         | /                   | /                 |    | /                              | /                             | /                        |
| gpt-5-high                             | /              |    | 68.5                      | 52.7                | 94.3              |    | 1436                           | 1470                          | 1473                     |
| GPT-5 Codex (high)                     | /              |    | 68.5                      | 53.5                | 98.7              |    | /                              | /                             | /                        |
| kimi-k2-thinking(new)                  | 67.9           |    | 67.0                      | 52.2                | 94.7              |    | 1422                           | 1473                          | /                        |
| gpt-5-2025-08-07                       | 68.9           |    | 66.4                      | 49.2                | 91.7              |    | /                              | /                             | /                        |
| DeepSeek-V3.2-Think                    | 70.9           |    | 66.0                      | /                   | /                 |    | /                              | /                             | /                        |
| DeepSeek-V3.2                          | 64.4           |    | 52.0                      | /                   | /                 |    | /                              | /                             | /                        |
| o3                                     | /              |    | 65.5                      | 52.2                | 88.3              |    | 1435                           | 1458                          | 1186                     |
| grok-4-0709                            | 61.2           |    | 65.3                      | 55.1                | 92.7              |    | 1410                           | 1435                          | 1174                     |
| ...                                    | ...            |    | ...                       | ...                 | ...               |    | ...                            | ...                           | ...                      |

Full scores: [LMArena+AA](LMArena+AA-EN.md)
<br><br>


## Capability Scores by Dimension
Scoring method: each LLM is scored along multiple dimensions; each dimension corresponds to an evaluation dataset containing a number of questions.
Each question is scored 1–5 based on the quality of the model's response. The scores for all questions in the dataset are summed and normalized to a 100-point scale, yielding the final score.

All scoring data: [alldata](leaderboard/alldata-EN.md)
<br><br>


## Why this leaderboard?
- LLMs are blooming in many forms, but their quality varies widely. Media coverage often exaggerates or glosses over weaknesses, which can be misleading; and some companies, for PR reasons, overstate their models' abilities, casually claiming to "match ChatGPT" or to be "number one in China".
As the saying goes, "outsiders watch the spectacle, insiders see the mechanics". The industry needs a current of cool air — one that resists hype, settles down to refine cutting-edge technology, and lets real technical capability speak for itself. That requires an open, fair, and impartial LLM evaluation system that lays out the strengths and weaknesses of various models for everyone to see.
With it, we can both grasp the current state of the art and the gap with top international technology, and more clearly see the direction of future effort, without being swept along by capital frenzy or public-opinion hype.
- For industry — especially for companies that don't develop LLMs themselves — understanding the technical boundaries of LLMs and efficiently choosing the right model for the task is becoming increasingly important.
An open, fair, and impartial LLM evaluation system provides exactly the kind of help needed: avoiding reinventing the wheel, avoiding unnecessary disputes caused by different tech stacks, and avoiding talking past each other.
- For LLM developers — including those interested in LLM technology and academics who value practice — comparisons of various models reflect the effectiveness of different technical routes and methods behind them, providing a very valuable reference.
Cross-referencing and learning from each other helps everyone avoid unnecessary pitfalls and wasted experimental resources, and contributes to the healthy, efficient development of the entire LLM ecosystem.
<br><br>


## Contact Us (Nonelinear AI ReLE benchmark team)
### Model Evaluation Community
First add the editor on WeChat, who will pull you into the group; please add a note "from GitHub, joining the group"<br>
![lin](pic/qrcode-wxgroup.jpg)
<br><br><br>
### Model Evaluation WeChat Official Account
Follow the WeChat official account for LLM evaluation to get the latest evaluation updates in time<br>
![lin](pic/qrcode-gzh.jpg)
<br><br><br>

---

## How to Cite ReLE (Cite Us)

If you use ReLE (chinese-llm-benchmark) data, results, or code in your papers, reports, or open-source projects, please cite us as follows. This helps us maintain the open-source evaluation ecosystem.

### Chinese Citation (GB/T 7714)
ReLE Benchmark Team. ReLE: Chinese AI LLM Capability Evaluation Dataset and Open Leaderboard [EB/OL]. GitHub, 2023-06-04 [2025-12-06]. https://github.com/jeinlee1991/chinese-llm-benchmark. DOI: 10.5281/zenodo.xxxxxxx.

### APA (7th)
ReLE Benchmark Team. (2023, June 4). *ReLE: Really Reliable Live Evaluation for Chinese LLMs* (Version v5.8.5) [Computer software]. GitHub. https://github.com/jeinlee1991/chinese-llm-benchmark

### IEEE
[1] ReLE Benchmark Team, "ReLE: Really Reliable Live Evaluation for Chinese LLMs," GitHub repository, v5.8.5, Jun. 4, 2023. https://github.com/jeinlee1991/chinese-llm-benchmark

### BibTeX
```bibtex
@misc{rele2023benchmark,
  author       = {{ReLE Benchmark Team}},
  title        = {ReLE: Really Reliable Live Evaluation for Chinese LLMs},
  year         = {2025},
  url          = {https://github.com/jeinlee1991/chinese-llm-benchmark},
  version      = {v5.8.5},
  publisher    = {GitHub}
}
```

### Versioning Notes
ReLE uses semantic versioning (`MAJOR.MINOR.PATCH`).
- MAJOR: significant framework or metric/weighting changes
- MINOR: new domains, sub-leaderboards, or >10% expansion of the question bank
- PATCH: bug fixes, sample de-noising, model additions

When citing, please specify the **exact tag** you used (e.g., `v5.8.5`) to ensure reproducibility.

