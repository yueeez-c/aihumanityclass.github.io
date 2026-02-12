+++
date = "07 Feb 2026"
draft = false
title = "Class 7: AI Bias and Interpretability"
author = "Team 1"
+++

**Blogging Team 1**: Tristan Grubbs, Srikar Bangaru, Sarah Francis, Amanda Appiah-Yeboah, Matthew Janicki 

# News: NVIDIA and OpenAI Deal
**Presented by Team 5: [Slides](https://docs.google.com/presentation/d/1iUzFexFYTxOdhoC3TIZbh1jgBCxOLOZ77IoRRidUr0g/edit?slide=id.g378a603d89a_0_520#slide=id.g378a603d89a_0_520)**

## Articles

- Down, A., & Milmo, D. (2026, February 5). [_What does the disappearance of a $100bn deal mean for the AI economy?_](https://www.theguardian.com/technology/2026/feb/05/disapperance-100bn-deal-ai-circular-economy-funding-nvidia-openai). The Guardian. 

- Aubrey, K. (2026, January 5). [_Inside the Nvidia Rubin platform: Six new chips, one AI supercomputer_](https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/). NVIDIA Technical Blog. 

## Discussion

Team 5 started class by talking about how the original deal between NVIDIA and OpenAI had broken down. The current deal stands closer to 20 billion being invested into OpenAI, a far cry from the original 100 billion. Separately, NVIDIA has been hedging its bets elsewhere with a 10 billion dollar deal with OpenAI competitor Anthropic. This is part of a larger trend in the world of AI, where companies in the space are making large investments in each other to fund the capital-intensive industry. This circular investing has clouded the current investment picture, making it seem like there is more money in the industry than there actually is.

<center>
<img src="/images/nvidia.png" width=60% alt=""></img><br>
Source: <a href="https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/">nVIDIA</a>
</center>

Due to the current nature of the industry, talks of an “AI bubble” in the market have been growing. Bubble believers like Michael Burry, the famed predictor of the real estate bubble, argue that the meteoric rise of the AI market and its large investments, while showing little revenue, is indicative of a bubble. However, optimists argue that national competition and corporate strategy justify the industry’s growth.

Besides the NVIDIA and OpenAI deal, other market leaders are moving forward with AI at the forefront of their future. Google is doubling its AI spending to 185 billion after stronger than expected earnings. Elon Musk’s SpaceX has bought xAI (also founded by Elon Musk), creating a 1.25 trillion dollar company, which could be one of the largest IPOs ever in the near future. Both sides of the conversation claim these events support their view of the future of the AI industry, which goes to show the unpredictability of the industry’s future.


# Lead: AI Bias and Interpretability

**Presented by Team 9: [Slides](https://docs.google.com/presentation/d/1MAlhsWZtCgzTyqjP-g15MuEG-kev8lhvWcV-t65bVAA/edit?usp=sharing)**

## Readings

- Kyra Wilson and Aylin Caliskan. [_Gender, Race, and Intersectional Bias in Resume Screening via Language Model Retrieval_](https://ojs.aaai.org/index.php/AIES/article/view/31748/33915). AAAI/ACM Conference on AI, Ethics, and Society (AIES2024). [https://ojs.aaai.org/index.php/AIES/article/view/31748/33915](https://ojs.aaai.org/index.php/AIES/article/view/31748/33915)

- Chapter 3: Classification from Solon Barocas, Moritz Hardt, Arvind Narayanan. Fairness and machine learning: Limitations and Opportunities (“FairML book”). MIT Press, 2023. (The full book is openly available at https://fairmlbook.org)].) [https://fairmlbook.org/classification.html](https://fairmlbook.org/classification.html)

## Discussion

Team 9 continued discussions, highlighting the discrepancies that exist in hiring systems, which are only worsened with the deployment of AI. 

[Kyra Wilson](https://kyrawilson.github.io/me/about/), a PhD candidate, and [Aylin Caliskan]((https://faculty.washington.edu/aylin/)), an Assoc. Professor from the University of Washington, both work in LLM and NLP research. Their research article, [_Gender, Race, and Intersectional Bias in Resume Screening via Language Model Retrieval_](https://ojs.aaai.org/index.php/AIES/article/view/31748/33915), focuses on hiring tools that leverage technologies such as LLMs and NLP.

While AI screening-systems may be seemingly faster and more efficient, the authors investigated to see whether the efficiency comes at the cost of biases. As part of their results, the researchers found strong evidence for biases in AI-driven systems. They highlighted that resumes with white-sounding names were preferred approximately 85.1% of the time, while female candidates were preferred only about 11.1% of the time, and Black male candidates were disadvantaged nearly 100% of the time. 

Interestingly though, when the name on the resume was changed, but qualifications were kept the exact same, the outcome was flipped. This is key because it showed that the AI-screening tool would rank and sort based on proxies like names and other racial or gender cues, as compared to qualifications or real merit. Furthermore, changing the frequency of certain names in the training corpus showed a change in bias direction, showing how the training data directly influences screening-model behaviors.

In light of these findings, Team 9 prompted the class to discuss “What is Bias?” and “What is fairness?”. These questions were interesting as the class discussed how to define these terms, as well as whether fairness is possible in these systems at all.

The group listed the official definition of fairness as “equal treatment across groups,” and went on to share an example of racial bias in software used in the justice system. They went on to discuss how removing race on its own is insufficient to guarantee fairness, as other factors serve as proxies to race. The discussion was then turned to the class, where we further broke down our perspectives on fairness and bias, both in the world and within AI systems. 

Many of the discussions centered around the possibility of fairness and creating unbiased systems in an inherently biased world with inherently biased judges. Additionally, the idea of “fair” treatment not necessarily appearing “equal” for everyone also arose,  and how bias in AI may come into play when determining essentially “who gets what”. The question of whether we should first address bias in the world or bias in AI systems, and the majority of the class agreed to first address bias in the world, as AI systems are trained on biased data that exists in the world.

Furthermore, the concept of fairness from a statistical lens was also introduced. The group broke down statistical fairness in classification into three parts: independence, when groups have equal acceptance rates, separation, when groups face similar errors, and sufficiency, when predicted outcomes face the same probability across groups.  

Lastly, the class discussion ended on a broader look at several of the domains currently utilizing AI systems that are affected by AI bias. These domains include healthcare, criminal justice, finance, education, and employment. Overall, it was generally agreed upon that AI has tangible benefits for these domains, but also poses serious risks due to bias, and it is becoming increasingly important to consider bias and understand how it may be impacting our AI systems before mass implementing them.

<center>
<img src="/images/bias.png" width=60% alt=""></img>
</center>

# Additional Sources found by Team 9 for Dicussion:

- Aka, A., Palikot, E., Ansari, A., & Yazdani, N. (2025). Better together: Quantifying the benefits of AI-assisted recruitment. arXiv.[https://doi.org/10.48550/arXiv.2507.08029](https://doi.org/10.48550/arXiv.2507.08029)
- Academy of Management. (2025). Symposium session. Academy of Management Proceedings. [https://doi.org/10.5465/AMPROC.2025.15911symposium](https://doi.org/10.5465/AMPROC.2025.15911symposium)
- National Center for Biotechnology Information. (n.d.). Article PMC12823528. PubMed Central.[https://pmc.ncbi.nlm.nih.gov/articles/PMC12823528/](https://pmc.ncbi.nlm.nih.gov/articles/PMC12823528/)
   ProPublica. (2016, May 23). Machine bias: There’s software used across the country to predict future criminals. And it’s biased against Blacks.[https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing) 
- Barocas, S., Hardt, M., & Narayanan, A. (n.d.). Classification. In Fairness and machine learning [https://fairmlbook.org/classification.html](https://fairmlbook.org/classification.html)
- Kevin Connolly. [Recruiter Productivity | 2025 Talent Trends Report](https://www.ashbyhq.com/talent-trends-report/reports/2023-recruiter-productivity-trends-report). Ashby, 2023.
- Associated Press. [_Civil rights agency drops a key tool used to investigate workplace discrimination_](https://apnews.com/article/trump-discrimination-ai-eeoc-disparate-impact-a2e8aba11f3d3f095df95d488c6b3c40). 30 September 2025.
