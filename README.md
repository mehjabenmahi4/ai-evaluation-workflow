# AI Evaluation Workflow

An automated pipeline that tests AI output quality across multiple 
metrics — ensuring reliable and consistent AI performance at scale.

## Demo

[Watch the demo](https://www.youtube.com/watch?v=ciFt8whU94A)

## How It Works

1. Dataset trigger fetches each row and passes it to the AI Agent
2. AI Agent generates a response using OpenAI Chat Model
3. Response is evaluated across three parallel metrics:
   - Correctness — checks factual accuracy of the output
   - Helpfulness — measures relevance and usefulness
   - String Similarity — compares output against expected answer
4. All metric scores are collected and set as final Evaluation output

## Tools Used

- n8n
- OpenAI Chat Model
- Correctness Metric
- Helpfulness Metric
- String Similarity Metric
- n8n Evaluation (setoutputs)
