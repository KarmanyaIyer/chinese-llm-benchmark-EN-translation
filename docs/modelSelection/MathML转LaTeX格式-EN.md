# MathML to LaTeX Format Conversion: How to Choose the Most Suitable Model?
Want to instantly convert MathML to LaTeX but worried that the model will "mess up"? Don't worry — this hands-on guide will help you finalize your model selection in 10 minutes!
We've prepared 10 typical formulas, ranging from x=5 to ∫₀^∞, covering high-frequency scenarios such as superscripts, fractions, square roots, and integrals; we score them strictly using the "accuracy" metric.
The entire process requires zero code — just five clicks on https://nonelinear.com and the cost, time, and score are at a glance!
Once you've read this, you'll know which model offers the best value for money. Your mom will never have to worry about your formula conversions again~ (Preface written by kimi-k2)

## 1. Prepare Test Data
As an example, we prepared 10 data items as follows: [Input] represents the model input (i.e., the prompt); [Expected Output] represents the reference answer.
### Sample 1
[Input]: Please convert the following MathML code to LaTeX format: ```<math><mi>x</mi><mo>=</mo><mn>5</mn></math>```

[Expected Output]: ```x = 5```

### Sample 2
[Input]: Please convert the following MathML code to LaTeX format: ```<math><mi>x</mi><mo>+</mo><mi>y</mi><mo>=</mo><mn>10</mn></math>```

[Expected Output]: ```x + y = 10```

### Sample 3
[Input]: Please convert the following MathML code to LaTeX format: ```<math><msup><mi>x</mi><mn>2</mn></msup></math>```

[Expected Output]: ```x^2```

### Sample 4
[Input]: Please convert the following MathML code to LaTeX format: ```<math><mfrac><mi>a</mi><mi>b</mi></mfrac></math>```

[Expected Output]: ```\frac{a}{b}```

### Sample 5
[Input]: Please convert the following MathML code to LaTeX format: ```<math><msqrt><mi>x</mi></msqrt></math>```

[Expected Output]: ```\sqrt{x}```

### Sample 6
[Input]: Please convert the following MathML code to LaTeX format: ```<math><msub><mi>x</mi><mn>1</mn></msub></math>```

[Expected Output]: ```x_1```

### Sample 7
[Input]: Please convert the following MathML code to LaTeX format: ```<math><mfrac><msup><mi>x</mi><mn>2</mn></msup><mn>4</mn></mfrac></math>```

[Expected Output]: ```\frac{x^2}{4}```

### Sample 8
[Input]: Please convert the following MathML code to LaTeX format: ```<math><mfrac><mn>1</mn><msqrt><mn>2</mn><mi>π</mi></msqrt></mfrac></math>```

[Expected Output]: ```\frac{1}{\sqrt{2\pi}}```

### Sample 9
[Input]: Please convert the following MathML code to LaTeX format: ```<math><msup><mi>e</mi><mrow><mo>-</mo><msup><mi>x</mi><mn>2</mn></msup></mrow></msup></math>```

[Expected Output]: ```e^{-x^2}```

### Sample 10
[Input]: Please convert the following MathML code to LaTeX format: ```<math><msubsup><mo>∫</mo><mn>0</mn><mi>∞</mi></msubsup><mi>f</mi><mo>(</mo><mi>x</mi><mo>)</mo><mi>dx</mi></math>```

[Expected Output]: ```\int_{0}^{\infty} f(x) dx```


<br><br>
## 2. Create a Model Selection Evaluation Task
First, open the task creation page at https://nonelinear.com/static/task-create.html.
### (1) Step 1: Set the Task ID
Enter a Task ID — the unique identifier of the task. Once created, it cannot be modified. Here, based on the specific task, we set it to: mml2latex2.

### (2) Step 2: Choose Models
Choose the models you want to evaluate. The page provides a default "Curated Cost-Effective Models" list (ordered from highest to lowest cost-effectiveness; models lower in the list are relatively less effective but cheaper), as well as a "Flagship Models" list. Of course, you can also click to view more models, with support for filtering by "thinking model or not", "open-source or not", and "domestic/foreign model". As an example, we selected two models: GLM-4.5-Flash-nothink and Qwen3-8B:free.

### (3) Step 3: Choose Evaluation Metrics
Choose the evaluation metric. The default is the "Accuracy" metric, which is suitable for most scenarios.
For prediction/scoring/voting scenarios — for instance, asking a model to score student essays — you can choose the "Scoring Consistency" metric.
#### About the "Accuracy" metric:
- When the test data includes an "Expected Output" (reference answer), the "Accuracy" metric defaults to: judging right or wrong only — when evaluating a model's response, it is either correct or incorrect, with no in-between score.
- When the test data does not include an "Expected Output" (reference answer), the "Accuracy" metric defaults to: a 5-point scale — when evaluating a model's response, it can score 1 to 5 points; 5 means perfect, fully correct; 1 is the lowest, meaning completely wrong.

### (4) Step 4: Add Data
Add the previously prepared test data to the form one by one. (A file upload feature will be made available later.)

### (5) Step 5: Evaluation Results
Click submit, and the page will automatically jump to the task detail page at https://nonelinear.com/static/task-result.html?task_id=mml2latex2 , where you can view execution progress in real time. Finally, you'll see results like the following: including each model's final score, cost, time, etc. You can then make a comprehensive assessment to choose the most suitable model.
![link](img/评测结果-mathml.png)

### (6) Step 6: Evaluation Details
On the task detail page, in the [Evaluation Results] section, click [View Details] to enter https://nonelinear.com/static/evaldetail.html?task_id=mml2latex2 , where you can view each model's individual responses and specific scores. You can also filter to see which test cases and which models produced poor responses. If you find that the system's automatic scoring does not match your standards, you can modify the score yourself; once modified, the corresponding model's overall score will be automatically updated in the backend.
![link](img/模型输出及评分详情-mathml.png)
