+++
title = "Class 10: AI & Software Development"
author = "Aaryan Asthana, Jason Chin, Sarah Petchel, Taylor Petrofski, Katherine Anne Rukavina"
date = "2026-02-17"
+++


**Blogging Team [4]**: Aaryan Asthana, Jason Chin, Sarah Petchel, Taylor Petrofski, Katherine Anne Rukavina

## News: The Filipino Workers at the Sharp End of AI

**Presented by Team 8**: [Slides](https://myuva-my.sharepoint.com/:p:/g/personal/ysx7nx_virginia_edu/IQBny3KwaXbrTrw2aOMtKqg8Adot8WQGXez-xnxs2HsFFxo?e=CLeC74)

### Articles Discussed

1. Simon, T. (2025, April 24). [_The Filipino workers at the sharp end of artificial intelligence_](https://www.equaltimes.org/the-filipino-workers-at-the-sharp)). Equal Times.  
  
2. Vyas, I. (2025, May 27). [_IT Outsourcing Statistics in 2025: Top Countries & Their Market Share._](https://citrusbug.com/blog/it-outsourcing-statistics-2025/). Citrusbugtechnolabs.

## Discussion: Outsourcing Intelligence: The Human Cost of AI Development

Team 8 began class with a discussion of the often invisible human labor that powers AI systems. The news presentation focused on an Equal Times article that reports on data labelers in the Philippines. These workers are performing repetitive tasks to train AI models, such as identifying objects in images, much like the reCAPTCHA systems many of us often encounter. 

Team 8 featured several quotes from workers describing the conditions they face in these roles. “I work between 8 and 10 hours per day for an average of €6,” says Junbee, 22, from one of Cagayan de Oro’s slums. Another worker, John-Henry, said, “The alternative is selling drugs. But I want a future.”

<center><img src="/images/cagayan.png" width=50% alt=""></img><br>

*Figure 1: Remotasks employees annotate data in a building rented by the company in Cagayan de Oro.
Photo by Théophile Simon via Equal Times*
</center>

Team 8 introduced the author, Théophile Simon, a French freelance journalist who has focused on human rights and the ethics of AI since 2023. They also pointed out that Equal Times is a publication that covers labor rights and social justice issues globally. 

Team 8 then transitioned to positioning AI outsourcing in the context of neocolonialism, which is the idea that wealthy nations exert control over developing countries through economic rather than political means. Interestingly, they explained that data has replaced raw materials as the resource being extracted. The risk and harm of content moderation and data labeling is outsourced to workers in the Global South, while the value generated is felt by tech companies in wealthy nations. They noted that 70% of companies confirm outsourcing is more economical, and 92% of G2000 companies utilize IT outsourcing services. The Philippines holds 13.5% of the global outsourcing market.

Particularly disturbing was the discussion of content moderation work, where workers must view traumatic content, such as violence and sexual assault, in order to train AI systems to recognize and filter such material. These workers are being paid wages below the legal minimum to complete tasks that carry a psychological toll.

---

**Discussion Question 1:** _Does intense AI competition make exploitation inevitable by disadvantaging companies that pay fair wages for data annotation?_

The class had differing perspectives. One point argued that exploitation is endemic across industries and that companies always try to accomplish as much as possible for as little cost as possible. The asynchronous, remote nature of data labeling work makes exploitation even easier since workers are isolated and invisible. However, another point suggested that the size and influence of major AI companies could actually shift industry norms. They used Patagonia as an example of a company that has successfully marketed themselves on ethical sourcing, so consumers are willing to pay their relatively higher prices. 


---

**Discussion Question 2:** _Would you pay more for an AI service if the workers were fairly compensated?_

Responses were mixed. Some said yes, but one point pushed back: “I say no because it should just be the baseline. Why do these externalities fall on the consumer?” Team 8 mentioned that Congress has written to Silicon Valley companies about labor conditions suggesting the pressure should be on companies to fix the source rather than making ethics optional for consumers. 

A practical challenge was also considered. How do you actually verify whether AI labor is ethically sourced? While bad conditions tend to surface through investigative reports, transparency about good practices is harder to confirm. 


---

**Discussion Question 3:** _Human cost of content moderation?_ + Professor Evan's Take

The last part of the discussion examined the human cost of content moderation. One point noted it’s a necessary job because someone has to ensure AI systems have guardrails for all users. Another point compared the role to similar positions in law enforcement, where investigators must review disturbing material and often don’t last long due to the mental health impact. Team 8 finished the discussion with a reflection question: _Would we accept these conditions if we asked Americans to do the same work?_

Professor Evans’s Perspective

Prof. Evans offered a nuanced take, comparing the situation to fast fashion and noting that the existence of air-conditioned offices for this work in countries like the Philippines actually represents a form of progress because these nations have developed enough economically to provide such facilities. While not dismissing the ethical concerns, he suggested viewing it as part of a broader economic trajectory. 

---

## Lead Topic: AI & Software Development

**Presented by Team 12**  
[Slides](https://docs.google.com/presentation/d/1FvILCVohiEfrdVzS9K-zw9Lsb0KNE6xCdJvMltYJxdI/edit?usp=sharing)

**Reading:**

- Joel Becker, Nate Rush, Elizabeth Barnes, David Rein. Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity. July 2025. https://arxiv.org/abs/2507.09089
- Agnia Sergeyuk, Eric Huang, Dariia Karaeva, Anastasiia Serova, Yaroslav Golubev, Iftekhar Ahmed. Evolving with AI: A Longitudinal Analysis of Developer Logs. International Conference on Software Engineering (ICSE), 2026. https://arxiv.org/abs/2601.10258  

## Overview

Team 12 started their presentation by walking through the history of software development, from machine-level code in the 1940s through the introduction of high-level programming languages, the internet era, and into today’s world of machine learning and cloud computing. They then turned to the growing popularity of AI coding tools, showing Google Trends data from GitHub Copilot since its announcement, which had a clear upward trajectory. 

Team 12 then did a live demonstration for the class using Cursor Pro to write a Rust program that would prompt Google’s Gemini API and print the response to the console. The demo pointed out an important security concern to pay attention to: storing an AI key directly in the source versus storing it securely as an environmental variable. Prof. Evans mentioned that companies have systems in place to detect and disable leaked API keys.

This led Team 12 into describing the details of the METR paper, a randomized controlled trial measuring how AI tools affect the productivity of experienced open-source developers. The study examined 16 experienced developers who worked on real tasks from their own repositories, with each task randomly assigned to either allow or disallow AI tools. 

The results were surprising. Before starting, developers predicted AI would speed them up by 24%. After completing the study, they believed AI had sped them up by 20%. However, the data showed the opposite: developers took 19% longer when using AI tools. Team 12 emphasized that this study used real tasks and not artificial lab experiments and focused on experienced developers working in codebases they were familiar with. 

<center>
<img src="/images/screenrec.png" width="60%" alt="">

*Figure 2: Source: https://arxiv.org/abs/2507.09089*
</center>

Team 12 offered their interpretation that when a developer has been working on a codebase for years, they’re more familiar with it than AI could be. Waiting for AI responses takes time, and reviewing AI-generated code for correctness adds overhead that may not pay off when the developer already knows what to do. 

They also discussed the second paper and explained how it used a longitudinal approach. It tracked AI tool usage over two years with 400 AI users and 400 non-users. The survey results showed that 71% of developers were satisfied with AI tools, and 61.3% reported increased reliance over time. The main takeaway is that AI tools don’t replace developer work, rather, they restructure it. Developers spend less time writing code from scratch and more time on verification and integration. 


---

**Discussion Question :** _Are people overestimating AI’s contribution to software development?_

One point argued that software developers still need intimate knowledge of what they’re coding. Even as models improve, they’re imperfect, and developers need to be able to fix mistakes. AI might make the initial process quicker but it can make later stages more tedious because the generated code isn’t always accurate. 


The discussion then shifted to whether AI tools might improve with access to more context. If an AI agent sifts through everything on your computer, it will likely then know more about the codebase than even the experienced developer knows. However, tools like Claude Code are not yet that advanced. 

Technical skill was a recurring theme in the discussion. One point included an analogy: AI can teach you how to build a car, but understanding the importance of the seatbelt still requires expertise. In other words, the quality of the AI output depends significantly on the skill of the person prompting it. 

The class also discussed whether tools struggle with large and complex codebases. Team 12 agreed this was a limitation as AI tools seem to perform better on smaller projects than on massive repositories.  

When will AI actually replace software developers? The class seemed to agree that it won’t be until AI is essentially perfect. Until then, human expertise remains essential for debugging and understanding the broader context of what software needs to accomplish. 


---

## Additional References

Additional Sources

Bean, R. and Davenport, T. H. (2026, January 6). Five Trends in AI and Data Science for 2026. MIT Sloan Management Review. https://sloanreview.mit.edu/article/five-trends-in-ai-and-data-science-for-2026/ 

GeeksforGeeks. (2023, November 8). Evolution of Software Development. GeeksforGeeks. https://www.geeksforgeeks.org/software-engineering/evolution-of-software-development-history-phases-and-future-trends/ 

(2025). Stanford.edu. https://hai.stanford.edu/ai-index/2025-ai-index-report/public-opinion


