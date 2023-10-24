# GPT API Cost Estimation for Enterprises

_By rUv, CTO Generative AI, EY Americas

## HTML OpenAi Cost Estimator
https://ruvnet.github.io/openai-cost-estimator

## Purpose

This document aims to provide a structured approach to estimating the costs associated with using OpenAI's GPT models in an enterprise setting. It covers various factors and formulas to offer a comprehensive view of potential costs.

### Understanding Token Costs

The primary driver for costs in OpenAI deployments is token usage. Tokens can be as short as one character or as long as one word. Costs are incurred for both input and output tokens.

**Formula:**

```
Total Token Cost = (Input Tokens + Output Tokens) x Cost per Token
```
---

### Deployment Costs

Deploying the GPT-4 API, for instance, involves costs based on the number of requests and the tokens per request.

**Formula:**

```
Deployment Cost = Requests per Day x Days per Month x (Average Input Tokens per Request + Average Output Tokens per Request) x Cost per Token
```

---

### Fine-tuning Costs (GPT-3.5 Only)

Fine-tuning GPT-3.5 with your specific data involves a one-time training cost and ongoing usage costs for input/output tokens.

**Formula:**
```
Training Cost = Dataset Size x Training Epochs x Cost per Token for Training
```
```
Monthly Usage Cost = (Daily Input Tokens + Daily Output Tokens) x Days of Operation per Month x Cost per Token for Usage
```

---

### Ongoing Interaction Costs

For applications requiring continuous interaction with the GPT API (intelligent agents, etc.), the frequency of interaction and average tokens per interaction should be estimated.

**Formula:**

```
Ongoing Interaction Cost = Number of Applications x Frequency of Interaction x Average Tokens per Interaction x Cost per Token
```

---

### Additional Considerations

- Be aware of the assumptions you make, such as average token count, as actual usage may vary.
- Consider the context size (8K or 32K) when deploying GPT-4 as it impacts the cost per token.
- Account for any potential increase in usage over time.

