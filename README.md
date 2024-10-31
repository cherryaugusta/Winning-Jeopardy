# Winning Jeopardy: A Statistical Analysis

This project is a solution for a guided project from Dataquest, originally titled ["Winning Jeopardy"](https://www.dataquest.io/projects/guided-project-a-winning-jeopardy/). I have completed and expanded upon the project to showcase my own statistical analysis and insights. This project is shared for educational and portfolio purposes only.

## Data Introduction

This analysis, titled **Winning Jeopardy**, focuses on the American TV show *Jeopardy*, a prominent part of U.S. popular culture known for its challenging trivia questions and cash prizes. The objective is to identify patterns within the questions that may provide contestants with a strategic advantage.

The dataset used for the analysis, `jeopardy.csv`, consists of 20,000 rows sampled from a comprehensive collection of Jeopardy questions. Each row represents a single question from a specific episode, reflecting the show's diverse and complex format. The dataset can be accessed at [this link https://www.reddit.com/r/datasets/comments/1uyd0t/200000_jeopardy_questions_in_a_json_file/). 

The dataset includes the following key columns:

- **Show Number**: A unique identifier for each Jeopardy episode.
- **Air Date**: The date when the episode was broadcast.
- **Round**: The round of Jeopardy during which the question was asked.
- **Category**: The thematic category of the question.
- **Value**: The monetary value awarded for a correct answer.
- **Question**: The text of the trivia question posed to the contestants.
- **Answer**: The correct response to the question.

The goal of this analysis is to uncover trends and insights that could inform strategies for succeeding on Jeopardy.

**Key Tools**: Python (Pandas, NumPy, Regular Expressions, Random, SciPy)

## Exploratory Data Analysis
### Recycled Questions
On average, the correct answer constitutes only about 6% of the total text of a question. This suggests that simply hearing a question is not sufficient to reliably identify the correct answer, indicating the need for study and preparation.

### Low-Value vs. High-Value Questions
Approximately 70% of the terms in new questions also appear in previous questions. This analysis is based on a limited sample and focuses on individual terms rather than entire phrases, which limits its significance. However, this overlap suggests that further exploration into the repetition of questions could provide useful insights.

## Chi-Squared Analysis
No notable differences in term usage were found between high-value and low-value questions. Furthermore, the chi-squared test's reliability is questionable, as all term frequencies were below 5. To improve the accuracy of this test, it would be beneficial to conduct the analysis using terms with higher frequencies.

## Conclusion

This analysis of Jeopardy questions reveals several key insights that could inform strategies for competing on the show. The high degree of term overlap between new and previous questions suggests that studying past questions may be beneficial. However, the limited difference in term usage between high-value and low-value questions implies that the complexity of Jeopardy questions may not significantly vary by monetary value, challenging the assumption that high-value questions are inherently more difficult.

While the chi-squared analysis did not produce strong conclusions due to low frequencies, future analyses could address this by focusing on more commonly used terms. Overall, a targeted study approach—particularly of recurring terms—appears to offer contestants a strategic advantage when preparing for Jeopardy.
