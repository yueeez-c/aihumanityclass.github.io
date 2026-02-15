+++
date = "10 Feb 2026"
draft = true
title = "Class 8: AI Interpretability"
author = "Team 2"
+++

**Blogging Team 2**: Amelia Chen, Laxmi Ghanate, Ryan Russo, Shaurya Singh, Matthew Vu

# News: AI Super Bowl Ads
[Slides from Team 6](https://docs.google.com/presentation/d/1WXhtrGHppLSOi9YMIZsfHN_u1dNFpsJMddmC1Y3zVwA/edit?slide=id.g3c6c41f5f1b_0_21#slide=id.g3c6c41f5f1b_0_21) 

Team 6's news presentation highlighted AI Ads in the Super Bowl. An estimated 23% of ads in the Super Bowl were AI ads, indicative of AI companies (OpenAI, Anthropic, Google, Amazon/Ring, Meta) attempting to shed doubt through advertising. Two ads were completely AI generated, one by Svedka Vodka and another by Artlist, an AI toolkit for artists and creators. Evident in each of these advertisements are each company’s perspective: Anthropic/Claude conveys their guarantee of safety regulations and responsible scaling; Google displays its commitment to the White House risk-based approach to AI; Meta introduced their AI-supported Meta Glasses in disregard for the EU’s AI safety code of practice; Svedka claimed robots as a reminder to be pro-human; OpenAI demonstrated its desire for the further incorporation of AI in giving up stringent regulations.

Anthropic mocked ChatGPT’s style of speech in their [ad](https://www.youtube.com/watch?v=kQRu7DdTTVA) claiming that “Ads are coming to AI. But not to Claude.” Altman called the ad dishonest, arguing that having ChatGPT have a free tier with ads furthers AI access and user agency. Much of the public disapproved of Altman’s response, defending the point that Anthropic was making and explaining how Altman “inadvertently validated Anthropic as a serious threat” (Lichtenberg). The notion of chatbots running ads also sparked public discourse on human emotional reliance on chatbots, and whether the gains in information chatbots experience will be equivalently translated to people.

<center>
<img src="/images/anthropic_ad.png" width=60% alt="Anthropic Super Bowl Ad"></img><br>
<strong>Figure 1</strong>: Anthropic's Super Bowl Ad 

([Source](https://www.theverge.com/ai-artificial-intelligence/875563/anthropics-super-bowl-ad-has-a-change-that-made-it-less-directly-about-openai-and-chatgpt))
</center>

## Discussion
**Is Advertising a good approach to making AI affordable and accessible? What alternatives are there?**

In class, we discussed the point Sam Altman raised about AI ads potentially making AI more accessible. Some issues discussed with bringing ads to AI platforms or chatbots is that ads could reduce the credibility of these platforms. For example, there are ethical concerns when users do not know if something is an advertisement or not - something that has been found to be an issue on popular social media platforms. It could signal a shift of the priorities of large AI companies to lie with advertisers rather than users. 

One example a classmate brought up was of the citation website EasyBib where users are asked to watch ads in order to use the site free of charge. Students mentioned advertising does not have to be seen as an inherently bad thing if companies do not have alternatives, but it will be important in the future for AI companies to keep ads separate from their platforms.

**Is it ethical for AI companies to use advertising? Do these ads make AI feel like a tool we control, or have to accept?**

We discussed further the ethical implications of advertising in AI platforms. A classmate brought up the types of ads these platforms should distribute, and there are greater concerns with high-risk ads such as healthcare related advertisements. It could be problematic for a chatbot system that is well-trusted by a user to provide sponsored information on health and safety. In general, advertising could erode the public's trust in AI models. This point is especially important when considering the large amounts of personal data that could be shared with advertising companies working with AI companies.

# Main Topic: AI Interpretability
[Slides from Team 10](https://docs.google.com/presentation/d/1yQeRo0TUDMedH1S8M8NrI9meELuVGQR0g4lKDGUGM7w/edit?slide=id.p#slide=id.p) (Hannah Cohen, Hemanth Saravanan, Nurdin Hossain, Pranav Goteti, Ruizhang Chen)

## Discussion
Class 8’s main discussion centered around the paper “[Stop explaining black box machine learning models for high stakes decisions and use interpretable models instead](https://aihumanityclass.github.io/docs/rudin2019.pdf)” by Cynthia Rudin, published in Nature Machine Intelligence in 2019. Cynthia Rudin is a Computer Science professor at Duke University whose research focus is on interpretable ML and the application of models to high-stakes decision-making. She received the 2022 Association for the Advancement of Artificial Intelligence (AAAI) Squirrel AI Award, an award for promoting positive uses of AI.

To begin a discussion on AI interpretability, a consensus must be reached on the definition of interpretability. Rudin makes a distinction between interpretability and explainability:

| Interpretability                                                                                                                                               | Explainability                                                                                                                                       |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| Concerned with making the model *understandable* through *transparency* and *low complexity*. The goal is to *understand* the mechanics *before* the decision. | Concerned with obtaining an *explanation* of a model’s decision *after* it has been made. Characterized by *low transparency* and *high complexity*. |

Black box models are not interpretable, as there is no way to understand the full process between taking in input and producing output. A black box model that explains its thinking post-decision making is not a true window into its workings. Rudin argues that the use of black box models and reliance on explainability for legitimacy, particularly in high stakes decisions, holds great potential dangers. She advocates for the pivot to interpretable models entirely, which can still be powerful, with some examples being decision trees and regression models. Another example is found in another paper co-authored by Rudin, “[This Looks Like That: Deep Learning for Interpretable Image Recognition](https://arxiv.org/pdf/1806.10574),” in which the researchers introduce ProtoPNet (prototypical part network) for image classification, a deep network architecture that identifies and reasons through prototypical parts similarly to how humans would.

<center>
<img src="/images/protopnet.png" width=60% alt="ProtoPNet Reasoning Process"></img><br>
<strong>Figure 2</strong>: ProtoPNet learned prototypical parts for species classification 

([Source](https://arxiv.org/pdf/1806.10574))
</center>

The “lack of transparency and accountability” (Rudin 1) with black box models is evident in a few real world cases. Firstly, COMPAS: a proprietary software that is used to determine if inmates are eligible for parole. A 2016 ProPublica [article](https://www.propublica.org/article/how-we-analyzed-the-compas-recidivism-algorithm) reported that the model held biases concerning age and race: defendants under 25, black defendants, and female defendants were significantly more likely to be given a higher risk score (Larson et al.). Additionally, the model was ultimately unreliable in its forecasting of violent crime, as “only 20 percent of the people predicted to commit violent crimes actually went on to do so” (Angwin). Since COMPAS is a black box, there is no way of understanding why the model made these biases and unreliable predictions. 

<center>
<img src="/images/compas.png" width=40% alt="COMPAS Risk Scores"></img><br>
<strong>Figure 3</strong>: COMPAS Risk Scores + Real World Outcomes

([Source](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing))
</center>

Next, health insurance companies UnitedHealth Group and Cigna are facing class action lawsuits for their use of AI models in deciding medical claims. UnitedHealth Group is current facing a class action lawsuit for their use of a model called nH Predict in deciding medical claims. An [article](https://www.theguardian.com/us-news/2025/jan/25/health-insurers-ai) posted to TheGuardian writes that the lawsuit against UnitedHealth Group pertains to their model “nH Predict,” which was alleged to have a “90% error rate, meaning nine out of 10 denials are reversed upon appeal.” The lawsuit against Cigna alleged that “Cigna denied more than 300,000 claims in a two-month period, which amounts to about 1.2 seconds for each physician-reviewed claim” (Cameron). Companies refuse to turn over proprietary models, yet the reasoning behind these denied claims remains unknown behind black box models, leaving questions about AI’s role in giving people the healthcare they need (or lack thereof).

<center>
<img src="/images/claim_denial_rates.png" width=50% alt="Health Insurance Claim Denial Rates"></img><br>
<strong>Figure 4</strong>: Health Insurer Claim Denial Rates

([Source](https://axenehp.com/health-insurer-claim-denial-rates-kaiser-outlier/))
</center>

Given the potential harms of black box models, why is it that they are still stood behind? Possible reasons include corporate greed, ease of development, and the belief that black box models prevent “gaming” of the system and have the capability discover hidden patterns. Companies may not want to reveal their trade secrets, or developers may want to avoid the computationally hard problems and genuine understanding/optimization that comes with building interpretable models. Some argue in defense of the way black box models prevent users from understanding what the model is analyzing, since it prevents outcomes from being manipulated by users, however the ability to game an interpretable model simply makes transparent a problem that can be fixed. Lastly, there exists idea that the complexity of black box models enables them to discover hidden patterns humans can’t, although it is likely interpretable models have this same ability. 

Current AI regulation in both the EU and US illustrate the reluctance to condemn black box models. The EU AI Act classifies systems by risk, stipulating that high-risk systems and black box models are permitted with documentation, oversight, and testing. In the US, the Colorado AI Act permits black boxes as long as companies perform internal “Impact Assessments,” which do not get disclosed to the public. The NYC Local Law 144 is demands just slightly more transparency, requiring employers to public a public summary of bias audits for hiring algorithms.

<center>
<img src="/images/ai_risk.png" width=60% alt="EU AI Act Risk Pyramid"></img><br>
<strong>Figure 5</strong>: EU AI Act Risk Pyramid

([Source](https://www.nemko.com/blog/a-quick-dive-into-the-eu-ai-act))
</center>

## Discussion
**Do you think any of these reasons for using black box models over interpretable models are valid? Rudin argues they are not – but do you agree?**

The class discussed that although interpretable models sound ideal there is no viable alternative interpretable model that could replace current usage. Furthermore, it is hard to enforce Rudin's ideas for restricting black box models. This is demonstrated by the lack of current regulation on the topic.

**When do you think it is worth it to sacrifice interpretability for raw accuracy? Does that vary based on a model’s use case?**

It was brought up that different risk levels can determine the level of accountability. For example, in areas such as crime or healthcare greater human accountability should be taken on interpretability of models. A counterargument to this would be, why trust the interpretation if the model can produce a high raw accuracy? If models were predicting at 100% accuracy there may be less emphasis on understanding them despite biases or errors.

# Sources
Angwin, Julia, et al. _“Machine Bias — Risk Assessments in Criminal Sentencing.”_ _ProPublica_, 2016, [https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing). Accessed 12 February 2026.

Cameron, Dell. _“New AI Tool Counters Health Insurance Denials Decided by Automated Algorithms.”_ _The Guardian_, 25 Jan. 2025, [https://www.theguardian.com/us-news/2025/jan/25/health-insurers-ai](https://www.theguardian.com/us-news/2025/jan/25/health-insurers-ai). Accessed 12 February 2026.

Chen, Chaofan, et al. _“This Looks Like That: Deep Learning for Interpretable Image Recognition.”_ _arXiv_, 27 June 2018, [https://arxiv.org/pdf/1806.10574](https://arxiv.org/pdf/1806.10574). arXiv.org, Accessed 12 February 2026.

Larson, Jeff, Surya Mattu, Lauren Kirchner, and Julia Angwin. _“How We Analyzed the COMPAS Recidivism Algorithm.”_ _ProPublica_, 23 May 2016, [https://www.propublica.org/article/how-we-analyzed-the-compas-recidivism-algorithm](https://www.propublica.org/article/how-we-analyzed-the-compas-recidivism-algorithm). Accessed 12 February 2026.

Lichtenberg, Nick. _“Scott Galloway on Why That Anthropic Super Bowl Ad Got Under Sam Altman’s Skin and Exposed ‘Therapy’ as the AI Use Case.”_ _Fortune_, 9 Feb. 2026, [https://fortune.com/2026/02/09/what-was-anthropic-super-bowl-ad-chatgpt-therapy-sam-altman-reaction/](https://fortune.com/2026/02/09/what-was-anthropic-super-bowl-ad-chatgpt-therapy-sam-altman-reaction/). Accessed 12 February 2026.

Rudin, Cynthia. _Stop Explaining Black Box Machine Learning Models for High Stakes Decisions and Use Interpretable Models Instead._ arXiv, 26 Nov. 2018, [https://arxiv.org/abs/1811.10154](https://arxiv.org/abs/1811.10154). Accessed 12 February 2026.