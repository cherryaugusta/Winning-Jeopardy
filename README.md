# Winning Jeopardy: A Statistical Analysis
## Data Introduction

In this project, titled **Winning Jeopardy**, the focus is on analyzing the American TV show Jeopardy. This program, a notable fixture in U.S. popular culture, is well-known for its challenging trivia questions and the appeal of cash prizes. The objective is to identify patterns within the questions that may provide contestants with a strategic advantage.

The analysis utilizes a dataset named `jeopardy.csv`, which includes 20,000 rows sampled from a comprehensive collection of Jeopardy questions. Each row represents a single question from a specific episode of the show, reflecting the diverse and complex nature of the game's format. The dataset is available for download at [this link https://www.reddit.com/r/datasets/comments/1uyd0t/200000_jeopardy_questions_in_a_json_file/). 

The dataset includes the following key columns:

- **Show Number**: A unique identifier for each Jeopardy episode.
- **Air Date**: The date when the episode was broadcast.
- **Round**: The round of Jeopardy during which the question was asked.
- **Category**: The thematic category of the question.
- **Value**: The monetary value awarded for a correct answer.
- **Question**: The text of the trivia question posed to the contestants.
- **Answer**: The correct response to the question.

The goal of this analysis is to uncover trends and insights that could inform strategies for succeeding on Jeopardy.

## Exploratory Data Analysis
### Key Tools: Python (Pandas, NumPy, Regular Expressions, Random, SciPy)

### Recycled Questions
On average, the answer accounts for only about 6% of the question. This is a relatively small portion, suggesting that simply hearing a question isn't enough to reliably identify the correct answer. It implies that studying will likely be necessary.

### Low Value vs. High Value Questions
Approximately `70%` of the terms in new questions also appear in previous questions. This analysis is based on a limited sample and focuses on individual terms rather than entire phrases, making its significance somewhat limited. However, this overlap suggests that further exploration into the repetition of questions could be valuable.

## Chi-Squared Analysis
There were no notable differences in term usage between high-value and low-value rows. Additionally, the chi-squared test's reliability is uncertain because all frequencies were below `5`. It would be more suitable to perform this test again with terms that have higher frequencies.
