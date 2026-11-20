# KhataPe Lending Decisions: Direct Answers vs Chain-of-Thought Prompting


**A FinTech case study on when AI can give a quick answer and when it must show its working.**


Author: [Your Name] · BBA (FinTech), Chitkara Business School · Tool: [ChatGPT / Claude] · [Month Year]


## The case
**KhataPe** (fictional) is a digital lender in Indore that lends to kirana shops and students. Every month it must choose between two loan products with different interest rates, fees and default risk. As a Business Analyst, I tested whether AI can pick the more profitable option, and whether asking it to reason step by step makes it more reliable.


## The data
8 synthetic monthly scenarios created with AI, including 3 "trap" scenarios where the higher interest rate makes less profit and 1 tie. I calculated the correct answers myself in a spreadsheet before testing.


## Decision rule
Net return = Interest rate + Processing fee − Expected default − Cost of funds
Profit = Net return × Loan budget


## Approach
| Step | Prompt type | Task |
|---|---|---|
| 1 | Direct | Which option has the higher interest rate? |
| 2 | Direct | Which option makes more profit? (final answer only) |
| 3 | Chain-of-thought | Same decision, solved step by step |
| 4 | Chain-of-thought | One number changed: does the AI update every step? |


## Results
| Metric | Direct | Step by step |
|---|---|---|
| Correct choice (/8) | __ | __ |
| Correct profit figure (/8) | __ | __ |
| Trap scenarios correct (/3) | __ | __ |
| Working I could check | No | Yes |


## Key learnings
1. **A direct answer is enough for one-step questions:** [your finding]
2. **Step-by-step reasoning helps multi-step decisions:** [scenario IDs it fixed]
3. **Convincing is not the same as correct:** [one step that looked right but was wrong, or "none found"]
4. **What the numbers do not show:** [two non-financial factors]


## My recommendation to KhataPe
[2–3 lines: how KhataPe should use AI for this monthly decision, and what a human must still check]


## Skills shown
Prompt engineering · Chain-of-thought prompting · Synthetic data creation · Spreadsheet financial analysis · AI output verification · Lending business basics


## What I learned
- A direct prompt works well for simple, one-step questions.
- Chain-of-thought prompting makes AI show each step, so I can check its working instead of trusting one number.
- Step-by-step working can look convincing and still contain a wrong number, so every step must be checked.
- How to create synthetic business scenarios with AI, including deliberate "trap" cases.
- Why I calculate my own answer key in a spreadsheet before testing AI.
- Changing one number is a quick test of whether AI really reasons or just repeats.
- Numbers alone do not make a lending decision; risk and regulation matter too.


*KhataPe and all data in this project are fictional and created for learning.*
