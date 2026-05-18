# WeChat Article Writing — Table Summarization: How to Choose the Most Suitable Model?
Want to pick the "smartest" yet most cost-effective model?
No worries! We bring you a "zero-code" evaluation workflow: from preparing data and creating tasks to comparing accuracy, time, and cost in real time, we'll guide you step-by-step through benchmarking popular open-source/commercial models.
Finalize your model selection in 5 minutes and pick a "writer" model that's both smart and economical, making every penny count! (Preface written by kimi-k2)

## 1. Prepare Test Data
As an example, we prepared 9 data items as follows:
[Input] represents the model input (i.e., the prompt); [Expected Output] represents the reference answer.<br>
### (1) Sample 1
[Input]:
``` |Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|Doubao|doubao-seed-1-6-thinking-250715|88.0|37s|2144|15.5|1|
|Commercial|Tencent|hunyuan-t1-20250711|85.5|40s|2693|9.9|2|
|Open-source|Doubao|Seed-OSS-36B-Instruct|85.2|156s|2832|10.8|3|
|Open-source|DeepSeek|DeepSeek-R1-0528|84.4|215s|3077|48.0|4|
|Open-source|DeepSeek|DeepSeek-V3.1-Think|84.3|103s|2186|24.7|5|
|Commercial|Alibaba|*qwen-plus-think-2025-07-28|84.1|/|3452|25.9|6|
|Commercial|Alibaba|*qwen3-max-preview|84.0|16s|898|17.4|7|
|Commercial|Baidu|ERNIE-4.5-Turbo-32K|83.6|66s|713|1.8|8|
|Commercial|Alibaba|*qwen-plus-2025-07-28|83.5|24s|1054|1.8|9|
|Commercial|Baidu|ERNIE-X1-Turbo-32K|83.4|288s|2609|9.7|10|
|Open-source|Alibaba|qwen3-235b-a22b-instruct-2507|83.0|22s|1061|7.1|11|
|Open-source|Alibaba|qwen3-235b-a22b-thinking-2507|82.9|99s|3389|62.1|12|
|Commercial|Google|gemini-2.5-pro|82.6|33s|2798|188.2|13|
|Commercial|Tencent|hunyuan-turbos-20250716|82.6|27s|1321|2.3|14|
|Commercial|OpenAI|gpt-5-2025-08-07|82.2|38s|600|30.0|15|
|Open-source|Moonshot|kimi-k2-0711-preview|81.6|62s|984|13.5|16|
|Commercial|xAI|grok-4-0709|80.6|293s|2379|241.5|17|
|Commercial|Doubao|doubao-seed-1-6-250615|80.0|90s|625|3.1|18|
|Open-source|Alibaba|Qwen3-30B-A3B-Thinking-2507|79.7|74s|3285|8.7|19|
|Commercial|Doubao|Doubao-1.5-pro-32k-250115|79.6|11s|541|0.8|20|
|Open-source|DeepSeek|DeepSeek-V3.1|79.5|27s|663|6.4|21|
|Commercial|Alibaba|qwen-flash-think-2025-07-28|78.7|32s|3271|4.6|22|
|Open-source|Baidu|ERNIE-4.5-300B-A47B|78.6|94s|588|3.3|23|
|Open-source|Zhipu AI|GLM-4.5|78.5|84s|3031|39.9|24|
|Commercial|Doubao|doubao-seed-1-6-flash-thinking-250615|78.4|19s|1712|2.2|25|
|Open-source|DeepSeek|deepseek-chat-v3-0324|78.3|132s|861|6.1|26|
|Open-source|Zhipu AI|GLM-4.5-Air|78.3|54s|3197|17.9|27|
|Open-source|StepFun|step-3|78.0|170s|3322|12.8|28|
|Commercial|iFlytek|xunfei-spark-x1-0725|77.8|/|2060|24.6|29|
|Open-source|MiniMax|MiniMax-M1|77.8|226s|4392|32.0|30|
|……|……|……|……|……|……|……|……|
|Commercial|Alibaba|*qwen-turbo-think-2025-07-15|76.6|/|3109|8.7|36|
|Commercial|Mistral|*mistral-medium-2508|70.2|159s|751|7.9|60|
|Open-source|Mistral|*Magistral-Small-2507|66.5|197s|6663|70.6|77|
|Open-source|Mistral|*Mistral-Small-3.2-24B-Instruct-2506|62.0|126s|1208|2.2|84|
-------------------------
The known new models are: mistral-medium-2508, Magistral-Small-2507, Mistral-Small-3.2-24B-Instruct-2506, qwen3-max-preview, qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, qwen-turbo-think-2025-07-15.
Based on the table above, write a summary in the format: "xx organization, xx organization... occupy the top 5 (organization names should not be repeated), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx... (ranked from highest to lowest)". Strictly follow the model names and organization names in the table.
```
[Expected Output]: <ignore, no need to fill in>
### (2) Sample 2
[Input]:
 ```|Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|Doubao|doubao-seed-1-6-thinking-250715|89.2|/|2660|18.8|1|
|Commercial|OpenAI|gpt-5-2025-08-07|89.0|44s|756|35.1|2|
|Open-source|Doubao|Seed-OSS-36B-Instruct|88.1|179s|3397|12.7|3|
|Open-source|DeepSeek|DeepSeek-R1-0528|88.0|214s|3766|58.9|4|
|Commercial|Tencent|hunyuan-t1-20250711|88.0|51s|3504|12.8|5|
|Commercial|OpenAI|o4-mini|87.8|39s|1682|46.8|6|
|Commercial|OpenAI|gpt-5-mini-2025-08-07|87.4|63s|1625|19.7|7|
|Open-source|DeepSeek|DeepSeek-V3.1-Think|86.1|140s|3022|34.0|8|
|Commercial|Alibaba|*qwen-plus-think-2025-07-28|85.5|/|3938|29.0|9|
|Commercial|Google|gemini-2.5-pro|85.2|34s|2987|194.5|10|
|Commercial|Alibaba|*qwen3-max-preview|85.2|19s|1142|21.2|11|
|Commercial|xAI|grok-4-0709|84.9|270s|2702|268.8|12|
|Open-source|Alibaba|qwen3-235b-a22b-thinking-2507|84.8|107s|3868|68.1|13|
|Open-source|OpenAI|gpt-oss-120b|84.2|73s|1313|3.4|14|
|Commercial|Alibaba|*qwen-plus-2025-07-28|84.1|28s|1308|2.2|15|
|Open-source|Alibaba|qwen3-235b-a22b-instruct-2507|83.8|27s|1333|8.6|16|
|Open-source|Alibaba|Qwen3-30B-A3B-Thinking-2507|83.7|79s|3679|9.6|17|
|Commercial|Baidu|ERNIE-X1-Turbo-32K|83.7|366s|3060|11.1|18|
|Open-source|Zhipu AI|GLM-4.5-Air|83.2|69s|4147|23.0|19|
|Commercial|Anthropic|claude-4-sonnet-thinking|83.0|53s|1036|90.3|20|
|Open-source|Moonshot|kimi-k2-0711-preview|82.7|80s|1260|16.8|21|
|Commercial|Alibaba|qwen-flash-think-2025-07-28|82.6|35s|3589|4.9|22|
|Commercial|OpenAI|gpt-5-nano-2025-08-07|81.9|59s|2912|7.7|23|
|Commercial|Zhipu AI|GLM-4.5-Flash|81.8|72s|4083|0.0|24|
|Open-source|Zhipu AI|GLM-4.5|81.5|93s|3890|50.9|25|
|Open-source|OpenAI|gpt-oss-20b|81.3|134s|2261|2.3|26|
|Commercial|Anthropic|claude-4-sonnet|81.2|47s|585|42.0|27|
|Commercial|Baidu|ERNIE-4.5-Turbo-32K|81.0|93s|792|1.7|28|
|Open-source|StepFun|step-3|80.9|200s|3990|15.2|29|
|Open-source|DeepSeek|DeepSeek-V3.1|80.4|31s|823|7.6|30|
|……|……|……|……|……|……|……|……|
|Commercial|Alibaba|*qwen-turbo-think-2025-07-15|79.9|/|3408|9.3|31|
|Open-source|Mistral|*Magistral-Small-2507|74.2|248s|6845|71.7|51|
|Commercial|Mistral|*mistral-medium-2508|70.2|197s|873|8.3|62|
|Open-source|Mistral|*Mistral-Small-3.2-24B-Instruct-2506|65.7|154s|1495|2.7|81|
-------------------------
The known new models are: mistral-medium-2508, Magistral-Small-2507, Mistral-Small-3.2-24B-Instruct-2506, qwen3-max-preview, qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, qwen-turbo-think-2025-07-15.
Based on the table above, write a summary in the format: "xx organization, xx organization... occupy the top 5 (organization names should not be repeated), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx... (ranked from highest to lowest)". Strictly follow the model names and organization names in the table.
```
[Expected Output]: <ignore, no need to fill in>
### (3) Sample 3
[Input]:
```|Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|Doubao|doubao-seed-1-6-thinking-250715|86.7|36s|1629|12.3|1|
|Commercial|Baidu|ERNIE-4.5-Turbo-32K|86.2|40s|635|1.8|2|
|Commercial|Tencent|hunyuan-turbos-20250716|85.3|24s|1181|2.2|3|
|Commercial|Doubao|doubao-seed-1-6-250615|84.3|87s|505|3.1|4|
|Commercial|Doubao|Doubao-1.5-pro-32k-250115|83.5|13s|460|0.8|5|
|Commercial|Baidu|ERNIE-X1-Turbo-32K|83.1|210s|2158|8.3|6|
|Commercial|Tencent|hunyuan-t1-20250711|83.0|29s|1883|7.0|7|
|Commercial|Alibaba|*qwen-plus-2025-07-28|83.0|20s|801|1.5|8|
|Commercial|Alibaba|*qwen3-max-preview|82.9|13s|654|13.6|9|
|Commercial|Alibaba|*qwen-plus-think-2025-07-28|82.7|/|2966|22.9|10|
|Open-source|DeepSeek|DeepSeek-V3.1-Think|82.6|66s|1351|15.4|11|
|Open-source|Alibaba|qwen3-235b-a22b-instruct-2507|82.3|18s|790|5.7|12|
|Open-source|Doubao|Seed-OSS-36B-Instruct|82.2|133s|2267|8.8|13|
|Open-source|Alibaba|qwen3-235b-a22b-thinking-2507|81.1|92s|2910|56.1|14|
|Open-source|DeepSeek|DeepSeek-R1-0528|80.8|216s|2388|37.0|15|
|Open-source|Moonshot|kimi-k2-0711-preview|80.6|44s|709|10.2|16|
|Commercial|Doubao|doubao-seed-1-6-flash-thinking-250615|80.6|14s|937|1.2|17|
|Open-source|Baidu|ERNIE-4.5-300B-A47B|80.5|113s|507|3.4|18|
|Commercial|Google|gemini-2.5-pro|80.0|33s|2609|182.0|19|
|Commercial|iFlytek|xunfei-spark-x1-0725|78.9|/|1528|18.1|20|
|Open-source|DeepSeek|DeepSeek-V3.1|78.7|24s|504|5.3|21|
|Open-source|Alibaba|Qwen3-32B|78.0|104s|2843|11.0|22|
|Open-source|DeepSeek|deepseek-chat-v3-0324|77.5|134s|747|5.4|23|
|Commercial|Doubao|doubao-seed-1-6-flash-250615|77.0|5s|446|0.5|24|
|Commercial|xAI|grok-4-0709|76.3|316s|2057|214.1|25|
|Commercial|Doubao|Doubao-1.5-lite-32k-250115|76.3|8s|324|0.2|26|
|Open-source|MiniMax|MiniMax-M1|76.1|259s|4147|30.5|27|
|Open-source|Alibaba|Qwen3-30B-A3B-Thinking-2507|75.7|70s|2892|7.9|28|
|Open-source|Zhipu AI|GLM-4.5|75.5|76s|2173|28.9|29|
|Open-source|Alibaba|Qwen3-14B|75.5|118s|4090|8.0|30|
|……|……|……|……|……|……|……|……|
|Commercial|Alibaba|*qwen-turbo-think-2025-07-15|73.4|/|2811|8.1|42|
|Commercial|Mistral|*mistral-medium-2508|70.1|121s|630|7.4|55|
|Open-source|Mistral|*Magistral-Small-2507|58.8|146s|6482|69.4|81|
|Open-source|Mistral|*Mistral-Small-3.2-24B-Instruct-2506|58.4|98s|922|1.8|84|
-------------------------
The known new models are: mistral-medium-2508, Magistral-Small-2507, Mistral-Small-3.2-24B-Instruct-2506, qwen3-max-preview, qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, qwen-turbo-think-2025-07-15.
Based on the table above, write a summary in the format: "xx organization, xx organization... occupy the top 5 (organization names should not be repeated), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx... (ranked from highest to lowest)". Strictly follow the model names and organization names in the table.
```
[Expected Output]: <ignore, no need to fill in>
### (4) Sample 4
[Input]:
``` 
|Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|Doubao|doubao-seed-1-6-thinking-250715|89.8|22s|1472|10.9|1|
|Open-source|Doubao|Seed-OSS-36B-Instruct|89.6|137s|2127|8.2|2|
|Commercial|Tencent|hunyuan-t1-20250711|89.3|31s|1996|7.3|3|
|Commercial|Alibaba|*qwen-plus-think-2025-07-28|87.8|/|2712|20.6|4|
|Open-source|Baidu|ERNIE-4.5-300B-A47B|87.4|185s|627|4.2|5|
|Commercial|Doubao|doubao-seed-1-6-250615|87.3|107s|458|2.5|6|
|Open-source|Alibaba|qwen3-235b-a22b-thinking-2507|86.8|80s|2813|53.8|7|
|Commercial|Alibaba|*qwen3-max-preview|86.7|14s|742|15.1|8|
|Commercial|Doubao|Doubao-1.5-pro-32k-250115|86.6|25s|535|0.9|9|
|Commercial|iFlytek|xunfei-spark-x1-0725|86.5|/|1846|21.8|10|
|Commercial|Baidu|ERNIE-X1-Turbo-32K|85.8|191s|2184|8.4|11|
|Commercial|Tencent|hunyuan-turbos-20250716|85.8|24s|1163|2.1|12|
|Commercial|Baidu|ERNIE-4.5-Turbo-32K|85.6|89s|677|1.9|13|
|Open-source|Alibaba|qwen3-235b-a22b-instruct-2507|85.3|21s|919|6.5|14|
|Open-source|DeepSeek|DeepSeek-V3.1-Think|85.0|69s|1421|16.0|15|
|Commercial|Doubao|doubao-seed-1-6-flash-thinking-250615|85.0|18s|1157|1.5|16|
|Commercial|Google|gemini-2.5-pro|84.9|32s|2837|197.2|17|
|Open-source|Alibaba|Qwen3-30B-A3B-Thinking-2507|84.7|66s|2713|7.3|18|
|Open-source|Moonshot|kimi-k2-0711-preview|84.6|51s|765|10.8|19|
|Commercial|Alibaba|*qwen-plus-2025-07-28|84.5|22s|909|1.6|20|
|Commercial|Alibaba|qwen-flash-think-2025-07-28|83.8|25s|2683|3.8|21|
|Commercial|Doubao|doubao-seed-1-6-flash-250615|83.6|6s|516|0.6|22|
|Open-source|Alibaba|Qwen3-32B|82.9|147s|3599|14.0|23|
|Open-source|DeepSeek|DeepSeek-R1-0528|82.6|211s|2757|42.7|24|
|Open-source|Tencent|Hunyuan-A13B-Instruct|82.5|145s|1385|5.2|25|
|Open-source|DeepSeek|DeepSeek-V3.1|82.4|24s|555|5.6|26|
|Commercial|Doubao|Doubao-1.5-lite-32k-250115|81.4|20s|350|0.2|27|
|Commercial|OpenAI|gpt-5-2025-08-07|81.3|33s|507|28.0|28|
|Commercial|xAI|grok-4-0709|81.3|278s|2586|270.0|29|
|Commercial|Alibaba|*qwen-turbo-think-2025-07-15|81.2|/|2997|8.6|30|
|……|……|……|……|……|……|……|……|
|Commercial|Mistral|*mistral-medium-2508|74.8|86s|660|7.5|54|
|Open-source|Mistral|*Magistral-Small-2507|70.8|158s|6207|66.2|76|
|Open-source|Mistral|*Mistral-Small-3.2-24B-Instruct-2506|64.5|98s|961|1.8|83|
-------------------------
The known new models are: mistral-medium-2508, Magistral-Small-2507, Mistral-Small-3.2-24B-Instruct-2506, qwen3-max-preview, qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, qwen-turbo-think-2025-07-15.
Based on the table above, write a summary in the format: "xx organization, xx organization... occupy the top 5 (organization names should not be repeated), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx... (ranked from highest to lowest)". Strictly follow the model names and organization names in the table.
```
[Expected Output]: <ignore, no need to fill in>
### (5) Sample 5
[Input]:
```|Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|Baidu|ERNIE-4.5-Turbo-32K|91.5|21s|535|1.6|1|
|Commercial|Tencent|hunyuan-turbos-20250716|89.5|12s|633|1.1|2|
|Commercial|Doubao|Doubao-1.5-pro-32k-250115|88.3|10s|378|0.7|3|
|Commercial|Doubao|doubao-seed-1-6-thinking-250715|87.8|23s|1145|8.7|4|
|Commercial|Doubao|doubao-seed-1-6-250615|85.5|102s|462|3.0|5|
|Commercial|Tencent|hunyuan-t1-20250711|82.9|27s|1656|6.2|6|
|Commercial|Baidu|ERNIE-X1-Turbo-32K|82.8|100s|1915|7.5|7|
|Commercial|Alibaba|*qwen3-max-preview|82.8|9s|456|9.5|8|
|Open-source|Alibaba|qwen3-235b-a22b-instruct-2507|82.7|11s|489|3.5|9|
|Open-source|Baidu|ERNIE-4.5-300B-A47B|82.6|21s|333|2.2|10|
|Open-source|Doubao|Seed-OSS-36B-Instruct|82.5|102s|1790|7.0|11|
|Commercial|Alibaba|*qwen-plus-2025-07-28|82.0|12s|490|0.9|12|
|Commercial|Doubao|doubao-seed-1-6-flash-thinking-250615|81.3|8s|620|0.8|13|
|Commercial|Alibaba|*qwen-plus-think-2025-07-28|81.2|/|2468|19.1|14|
|Commercial|Doubao|doubao-seed-1-6-flash-250615|80.9|3s|318|0.4|15|
|Commercial|iFlytek|xunfei-spark-max|80.7|3s|134|4.1|16|
|Open-source|DeepSeek|DeepSeek-R1-0528|80.6|225s|1831|28.5|17|
|Commercial|Doubao|Doubao-1.5-lite-32k-250115|80.5|4s|196|0.1|18|
|Open-source|Moonshot|kimi-k2-0711-preview|80.5|30s|514|7.4|19|
|Open-source|DeepSeek|DeepSeek-V3.1-Think|80.5|51s|994|11.4|20|
|Commercial|iFlytek|xunfei-spark-x1-0725|80.0|/|979|11.8|21|
|Open-source|DeepSeek|deepseek-chat-v3-0324|79.9|101s|310|2.1|22|
|Open-source|Alibaba|Qwen3-32B|79.9|56s|1622|6.3|23|
|Commercial|iFlytek|xunfei-4.0Ultra|79.9|3s|135|9.5|24|
|Open-source|Alibaba|qwen3-235b-a22b-thinking-2507|79.5|91s|2424|46.8|25|
|Open-source|DeepSeek|DeepSeek-V3.1|79.1|17s|334|3.5|26|
|Commercial|Moonshot|kimi-latest-8k|78.5|22s|486|5.9|27|
|Commercial|Google|gemini-2.5-pro|77.8|35s|2315|163.4|28|
|Commercial|iFlytek|xunfei-spark-pro|77.2|/|/|/|29|
|Open-source|MiniMax|MiniMax-M1|77.1|168s|2807|19.2|30|
|……|……|……|……|……|……|……|……|
|Commercial|Alibaba|*qwen-turbo-think-2025-07-15|70.5|/|2153|6.2|56|
|Commercial|Mistral|*mistral-medium-2508|68.0|202s|482|5.9|62|
|Open-source|Mistral|*Magistral-Small-2507|55.3|178s|5568|59.9|83|
|Open-source|Mistral|*Mistral-Small-3.2-24B-Instruct-2506|54.1|157s|510|1.0|87|
-------------------------
The known new models are: mistral-medium-2508, Magistral-Small-2507, Mistral-Small-3.2-24B-Instruct-2506, qwen3-max-preview, qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, qwen-turbo-think-2025-07-15.
Based on the table above, write a summary in the format: "xx organization, xx organization... occupy the top 5 (organization names should not be repeated), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx... (ranked from highest to lowest)". Strictly follow the model names and organization names in the table.
```
[Expected Output]: <ignore, no need to fill in>
### (6) Sample 6
[Input]:
``` |Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|Baidu|ERNIE-4.5-Turbo-32K|85.8|22s|520|1.5|1|
|Commercial|Alibaba|*qwen3-max-preview|85.1|11s|547|11.4|2|
|Commercial|Doubao|doubao-seed-1-6-thinking-250715|84.1|28s|1472|11.1|3|
|Commercial|Tencent|hunyuan-turbos-20250716|83.9|21s|1026|1.9|4|
|Commercial|Tencent|hunyuan-t1-20250711|83.6|28s|1806|6.8|5|
|Commercial|Doubao|Doubao-1.5-pro-32k-250115|83.3|10s|403|0.7|6|
|Commercial|Alibaba|*qwen-plus-think-2025-07-28|83.0|/|2760|21.4|7|
|Open-source|DeepSeek|DeepSeek-V3.1-Think|82.8|61s|1230|14.1|8|
|Commercial|Alibaba|*qwen-plus-2025-07-28|82.8|18s|709|1.3|9|
|Open-source|Huawei|pangu-pro-moe|82.8|79s|1541|5.9|10|
|Commercial|Baidu|ERNIE-X1-Turbo-32K|82.5|123s|2085|8.1|11|
|Commercial|Doubao|doubao-seed-1-6-250615|82.0|86s|417|2.4|12|
|Open-source|Alibaba|qwen3-235b-a22b-instruct-2507|81.7|14s|637|4.5|13|
|Open-source|Alibaba|Qwen3-14B|80.2|32s|1516|2.9|14|
|Open-source|Alibaba|Qwen3-32B|79.7|32s|1218|4.6|15|
|Open-source|Alibaba|qwen3-235b-a22b-thinking-2507|79.6|111s|2682|51.9|16|
|Commercial|Doubao|doubao-seed-1-6-flash-thinking-250615|79.2|19s|1052|1.4|17|
|Open-source|DeepSeek|DeepSeek-R1-0528|79.0|240s|2222|34.5|18|
|Open-source|Baidu|ERNIE-4.5-300B-A47B|78.9|23s|507|3.5|19|
|Open-source|Moonshot|kimi-k2-0711-preview|78.6|26s|438|6.0|20|
|Open-source|DeepSeek|DeepSeek-V3.1|78.5|21s|405|4.2|21|
|Commercial|Google|gemini-2.5-pro|78.5|30s|2196|153.3|22|
|Open-source|MiniMax|MiniMax-M1|78.0|211s|3469|24.4|23|
|Commercial|Doubao|doubao-seed-1-6-flash-250615|77.2|9s|487|0.6|24|
|Commercial|Doubao|Doubao-1.5-lite-32k-250115|77.2|6s|288|0.1|25|
|Commercial|Alibaba|qwen-long-2025-01-25|76.9|43s|377|0.6|26|
|Open-source|Zhipu AI|GLM-4.5|76.9|81s|2191|29.7|27|
|Open-source|DeepSeek|deepseek-chat-v3-0324|76.8|125s|460|3.2|28|
|Open-source|Doubao|Seed-OSS-36B-Instruct|75.9|104s|2137|8.3|29|
|Commercial|iFlytek|xunfei-4.0Ultra|75.5|7s|220|15.5|30|
|……|……|……|……|……|……|……|……|
|Commercial|Mistral|*mistral-medium-2508|73.1|65s|525|6.2|41|
|Commercial|Alibaba|*qwen-turbo-think-2025-07-15|71.7|/|2774|8.1|47|
|Open-source|Mistral|*Magistral-Small-2507|55.9|140s|5837|62.6|88|
|Open-source|Mistral|*Mistral-Small-3.2-24B-Instruct-2506|54.5|112s|731|1.4|90|
-------------------------
The known new models are: mistral-medium-2508, Magistral-Small-2507, Mistral-Small-3.2-24B-Instruct-2506, qwen3-max-preview, qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, qwen-turbo-think-2025-07-15.
Based on the table above, write a summary in the format: "xx organization, xx organization... occupy the top 5 (organization names should not be repeated), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx... (ranked from highest to lowest)". Strictly follow the model names and organization names in the table.
```
[Expected Output]: <ignore, no need to fill in>
### (7) Sample 7
[Input]:
``` |Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|Doubao|doubao-seed-1-6-thinking-250715|85.0|72s|2430|18.4|1|
|Commercial|Doubao|doubao-seed-1-6-250615|82.7|53s|685|4.3|2|
|Commercial|Alibaba|*qwen-plus-2025-07-28|82.7|29s|1096|2.0|3|
|Commercial|Tencent|hunyuan-turbos-20250716|82.2|40s|1903|3.6|4|
|Open-source|DeepSeek|DeepSeek-V3.1-Think|82.0|85s|1761|20.1|5|
|Commercial|Baidu|ERNIE-4.5-Turbo-32K|81.5|29s|808|2.3|6|
|Commercial|Baidu|ERNIE-X1-Turbo-32K|81.2|428s|2451|9.4|7|
|Open-source|DeepSeek|DeepSeek-R1-0528|81.0|189s|2743|42.4|8|
|Open-source|Doubao|Seed-OSS-36B-Instruct|81.0|190s|3016|11.7|9|
|Commercial|iFlytek|xunfei-spark-x1-0725|80.2|/|1972|23.2|10|
|Open-source|Alibaba|qwen3-235b-a22b-instruct-2507|79.3|27s|1115|8.1|11|
|Commercial|Google|gemini-2.5-pro|78.8|35s|3088|214.1|12|
|Open-source|Moonshot|kimi-k2-0711-preview|78.7|72s|1119|16.4|13|
|Commercial|Alibaba|*qwen-plus-think-2025-07-28|78.7|/|3924|30.4|14|
|Open-source|Alibaba|qwen3-235b-a22b-thinking-2507|78.3|87s|3721|71.9|15|
|Commercial|Alibaba|*qwen3-max-preview|77.0|19s|873|18.4|16|
|Commercial|Doubao|doubao-seed-1-6-flash-thinking-250615|76.8|14s|922|1.1|17|
|Commercial|Tencent|hunyuan-t1-20250711|76.5|33s|2077|7.8|18|
|Open-source|Alibaba|Qwen3-30B-A3B-Thinking-2507|75.7|77s|3419|9.3|19|
|Commercial|Doubao|Doubao-1.5-pro-32k-250115|75.7|8s|524|0.9|20|
|Open-source|DeepSeek|deepseek-chat-v3-0324|75.0|188s|1564|11.8|21|
|Open-source|DeepSeek|DeepSeek-V3.1|74.7|35s|723|7.7|22|
|Commercial|xAI|grok-4-0709|74.0|424s|2495|258.8|23|
|Commercial|OpenAI|gpt-5-2025-08-07|73.7|34s|577|31.8|24|
|Open-source|Baidu|ERNIE-4.5-300B-A47B|73.2|224s|564|3.6|25|
|Open-source|StepFun|step-3|73.0|165s|3255|12.7|26|
|Open-source|MiniMax|MiniMax-M1|73.0|415s|5818|44.5|27|
|Commercial|Google|gemini-2.5-flash|73.0|15s|2991|51.7|28|
|Open-source|Zhipu AI|GLM-4.5|72.7|84s|2126|27.0|29|
|Commercial|Alibaba|qwen-flash-think-2025-07-28|72.7|39s|3762|5.5|30|
|……|……|……|……|……|……|……|……|
|Commercial|Alibaba|*qwen-turbo-think-2025-07-15|70.0|/|3323|9.6|35|
|Commercial|Mistral|*mistral-medium-2508|64.3|133s|853|10.1|53|
|Open-source|Mistral|*Mistral-Small-3.2-24B-Instruct-2506|60.3|25s|1486|2.9|64|
|Open-source|Mistral|*Magistral-Small-2507|53.3|111s|8317|89.0|77|
-------------------------
The known new models are: mistral-medium-2508, Magistral-Small-2507, Mistral-Small-3.2-24B-Instruct-2506, qwen3-max-preview, qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, qwen-turbo-think-2025-07-15.
Based on the table above, write a summary in the format: "xx organization, xx organization... occupy the top 5 (organization names should not be repeated), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx... (ranked from highest to lowest)". Strictly follow the model names and organization names in the table.
```
[Expected Output]: <ignore, no need to fill in>
### (8) Sample 8
[Input]:
``` |Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|OpenAI|o4-mini|91.1|47s|2425|66.1|1|
|Open-source|Doubao|Seed-OSS-36B-Instruct|90.2|280s|5618|21.0|2|
|Commercial|Doubao|doubao-seed-1-6-thinking-250715|90.0|63s|4295|30.2|3|
|Commercial|OpenAI|gpt-5-mini-2025-08-07|89.9|51s|2391|28.7|4|
|Commercial|OpenAI|gpt-5-2025-08-07|89.3|61s|1075|46.8|5|
|Open-source|DeepSeek|DeepSeek-R1-0528|88.5|288s|5887|92.9|6|
|Commercial|Alibaba|*qwen-plus-think-2025-07-28|88.0|/|5582|40.5|7|
|Open-source|OpenAI|gpt-oss-120b|87.4|74s|1961|5.0|8|
|Open-source|Alibaba|qwen3-235b-a22b-thinking-2507|87.0|157s|5455|92.9|9|
|Commercial|Tencent|hunyuan-t1-20250711|87.0|86s|5906|21.6|10|
|Open-source|DeepSeek|DeepSeek-V3.1-Think|86.2|234s|5113|57.7|11|
|Open-source|Alibaba|Qwen3-30B-A3B-Thinking-2507|84.9|106s|5239|13.5|12|
|Commercial|Google|gemini-2.5-pro|84.7|42s|4095|260.2|13|
|Commercial|OpenAI|gpt-5-nano-2025-08-07|83.7|76s|4061|10.6|14|
|Open-source|OpenAI|gpt-oss-20b|83.5|195s|3254|3.3|15|
|Commercial|Alibaba|*qwen3-max-preview|83.0|31s|1881|34.9|16|
|Commercial|Alibaba|qwen-flash-think-2025-07-28|82.8|51s|5142|6.9|17|
|Commercial|Alibaba|*qwen-plus-2025-07-28|82.6|45s|2145|3.6|18|
|Commercial|xAI|grok-4-0709|82.3|227s|4119|408.2|19|
|Open-source|Zhipu AI|GLM-4.5-Air|82.1|110s|6636|36.6|20|
|Open-source|Alibaba|qwen3-235b-a22b-instruct-2507|81.0|46s|2199|14.2|21|
|Open-source|Zhipu AI|GLM-4.5|80.4|127s|6030|78.6|22|
|Open-source|StepFun|step-3|80.0|319s|6341|24.2|23|
|Commercial|Anthropic|claude-4-sonnet-thinking|80.0|60s|1209|100.1|24|
|Commercial|Zhipu AI|GLM-4.5-Flash|79.9|116s|6504|0.0|25|
|Commercial|Baidu|ERNIE-X1-Turbo-32K|79.5|433s|5043|18.3|26|
|Commercial|Alibaba|*qwen-turbo-think-2025-07-15|79.0|/|5474|14.9|27|
|Open-source|MiniMax|MiniMax-M1|78.7|297s|6679|48.3|28|
|Open-source|Alibaba|Qwen3-30B-A3B-Instruct-2507|78.4|24s|2404|5.9|29|
|Commercial|xAI|grok-3-mini|77.3|132s|2531|8.5|30|
|……|……|……|……|……|……|……|……|
|Open-source|Mistral|*Magistral-Small-2507|72.6|322s|9712|101.3|43|
|Open-source|Mistral|*Mistral-Small-3.2-24B-Instruct-2506|62.5|106s|2527|4.6|65|
|Commercial|Mistral|*mistral-medium-2508|62.3|328s|1326|12.4|67|
-------------------------
The known new models are: mistral-medium-2508, Magistral-Small-2507, Mistral-Small-3.2-24B-Instruct-2506, qwen3-max-preview, qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, qwen-turbo-think-2025-07-15.
Based on the table above, write a summary in the format: "xx organization, xx organization... occupy the top 5 (organization names should not be repeated), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx... (ranked from highest to lowest)". Strictly follow the model names and organization names in the table.
```
[Expected Output]: <ignore, no need to fill in>
### (9) Sample 9
[Input]:
``` |Category|Organization|Model|Accuracy|Avg Time|Avg Tokens|Cost / 1k calls (¥)|Rank (Accuracy)|
|---|---|-----|-------------------|-------|-----------|-----------|-----------|
|Commercial|Tencent|hunyuan-turbos-20250716|89.3|10s|546|0.9|1|
|Commercial|Tencent|hunyuan-t1-20250711|89.0|17s|1103|4.0|2|
|Commercial|OpenAI|gpt-5-2025-08-07|88.6|28s|437|23.3|3|
|Open-source|Baidu|ERNIE-4.5-300B-A47B|88.5|40s|236|1.2|4|
|Commercial|Doubao|doubao-seed-1-6-thinking-250715|88.5|18s|1026|7.3|5|
|Open-source|Moonshot|kimi-k2-0711-preview|88.2|26s|488|6.6|6|
|Commercial|Baidu|ERNIE-X1-Turbo-32K|87.8|299s|1077|4.0|7|
|Commercial|Anthropic|claude-4-sonnet|87.7|40s|436|34.1|8|
|Open-source|DeepSeek|DeepSeek-R1-0528|87.6|140s|1645|24.9|9|
|Commercial|xAI|grok-4-0709|87.5|313s|1285|129.5|10|
|Commercial|Alibaba|*qwen3-max-preview|87.2|7s|404|7.5|11|
|Commercial|Baidu|ERNIE-4.5-Turbo-32K|87.1|145s|292|0.6|12|
|Open-source|Alibaba|qwen3-235b-a22b-instruct-2507|86.6|9s|467|3.0|13|
|Commercial|Doubao|Doubao-1.5-pro-32k-250115|86.2|5s|318|0.5|14|
|Open-source|Doubao|Seed-OSS-36B-Instruct|86.0|79s|1176|4.4|15|
|Commercial|Anthropic|claude-4-sonnet-thinking|86.0|47s|863|80.5|16|
|Open-source|DeepSeek|DeepSeek-V3.1-Think|85.9|46s|931|10.3|17|
|Commercial|Alibaba|*qwen-plus-2025-07-28|85.6|11s|472|0.8|18|
|Commercial|Google|gemini-2.5-pro|85.6|27s|1880|128.7|19|
|Open-source|DeepSeek|DeepSeek-V3.1|84.9|15s|326|3.1|20|
|Commercial|OpenAI|gpt-5-mini-2025-08-07|84.8|75s|860|10.7|21|
|Commercial|OpenAI|o4-mini|84.5|32s|939|27.5|22|
|Open-source|Zhipu AI|GLM-4.5-Air|84.4|29s|1658|9.3|23|
|Open-source|DeepSeek|deepseek-chat-v3-0324|84.1|117s|420|2.9|24|
|Commercial|Doubao|doubao-seed-1-6-250615|84.1|92s|349|1.6|25|
|Commercial|iFlytek|xunfei-spark-x1-0725|83.7|/|627|7.5|26|
|Commercial|Zhipu AI|GLM-4.5-Flash|83.5|29s|1662|0.0|27|
|Commercial|Alibaba|*qwen-plus-think-2025-07-28|82.9|/|2294|17.5|28|
|Open-source|Zhipu AI|GLM-4.5|82.7|59s|1750|23.1|29|
|Open-source|Alibaba|qwen3-235b-a22b-thinking-2507|82.6|57s|2281|43.4|30|
|……|……|……|……|……|……|……|……|
|Commercial|Alibaba|*qwen-turbo-think-2025-07-15|80.7|/|1343|3.7|41|
|Commercial|Mistral|*mistral-medium-2508|78.2|67s|420|4.3|59|
|Open-source|Mistral|*Magistral-Small-2507|75.7|175s|3979|42.1|69|
|Open-source|Mistral|*Mistral-Small-3.2-24B-Instruct-2506|68.8|203s|464|0.8|89|
-------------------------
The known new models are: mistral-medium-2508, Magistral-Small-2507, Mistral-Small-3.2-24B-Instruct-2506, qwen3-max-preview, qwen-plus-2025-07-28, qwen-plus-think-2025-07-28, qwen-turbo-think-2025-07-15.
Based on the table above, write a summary in the format: "xx organization, xx organization... occupy the top 5 (organization names should not be repeated), then describe the distribution of open-source and commercial models. Among the new models, xx ranks xx, xx ranks xx... (ranked from highest to lowest)". Strictly follow the model names and organization names in the table.
```
[Expected Output]: <ignore, no need to fill in>


<br><br>
## 2. Create a Model Selection Evaluation Task
First, open the task creation page at https://nonelinear.com/static/task-create.html.<br>
### (1) Step 1: Set the Task ID
Enter a Task ID — the unique identifier of the task. Once created, it cannot be modified. Here, based on the specific task, we set it to: rele-weekly-ranking/summary-one-domain.<br>

### (2) Step 2: Choose Models
Choose the models you want to evaluate. The page provides a default "Curated Cost-Effective Models" list (ordered from highest to lowest cost-effectiveness; models lower in the list are relatively less effective but cheaper), as well as a "Flagship Models" list.
Of course, you can also click to view more models, with support for filtering by "thinking model or not", "open-source or not", and "domestic/foreign model".
As an example, we selected 2 models: gpt-oss-20b and Qwen3-8B:free.
![link](img/创建任务-更多模型.png)

### (3) Step 3: Choose Evaluation Metrics
Choose the evaluation metric. The default is the "Accuracy" metric, which is suitable for most scenarios.
For prediction/scoring/voting scenarios — for instance, asking a model to score student essays — you can choose the "Scoring Consistency" metric.
#### About the "Accuracy" metric:
- When the test data includes an "Expected Output" (reference answer), the "Accuracy" metric defaults to: judging right or wrong only — when evaluating a model's response, it is either correct or incorrect, with no in-between score.
- When the test data does not include an "Expected Output" (reference answer), the "Accuracy" metric defaults to: a 5-point scale — when evaluating a model's response, it can score 1 to 5 points; 5 means perfect, fully correct; 1 is the lowest, meaning completely wrong.

### (4) Step 4: Add Data
Add the previously prepared test data to the form one by one. (A file upload feature will be made available later.)

### (5) Step 5: Evaluation Results
Click submit, and the page will automatically jump to the task detail page at https://nonelinear.com/static/task-result.html?task_id=rele-weekly-ranking/summary-one-domain ,
where you can view execution progress in real time. Finally, you'll see results like the following: including each model's final score, cost, time, etc. You can then make a comprehensive assessment to choose the most suitable model.
![link](img/评测结果-表格总结.png)

### (6) Step 6: Evaluation Details
On the task detail page, in the [Evaluation Results] section, click [View Details] to enter https://nonelinear.com/static/evaldetail.html?task_id=rele-weekly-ranking/summary-one-domain ,
where you can view each model's individual responses and specific scores. You can also filter to see which test cases and which models produced poor responses.
If you find that the system's automatic scoring does not match your standards, you can modify the score yourself; once modified, the corresponding model's overall score will be automatically updated in the backend.
![link](img/模型输出及评分详情-表格总结.png)
