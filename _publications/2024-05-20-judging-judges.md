---
title: "Judging the Judges: Evaluating Alignment and Vulnerabilities in LLMs-as-Judges"
collection: publications
permalink: /publication/2025-07-01-judging-judges
excerpt: 'A comprehensive study of the LLM-as-a-judge paradigm in a controlled setup that reveals new results about its strengths and weaknesses.'
date: 2025-07-01
venue: 'Workshop on Generation, Evaluation and Metrics (GEM²)'
---

{% include figure image_path="images/assets/publications/judging-judges/judge-score-alignment.png"
alt="Judge alignment chart" caption="(Left) Scores assigned by different judge LLMs to different exam-taker
LLMs. (Right) Alignment scores of different judges with human annotation." %}

Offering a promising solution to the scalability challenges associated with human evaluation, the LLM-as-a-judge
paradigm is rapidly gaining traction as an approach to evaluating large language models (LLMs). However, there are
still many open questions about the strengths and weaknesses of this paradigm, and what potential biases it may hold.
In this paper, we present a comprehensive study of the performance of various LLMs acting as judges. We leverage
TriviaQA as a benchmark for assessing objective knowledge reasoning of LLMs and evaluate them alongside human
annotations which we found to have a high inter-annotator agreement. Our study includes 9 judge models and 9 exam
taker models -- both base and instruction-tuned. We assess the judge model's alignment across different model sizes,
families, and judge prompts. Among other results, our research rediscovers the importance of using Cohen's kappa as a
metric of alignment as opposed to simple percent agreement, showing that judges with high percent agreement can still
assign vastly different scores. We find that both Llama-3 70B and GPT-4 Turbo have an excellent alignment with humans,
but in terms of ranking exam taker models, they are outperformed by both JudgeLM-7B and the lexical judge Contains,
which have up to 34 points lower human alignment. Through error analysis and various other studies, including the
effects of instruction length and leniency bias, we hope to provide valuable lessons for using LLMs as judges in
the future.

Accepted at the [Workshop on Generation, Evaluation and Metrics (GEM²)](https://aclanthology.org/volumes/2025.gem-1/), 2025.

[Paper](https://aclanthology.org/2025.gem-1.33.pdf){:target="_blank" rel="noopener noreferrer"} \|
[Code](https://github.com/judging-judges/judging-judges){:target="_blank" rel="noopener noreferrer"}

Cite as:

{% raw %}
```bibtex
@inproceedings{thakur-etal-2025-judging,
    title = "Judging the Judges: Evaluating Alignment and Vulnerabilities in {LLM}s-as-Judges",
    author = "Thakur, Aman Singh  and
      Choudhary, Kartik  and
      Ramayapally, Venkat Srinik  and
      Vaidyanathan, Sankaran  and
      Hupkes, Dieuwke",
    booktitle = "Proceedings of the Fourth Workshop on Generation, Evaluation and Metrics (GEM{\texttwosuperior})",
    month = jul,
    year = "2025",
    address = "Vienna, Austria and virtual meeting",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.gem-1.33/",
    pages = "404--430",
    ISBN = "979-8-89176-261-9"
}
```
{% endraw %}
