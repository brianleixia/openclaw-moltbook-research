# QE Defense Speech Script
## Beyond Citation Counts: A Survey of Semantic Scientific Impact Evaluation

**Author:** XIA Lei (Department of Computer Science, Hong Kong Baptist University)  
**Duration:** 25 minutes  
**Word Count:** ~3,200 words

---

## Slide 1: Title Slide

*[Begin with a confident stance, make eye contact with the audience]*

Good morning, distinguished committee members, colleagues, and friends. Thank you for being here today.

My name is XIA Lei, and I am a PhD candidate in the Department of Computer Science at Hong Kong Baptist University. Today, I am honored to present my QE report entitled "Beyond Citation Counts: A Survey of Semantic Scientific Impact Evaluation."

This work represents my journey into understanding how we evaluate scientific impact — not just by counting citations, but by understanding what those citations actually mean. Over the next 25 minutes, I will walk you through the motivation behind this research, our core methodology, the framework we have developed, and the preliminary experiments that validate our approach.

*[Pause briefly, gesture to the screen]*

Let me begin by outlining what we will cover today.

---

## Slide 2: Outline / Agenda

*[Gesture toward the roadmap on screen]*

Today's presentation is structured in seven parts. First, I will introduce the fundamental problem that motivated this research — why traditional citation metrics are insufficient for understanding scientific impact. Second, I will elaborate on the problem background and the semantic gap in current evaluation practices. Third, I will present our core methodology: Citation Content Analysis, or CCA. Fourth, I will introduce the three evidence sources that form the foundation of our framework. Fifth, I will present our proposed framework for Evidence-Grounded Meaningful Citation Identification. Sixth, I will share results from our preliminary experiments. Finally, I will conclude with a summary and directions for future work.

*[Brief pause]*

Before diving into the technical content, let me briefly introduce myself and my research journey.

---

## Slide 3: Personal Introduction

*[Speak with personal warmth and authenticity]*

I came to this research question through a rather circuitous path. Like many of you, I have spent countless hours reading papers, writing literature reviews, and trying to understand which works in my field truly matter. Early in my PhD, I found myself frustrated by the disconnect between what citation counts suggested was important and what my careful reading revealed was actually influential.

I would see papers with hundreds of citations that were merely mentioned in passing — background citations that authors felt obligated to include. At the same time, I would discover brilliant methodological innovations buried in papers with modest citation counts, works that had fundamentally changed how subsequent research was conducted but never received the recognition they deserved.

This observation led me to a simple but profound question: What if we could understand citations not just as numbers, but as semantic relationships? What if we could distinguish between a citation that merely acknowledges prior work and one that genuinely builds upon it? This question has driven my research for the past two years, and today I am excited to share what we have learned.

*[Transition to the problem statement]*

Let me now articulate the central problem we address in this work.

---

## Slide 4: The Citation Paradox

*[Use a measured, serious tone to convey the importance of the problem]*

The citation paradox can be summarized in a single sentence: We count citations, but we don't understand them.

For decades, the scientific community has relied on a trio of metrics to evaluate research impact. Citation count tells us how many times a paper has been referenced. The h-index attempts to balance productivity with impact. Journal impact factor serves as a proxy for the prestige of the venue where work is published.

*[Pause for emphasis]*

These metrics share a fundamental and problematic assumption: they treat all citations as equivalent. A citation that merely acknowledges related work counts the same as a citation that adopts the methodology, extends the findings, or engages in substantive critique.

This assumption is not just an oversimplification — it is fundamentally wrong. Citation is not a monolithic concept. When we cite a paper, we do so for many different reasons, with varying degrees of engagement and intellectual debt. Reducing this rich semantic landscape to a single number is like trying to understand a conversation by counting how many times each person speaks, without listening to what they actually say.

*[Gesture to indicate the next point]*

To illustrate why this matters, let me show you some concrete examples.

---

## Slide 5: Why Semantics Matter

*[Speak with illustrative examples, use hand gestures to differentiate types]*

Consider these five different ways a paper might be cited. First, as background — "Previous work established the foundation for our approach." This is a polite acknowledgment, but it tells us little about the actual influence of the cited work.

Second, as methodology — "Following Smith et al., we adopt the same evaluation protocol." Here, the citation represents a substantial intellectual debt. The citing work is built upon the methodological foundation laid by the cited work.

Third, for comparison — "Unlike Jones et al., our approach handles edge cases." This citation engages critically with prior work, positioning the new contribution in relation to existing approaches.

Fourth, as critique — "However, Wang et al. suffer from scalability issues." Negative citations, while seemingly detrimental, often indicate that the cited work was significant enough to warrant serious engagement.

Fifth, as extension — "Building upon Chen et al., we introduce a novel regularization technique." This represents perhaps the most meaningful form of citation, where the cited work directly enables new contributions.

*[Pause, look at the audience]*

The key insight here is that the same citation count can represent vastly different patterns of scientific contribution. A paper with fifty methodological adoption citations has had a fundamentally different impact than a paper with fifty background mentions, yet traditional metrics treat them identically.

So how do we capture this semantic richness? This brings us to our core methodology.

---

## Slide 6: Core Methodology — Citation Content Analysis (CCA)

*[Transition to technical content, speak with clarity and precision]*

Citation Content Analysis, or CCA, is our approach to systematically examining the contexts in which citations appear. Rather than treating citations as isolated entities, we analyze the surrounding text to understand the nature of the citation relationship.

Our methodology encompasses four key extraction tasks. First, citation context extraction — identifying the sentences that contain citations and capturing both their immediate local context and broader discourse context within the paper.

Second, citation intent or function classification — determining why a work was cited. Was it for background, methodology, comparison, critique, or extension? This task moves us from simply knowing that a citation exists to understanding its purpose.

Third, citation polarity and stance detection — assessing whether the citation is positive, negative, or neutral. Does the citing author endorse the cited work, criticize it, or merely acknowledge it?

Fourth, influential citation identification — distinguishing between ceremonial citations that serve social or political functions and substantive citations that genuinely shape the citing work.

*[Gesture to indicate the pipeline]*

Let me now walk you through how we operationalize this methodology.

---

## Slide 7: CCA Technical Pipeline

*[Use the diagram on screen to guide the explanation]*

Our technical pipeline begins with scientific papers in PDF or XML format. We first extract and preprocess the text, handling the various formatting conventions used by different publishers.

Next, we perform citation mention detection, identifying where in the text citations appear and linking them to entries in the reference list. This is more challenging than it might seem, given the variety of citation styles and the presence of parenthetical mentions, numbered references, and author-date formats.

Once we have identified citation mentions, we extract context windows around each mention. We capture not just the sentence containing the citation, but surrounding sentences that provide important discourse context.

From these contexts, we apply our four analysis tasks. For intent classification, we use BERT-based models fine-tuned on annotated citation corpora. For polarity detection, we combine sentiment analysis with domain-specific training. For influence scoring, we integrate graph-based features from the citation network with text-based features from the contexts.

The output is a structured citation knowledge base that captures not just who cited whom, but the semantic nature of each citation relationship.

*[Acknowledge technical challenges]*

We face several technical challenges in this pipeline. Scientific papers use diverse citation formats, requiring robust parsing. Models must adapt across scientific fields with different citation conventions. And processing long documents with hundreds of citations requires careful attention to computational efficiency.

---

## Slide 8: The Semantic Gap — Visualized

*[Use the visual comparison to reinforce the message]*

To make this concrete, let me show you what changes when we apply CCA. Before CCA, our citation network looks like the diagram on the left. Every edge looks the same. We know that Paper A cites Paper B, but we have no information about the nature of that relationship.

After CCA, our network looks like the diagram on the right. Now edges have semantic labels. We can see that Paper A extends Paper B — a strong, positive relationship. Paper B critiques Paper C — a negative but still meaningful engagement. Paper C cites Paper A as background — a weaker, more ceremonial connection.

*[Pause for emphasis]*

This transformation from a monochrome network to a semantically rich graph is the core contribution of CCA. It allows us to move beyond counting connections to understanding their meaning.

Now, how do we use this semantic understanding for impact evaluation? This brings us to our three evidence sources.

---

## Slide 9: Three Evidence Sources — Overview

*[Introduce the framework with a holistic perspective]*

We propose a holistic framework for impact evaluation based on three distinct but complementary evidence sources. No single source tells the complete story of a paper's impact, but together they provide a much richer picture than citation counts alone.

The first source is E-citation — external evidence derived from how the community engages with the work through citations. This is where CCA plays a central role.

The second source is E-quality — intrinsic evidence derived from assessing the quality of the work itself, independent of its reception. This includes automatic peer review and novelty detection.

The third source is E-integrity — validation evidence derived from checking the trustworthiness of citations and the accuracy of claims.

*[Gesture to the diagram]*

These three sources form a comprehensive foundation for impact assessment. Let me elaborate on each in turn.

---

## Slide 10: E_citation — Citation Evidence

*[Focus on the external validation aspect]*

E-citation captures how the scientific community engages with a work through citations. This is external validation — evidence that comes from outside the paper itself.

From CCA, we derive several meaningful metrics. The intent distribution tells us what purposes the work serves for the community. Is it primarily used for background, or do researchers actually adopt its methodology? The polarity profile reveals whether the reception has been generally positive or if the work has generated controversy. The influence score distinguishes substantive citations that shape subsequent work from ceremonial citations that merely pay lip service.

*[Provide a concrete example]*

Consider this example. Paper X has one hundred citations, but eighty percent are background mentions — polite acknowledgments with little substantive engagement. Paper Y has only fifty citations, but sixty percent represent methodological adoption — researchers are actually using the techniques developed in this work. Traditional metrics favor Paper X. Our semantic analysis reveals that Paper Y has had more meaningful impact.

This is the power of E-citation: it allows us to distinguish between popularity and genuine influence.

---

## Slide 11: E_quality — Intrinsic Quality Assessment

*[Shift to the internal evaluation perspective]*

E-quality shifts our focus from how the community receives a work to the intrinsic quality of the work itself. This is internal validation — evidence derived from analyzing the paper's content.

We approach this through two main avenues. First, automatic peer review — using natural language processing to assess methodology soundness, evaluate experimental design, and check for reproducibility indicators. While not replacing human peer review, these automated tools can provide consistent, scalable quality signals.

Second, novelty detection — classifying the type of contribution a paper makes, scoring its degree of innovation, and analyzing its relationship to prior work. Is this an incremental improvement or a breakthrough? Does it open new research directions or close existing ones?

*[Pose the key question]*

The key question E-quality asks is this: Does the work meet high scientific standards independent of its popularity? A paper might be widely cited for historical reasons or because it confirms popular biases, but E-quality asks whether it is scientifically sound on its own merits.

This is particularly important for identifying undervalued work — brilliant papers that have not yet received the attention they deserve.

---

## Slide 12: E_integrity — Integrity & Verification

*[Adopt a serious tone appropriate to the topic of integrity]*

E-integrity addresses a concern that has received increasing attention in recent years: the trustworthiness of scientific claims and the accuracy of citations.

Citation validity checking examines whether citations accurately represent the cited work. Does the citing paper fairly characterize the findings of the cited work, or does it distort them to support its own claims? Our analysis suggests that citation distortion is more common than we might hope, with approximately fifteen percent of citations showing some form of misrepresentation.

Claim provenance tracing follows claims back to their origins. When a paper makes a strong claim, where did that claim come from? Is it properly attributed? Does the cited work actually support the claim being made?

*[Highlight the importance]*

Integrity issues undermine the entire edifice of scientific communication. If we cannot trust that citations accurately represent the works they cite, then citation counts become not just meaningless but actively misleading. E-integrity provides tools to detect and flag these issues, contributing to a more trustworthy scientific literature.

---

## Slide 13: Proposed Framework — Evidence-Grounded Meaningful Citation Identification

*[Present the integrated framework with pride]*

Bringing together these three evidence sources, we propose a unified framework for Evidence-Grounded Meaningful Citation Identification. This is our main contribution — a systematic approach to identifying citations that represent genuine scientific influence.

*[Walk through the architecture]*

The framework takes as input a candidate paper and its citation network. It then processes this input through three parallel modules. The E-citation module produces a citation evidence score based on the semantic analysis of incoming citations. The E-quality module produces an intrinsic quality score based on automated assessment of the paper's content. The E-integrity module produces a trustworthiness score based on verification of citations and claims.

These three scores are then fused through an evidence integration layer that weights and combines them based on their reliability and relevance. The output is a meaningful citation score that ranks papers by their genuine scientific impact.

*[Emphasize the novelty]*

What distinguishes our framework is its multi-source approach. By combining external reception, intrinsic quality, and integrity verification, we avoid the pitfalls of relying on any single metric. A paper with high citation counts but poor integrity scores is flagged. A paper with modest citations but high quality and positive reception is elevated.

---

## Slide 14: Preliminary Experiments

*[Present results with appropriate scientific caution and enthusiasm]*

To validate our framework, we conducted four preliminary experiments. I will briefly summarize the key findings.

For citation intent classification, we fine-tuned SciBERT on the ACL-ARC and SciCite datasets. We achieved an F1 score of 0.84 for three-class classification and 0.76 for six-class classification. These results demonstrate that automatic intent classification is feasible with current NLP techniques.

For citation polarity classification, we trained a RoBERTa model with domain adaptation on a custom annotated corpus. We achieved 81% accuracy and a macro F1 of 0.78, showing that we can reliably distinguish positive, negative, and neutral citations.

For citation-based summarization, we developed a hybrid extractive-abstractive approach that generates paper summaries from citation contexts. Our ROUGE scores of 0.42 for ROUGE-1 and 0.38 for ROUGE-L indicate that citation contexts contain sufficient information for meaningful summarization.

Most importantly, for meaningful citation identification, we compared our evidence-grounded approach against a citation count baseline using expert annotations as ground truth. Our method achieved a 23% improvement in precision at top-10, demonstrating that semantic features significantly improve impact prediction.

---

## Slide 15: Key Findings & Insights

*[Synthesize the lessons learned]*

These experiments have yielded several important insights that I want to highlight.

First, semantic features significantly improve impact prediction. The distribution of citation intents is more informative than raw counts alone. Interestingly, we found that negative citations can indicate high influence — controversy drives engagement, and papers that generate strong reactions are often those that have fundamentally shaped their fields.

Second, quality and popularity are not synonymous. Our intrinsic quality assessment reveals many papers with high citation counts but modest quality scores, as well as brilliant but undercited work. This confirms our initial observation that citation counts alone are insufficient for impact evaluation.

Third, integrity issues are prevalent. Our analysis found that approximately fifteen percent of citations show some form of distortion, whether through misrepresentation of findings, cherry-picking of evidence, or citation amnesia. Automated detection of these issues is both feasible and necessary.

Fourth, multi-source evidence is essential. No single metric captures meaningful impact. Our fusion approaches consistently outperform individual signals, confirming the value of our three-pillar framework.

---

## Slide 16: Contributions & Impact

*[Clearly articulate the value of the work]*

Let me summarize the main contributions of this research.

First, we provide a comprehensive survey of semantic citation analysis. To our knowledge, this is the first systematic review of CCA approaches, and we introduce a unified taxonomy that organizes the diverse methods in this space.

Second, we propose a novel evidence-based framework that integrates three distinct sources of evidence — external citation patterns, intrinsic quality signals, and integrity verification. This multi-pillar approach addresses the limitations of single-metric evaluation.

Third, we provide empirical validation of our framework components through carefully designed experiments. We are committed to open science and will release our datasets and code to the research community.

*[Discuss broader impact]*

The potential impact of this work extends beyond academic interest. More nuanced research evaluation could improve hiring and promotion decisions, helping institutions identify truly influential scholars rather than merely popular ones. Better identification of influential work could enhance literature review and discovery tools. And the policy implications for funding agencies and evaluation committees are significant — we can move toward evaluation systems that reward genuine scientific contribution rather than gaming of metrics.

---

## Slide 17: Conclusion & Future Directions

*[Conclude with confidence and vision]*

Let me conclude by returning to the central theme of this presentation. Moving beyond citation counts requires understanding the semantic fabric of scientific discourse. Citations are not just links in a network — they are conversations between researchers, acknowledgments of intellectual debt, critiques of prior work, and foundations for future contributions.

Our framework provides a foundation for more meaningful impact evaluation by capturing this semantic richness. We do not claim to have solved the problem of research evaluation — that is a task that will require ongoing effort from the entire scientific community. But we believe we have taken an important step toward evaluation systems that align with the values of science: rigor, innovation, and genuine contribution to knowledge.

*[Outline future directions]*

Looking ahead, we see several important directions for future work. We need to scale our framework to full publication corpora like Web of Science and Semantic Scholar, moving beyond the limited datasets we have used for validation. We need to adapt our framework to humanities and social sciences, where citation practices differ significantly from computer science and the natural sciences. We are interested in longitudinal analysis — tracking how a paper's impact evolves over time, from initial reception to long-term influence. We want to integrate our framework with academic search and recommendation systems, helping researchers discover influential work that traditional metrics might miss. And we hope to collaborate with funding agencies and evaluation committees to translate our research into practical policy improvements.

*[Final thanks]*

Thank you for your attention. I am happy to take any questions you may have.

---

## Q&A Preparation Notes

**Likely Questions and Suggested Responses:**

1. **"How does your framework handle interdisciplinary research where citation practices differ?"**
   - Acknowledge this is an active challenge
   - Mention plans for domain adaptation
   - Emphasize the modular nature of the framework allowing field-specific tuning

2. **"What is the computational cost of your approach compared to simple citation counting?"**
   - Be honest about the increased cost
   - Argue that the improved accuracy justifies the cost for important decisions
   - Mention ongoing optimization work

3. **"How do you validate your 'meaningful citation' ground truth?"**
   - Describe the expert annotation process
   - Acknowledge subjectivity and inter-annotator agreement
   - Mention plans for larger-scale validation studies

4. **"Could this framework be gamed if widely adopted?"**
   - Acknowledge the possibility
   - Argue that semantic analysis is harder to game than simple counts
   - Emphasize integrity checking as a countermeasure

5. **"What are the immediate practical applications?"**
   - Literature review assistance
   - Grant evaluation support
   - Researcher profiling for hiring
   - Academic search ranking improvements

---

## Delivery Tips

**Pacing:**
- Speak slightly slower than normal conversation
- Pause after key points for emphasis
- Allow time for the audience to process diagrams

**Body Language:**
- Make eye contact with different committee members
- Use hand gestures to emphasize key points
- Stand confidently, avoid fidgeting

**Handling Nerves:**
- Remember that you know this material better than anyone
- The committee wants you to succeed
- It's okay to pause and collect your thoughts

**Technical Issues:**
- Have slides available offline
- Know key points by heart in case slides fail
- Stay calm and professional if technology fails

---

## End of Script
