# Regex Generation: How to Choose the Most Suitable Model?

## 1. Prepare Test Data
As an example, we prepared 10 data items as follows: [Input] represents the model input (i.e., the prompt); [Expected Output] represents the reference answer.

### Sample 1
- [Input]: Write a regular expression to match Chinese mobile phone numbers (11 digits, starting with 1). The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```^1[3-9]\d{9}$```

### Sample 2
- [Input]: Write a regular expression to match a valid email address format. The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$```

### Sample 3
- [Input]: Write a regular expression to match an IPv4 address format. The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$```

### Sample 4
- [Input]: Write a regular expression to match a strong password (at least 8 characters, including uppercase and lowercase letters, digits, and special characters). The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*?&])[A-Za-z\d@$!%*?&]{8,}$```

### Sample 5
- [Input]: Write a regular expression to match a URL address (supporting http and https). The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```^https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)$```

### Sample 6
- [Input]: Write a regular expression to match HTML tags. The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```<[^>]+>```

### Sample 7
- [Input]: Write a regular expression to match Chinese characters. The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```[一-龥]+```

### Sample 8
- [Input]: Write a regular expression to match a bank card number (13-19 digits). The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```^\d{13,19}$```

### Sample 9
- [Input]: Write a regular expression to match a hexadecimal color code. The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```^#([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3})$```

### Sample 10
- [Input]: Write a regular expression to match a MAC address format. The output format should be a pure regular expression, without any explanations. Example: matching letters and digits can be represented as [a-zA-Z0-9]

- [Expected Output]: ```^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$```


<br><br>
## 2. Create a Model Selection Evaluation Task
First, open the task creation page at https://nonelinear.com/static/task-create.html.

### (1) Step 1: Set the Task ID
Enter a Task ID — the unique identifier of the task. Once created, it cannot be modified. Here, based on the specific task, we set it to: regix_eval.

### (2) Step 2: Choose Models
Choose the models you want to evaluate. The page provides a default "Curated Cost-Effective Models" list (ordered from highest to lowest cost-effectiveness; models lower in the list are relatively less effective but cheaper), as well as a "Flagship Models" list. Of course, you can also click to view more models, with support for filtering by "thinking model or not", "open-source or not", and "domestic/foreign model". As an example, we selected four models: gpt-oss-120b, GLM-4.5-Flash-nothink, GLM-4.5-Flash, and Qwen3-8B:free.

### (3) Step 3: Choose Evaluation Metrics
Choose the evaluation metric. The default is the "Accuracy" metric, which is suitable for most scenarios.
For prediction/scoring/voting scenarios — for instance, asking a model to score student essays — you can choose the "Scoring Consistency" metric.
#### About the "Accuracy" metric:
- When the test data includes an "Expected Output" (reference answer), the "Accuracy" metric defaults to: judging right or wrong only — when evaluating a model's response, it is either correct or incorrect, with no in-between score.
- When the test data does not include an "Expected Output" (reference answer), the "Accuracy" metric defaults to: a 5-point scale — when evaluating a model's response, it can score 1 to 5 points; 5 means perfect, fully correct; 1 is the lowest, meaning completely wrong.

### (4) Step 4: Add Data
Add the previously prepared test data to the form one by one. (A file upload feature will be made available later.)

### (5) Step 5: Evaluation Results
Click submit, and the page will automatically jump to the task detail page at https://nonelinear.com/static/task-result.html?task_id=regix_eval , where you can view execution progress in real time. Finally, you'll see results like the following: including each model's final score, cost, time, etc. You can then make a comprehensive assessment to choose the most suitable model.
![link](img/评测结果-regex.png)

### (6) Step 6: Evaluation Details
On the task detail page, in the [Evaluation Results] section, click [View Details] to enter https://nonelinear.com/static/evaldetail.html?task_id=regix_eval , where you can view each model's individual responses and specific scores. You can also filter to see which test cases and which models produced poor responses. If you find that the system's automatic scoring does not match your standards, you can modify the score yourself; once modified, the corresponding model's overall score will be automatically updated in the backend.
![link](img/模型输出及评分详情-regex.png)
