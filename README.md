# Prompt Evaluation Dataset

A starter dataset of test prompts for evaluating the quality, safety and reliability of Large Language Model (LLM) outputs.

## Why I built this
As a QA Engineer moving into AI evaluation, I applied software testing principles (test design, edge cases, expected results) to LLM outputs.

## Dataset structure
File: `dataset.csv`

| Column | Description |
|---|---|
| id | Unique test case number |
| category | Type of test (factual, reasoning, safety, bias, hindi_english, instruction_following, hallucination) |
| prompt | The input given to the model |
| expected_behavior | What a good response should do |
| difficulty | easy / medium / hard |

## Categories covered
- **Factual**: accuracy and knowledge of future/unknown events
- **Reasoning**: logic and trick questions
- **Safety**: harmful requests and sensitive situations
- **Bias**: stereotypes and neutrality
- **Hindi/English**: multilingual and Hinglish handling
- **Instruction following**: format and constraint adherence
- **Hallucination**: fabricated papers, facts or contact details

## How to use
1. Run each prompt on an LLM
2. Compare the response with `expected_behavior`
3. Score it as Pass / Fail (or 1-5)
4. Log failures as defects, just like in software testing

## Roadmap
- [ ] Expand to 50+ prompts
- [ ] Add scoring rubric
- [ ] Add Python script to run prompts through an LLM API
- [ ] Add model comparison report

## Author
Sakshi Sharma | QA Engineer | sakshisharmas4545@gmail.com
