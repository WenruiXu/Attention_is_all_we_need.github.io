

# The web page of the final project for CSCI 5541 F25
# CSCI-5541-Final-Project
Team Name: Attention is all we need
**Authors:** Wenwen Cao, Jikai Sun, Wenrui Xu, Zishu Wang


## Overview
With the growing use of GenAI systems (e.g., ChatGPT), emotionally expressive chatbots are becoming a new channel for product discovery and consumer decision-making. This project studies whether emotional expression in an LLM-based product recommendation chatbot improves or harms user responses (engagement, satisfaction, purchase intention), and how this depends on expectation confirmation/violation, product type, and perceived human likeness.

## Research Questions
- Does emotional expression in a product recommendation chatbot increase engagement, satisfaction, and purchase intention—or undermine them?
- How do **users’ expectations**, **product type** (hedonic vs. utilitarian), and **perceived human likeness** shape these outcomes?

## Method
We designed an online experiment where participants interact with an LLM-based chatbot connected via API and then complete survey measures. Participants are recruited from online platforms (e.g., Prolific). 
### Experimental Design (2×2)
Participants are assigned to:
1. **Chatbot style:** Emotional vs. Neutral  
2. **Product type:** Hedonic (chocolate) vs. Utilitarian (dish soap) 

**Workflow diagrams:** The overall workflow is illustrated in Figure 1 (page 3) and the web interface for control variables is shown in Figure 2 (page 3). 
### Chatbot Prompts (Core Manipulation)
**Emotional condition prompt (excerpt):**
- “You are an enthusiastic and warm product recommendation assistant… Use emotionally rich language… show understanding… build a friendly connection…” 

**Neutral condition prompt (excerpt):**
- “You are a neutral product recommendation assistant… Provide clear, factual, and informative responses without emotional expression…” 

**Token control:** An additional instruction was used: *“Provide the answer in 300 tokens.”*

## Measurements
All outcomes are self-reported:
- **Engagement:** 1 item, 7-point Likert (e.g., “engaging and interesting”). 
- **Satisfaction:** 3 items, 7-point Likert (adapted from prior work).  
- **Purchase Intention:** 7-point bipolar scales (unlikely/likely, improbable/probable, impossible/possible).
- **Perceived Human Likeness:** bipolar items (technology-like vs. human-like, etc.). 
- **Emotional Intensity:** 3 bipolar items (very little emotion vs. great deal of emotion, etc.).
- **Expectation Confirmation (post-test):** 3 items on a 7-point Likert scale. 

## Preliminary Results (N = 23)
Key manipulation checks were successful:
- **Human likeness** was significantly higher for emotional vs. neutral chatbot:
  - Neutral: M = 2.57 (SD = 1.28)
  - Emotional: M = 4.15 (SD = 1.36)
  - F = 7.65, p = 0.01, η²p = 0.29 
- **Emotional intensity** was significantly higher for emotional vs. neutral chatbot:
  - Neutral: M = 2.62 (SD = 1.80)
  - Emotional: M = 4.52 (SD = 1.66)
  - F = 7.63, p = 0.01, η²p = 0.29 
- **Expectation confirmation** differed significantly between confirmation vs. violation groups:
  - Confirmation: M = 5.03 (SD = 1.42)
  - Violation: M = 3.78 (SD = 1.33)
  - F = 5.18, p = 0.03, η²p = 0.21 

No significant effects were detected on:
- **Engagement**, **Satisfaction**, and **Purchase Intention** (across expectation confirmation/violation, emotion condition, and product type), likely due to small sample size and limited power.

### Descriptive Statistics (Key Variables)
- Engagement: M = 4.57, SD = 1.78  
- Satisfaction: M = 5.17, SD = 1.31  
- Purchase intention: M = 5.13, SD = 1.52  
- Human likeness: M = 3.19, SD = 1.50  
- Emotional intensity: M = 3.36, SD = 1.95  
- Expectation confirmation: M = 4.38, SD = 1.48

### Correlations (Selected)
Engagement correlates with satisfaction (0.74***), and satisfaction correlates strongly with purchase intention (0.85***). Human likeness correlates with emotional intensity (0.66***).

## Replicability
- The study uses a clear **2×2 design** (emotion condition × product type) and a local HTML/CSS/JS chat interface that calls an LLM via fixed prompts.
- Conversations were generated locally and not stored; thus exact dialogues are not reproducible, but the **procedure and survey measures** are straightforward to replicate.

## Dataset
The dataset consists of **participants’ survey responses** (ratings for engagement, human-likeness, emotional intensity, expectation confirmation, satisfaction, purchase intention). No manual annotation required.

## Ethics
- Informed consent was used.
- Only low-stakes product categories were used.
- The project highlights the importance of transparency about the chatbot’s artificial nature and avoiding excessive emotional cues.

## Limitations & Future Work
- Small sample size (N = 23) limits statistical power.
- Conversations were not stored, preventing linguistic/behavioral analysis.
- Emotion manipulation was text-only (no multimodal emotion).
- Future plans: larger sample, consented conversation logging, more product categories, compare different LLMs, explore adaptive emotional strategies. 
