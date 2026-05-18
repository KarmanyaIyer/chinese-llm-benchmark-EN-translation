# E-commerce Review Sentiment Analysis: How to Choose the Most Suitable Model?
In the e-commerce era, user reviews flood in like a tide, and the sentiment they carry directly affects brand reputation and sales.
How to efficiently and accurately judge whether a review is a "recommendation" or a "warning" has become a must-have skill for operations and customer service.
Traditional manual labeling is costly and time-consuming, and while there are many models available, they vary widely in quality and price. (Preface written by kimi-k2)

This tutorial will walk you step-by-step through using 10 real review samples to launch a multi-model comparison evaluation on the nonelinear platform: from data preparation and metric selection to result interpretation, lock in the most cost-effective sentiment analysis model in 5 minutes, letting algorithms "read between the lines" for you, accelerating product page conversion and negative-review alerts.

## 1. Prepare Test Data
As an example, we prepared 10 data items as follows:
[Input] represents the model input (i.e., the prompt); [Expected Output] represents the reference answer.<br>
### Sample 1
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): The camera on this phone is truly amazing — night mode is especially clear, completely exceeding expectations!
  - [Expected Output]: Positive
### Sample 2
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): The quality is good, the price is reasonable, but the packaging is a bit shabby. Overall, it's okay.
  - [Expected Output]: Neutral
### Sample 3
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): It crashed twice within three days of use, and customer service was rude. The experience was terrible — I won't buy again.
  - [Expected Output]: Negative
### Sample 4
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): The headphones have great sound quality, the noise cancellation is effective, and they're especially comfortable to use during my commute. Recommended!
  - [Expected Output]: Positive
### Sample 5
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): Logistics was fast, the product is similar to the description, nothing special, but not disappointing either.
  - [Expected Output]: Neutral
### Sample 6
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): The color of the clothes is very different from the picture, and the material is rough. I feel deceived.
  - [Expected Output]: Negative
### Sample 7
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): This coffee machine is simple to operate, and the coffee it makes is rich and tasty. I use it every morning before work — it has greatly increased my happiness in life!
  - [Expected Output]: Positive
### Sample 8
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): I bought a massager for my mom; she says the intensity is just right and her neck and shoulders feel much more relaxed after using it. Great value for money.
  - [Expected Output]: Positive
### Sample 9
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): The product's basic functions work, but the instructions are unclear and setting it up is a bit troublesome.
  - [Expected Output]: Neutral
### Sample 10
  - [Input]: Judge the sentiment (Positive/Negative/Neutral): After fully charging the power bank, it could only charge the phone once before running out. The capacity is severely overstated — very disappointing.
  - [Expected Output]: Negative


<br><br>
## 2. Create a Model Selection Evaluation Task
First, open the task creation page at https://nonelinear.com/static/task-create.html.<br>
### (1) Step 1: Set the Task ID
Enter a Task ID — the unique identifier of the task. Once created, it cannot be modified. Here, based on the specific task, we set it to: product-review-sentiment.<br>

### (2) Step 2: Choose Models
Choose the models you want to evaluate. The page provides a default "Curated Cost-Effective Models" list (ordered from highest to lowest cost-effectiveness; models lower in the list are relatively less effective but cheaper), as well as a "Flagship Models" list.
Of course, you can also click to view more models, with support for filtering by "thinking model or not", "open-source or not", and "domestic/foreign model".
As an example, we selected five models: GLM-4.5-Flash-nothink, qwen-turbo-2025-07-15, Doubao-1.5-lite-32k-250115, Qwen3-8B:free, and gpt-5-mini-2025-08-07.
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
Click submit, and the page will automatically jump to the task detail page at https://nonelinear.com/static/task-result.html?task_id=product-review-sentiment ,
where you can view execution progress in real time. Finally, you'll see results like the following: including each model's final score, cost, time, etc. You can then make a comprehensive assessment to choose the most suitable model.
![link](img/评测结果.png)

### (6) Step 6: Evaluation Details
On the task detail page, in the [Evaluation Results] section, click [View Details] to enter https://nonelinear.com/static/evaldetail.html?task_id=product-review-sentiment ,
where you can view each model's individual responses and specific scores. You can also filter to see which test cases and which models produced poor responses.
If you find that the system's automatic scoring does not match your standards, you can modify the score yourself; once modified, the corresponding model's overall score will be automatically updated in the backend.
![link](img/模型输出及评分详情.png)
