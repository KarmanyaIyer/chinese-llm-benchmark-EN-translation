 - Contains 2025 Gaokao (Chinese college entrance exam) papers from provinces and municipalities across China, covering 9 subjects. Data is grouped by subject — e.g., the Chinese JSON file contains all publicly released questions nationwide; the originating province/municipality is recorded in the `detail` field.
 - To simplify evaluation, we keep only plain-text objective questions. Questions with embedded images are deferred to a future "Multimodal Evaluation" section.
 - In the current version, the number of questions per subject is: Chinese 28, Math 108, English 33, Physics 59, Chemistry 41, Biology 80, History 68, Geography 19, Politics 77.

Sample item:
```
  {
    "prompt": "牡蛎、贻贝等双壳贝类环境适应性强，主要滤食浮游生物和有机颗粒，其生长过程中吸收并固定二氧化碳。福建省莆田市秀屿区是重要的双壳贝类养殖基地。近年来，莆田市持续开展海上养殖转型升级，引导海上养殖向生态化方向发展。2022年5月，福州市某企业出资20余万元，向秀屿区某水产养殖公司购买双壳贝类碳汇，用于抵消其生产经营活动中的碳排放，是全国首例双壳贝类碳汇交易。根据材料完成下面小题。\n\n扩大秀屿区牡蛎养殖碳汇量的有效措施是（ ）\n（A） 增加养殖品种\n（B） 降低企业碳排放\n（C） 改善养殖水质\n（D） 提升养殖单产水平\n",
    "reference": "D",
    "class": "2025高考地理",
    "id": "ReLE-5e9151632",
    "detail": "2025年辽宁、黑龙江、吉林、内蒙古普通高校选择性考试-地理-选择题-5"
  }
```

> **Note:** Question text (`prompt`) and Chinese metadata (`class`, `detail`) are intentionally kept in Chinese — these are tests of Chinese-language comprehension, so translating the questions would invalidate the benchmark. Translated metadata is provided in the companion `*-EN.json` files via `_en_meta` fields.

Field descriptions:
 - `prompt`: the question
 - `reference`: the reference answer
 - `class`: subject category (e.g. `2025高考地理` = 2025 Gaokao Geography)
 - `id`: unique identifier for the prompt
 - `detail`: supplementary information, such as the province/municipality the question came from
