# EXP-3-PROMPT-ENGINEERING-

## Aim: 
Evaluation of 2024 Prompting Tools Across Diverse AI Platforms: 
ChatGPT, Claude, Bard, Cohere Command, and Meta
Experiment:
Within a specific use case (e.g., summarizing text, answering technical questions), compare the performance, user experience, and response quality of prompting tools across these different AI platforms.

## Algorithm:
1.	Define scope & dataset
 o	Choose use cases (e.g., summarization, technical Q&A).
 o	Prepare a prompt set (N prompts per use case). Ensure variety, difficulty levels, and ground-truth where applicable.
2.	Define evaluation rubric
 o	Metrics: Accuracy (factual), Relevance, Clarity, Completeness/Depth, Conciseness, Safety/No-hallucination.
 o	Scoring scale: e.g., 1–5 for each metric.
3.	Generate outputs
 o	For each platform P and each prompt i, send prompt and collect response R_{P,i}.
 o	Record metadata: timestamp, model version, prompt template, parameters (temperature, max tokens).
4.	Human & automated evaluation
 o	Prepare blind evaluation sheets (remove platform labels).
 o	Have k human raters score each (or use automated checks for things like length, grammar, factual overlap).
 o	Compute inter-rater reliability (Cronbach’s alpha or Fleiss’ kappa).
5.	Aggregate scores
 o	For each (P, prompt), compute mean metric scores across raters.
 o	For each platform P, compute overall mean scores (per metric and weighted composite).
6.	Statistical testing
 o	Test for significance across platforms: repeated-measures ANOVA or Friedman test (non-parametric) depending on data distribution.
 o	If significant, perform pairwise comparisons (paired t-test with Bonferroni or Wilcoxon signed-rank).
7.	Qualitative analysis
 o	Collect representative good / bad outputs per platform.
 o	Note systematic behaviours (verbosity, hallucination patterns, formatting).
8.	Reporting
 o	Produce tables, radar charts, and per-use-case breakdowns.
 o	Provide recommendations and limitations.

## Prompt
I want to run a structured comparison of five major AI platforms—ChatGPT, Claude, Bard, Cohere Command, and Meta AI—by giving them the exact same tasks such as text summarization, technical question answering, and an open-ended reasoning challenge, and for each system I’ll record the identical prompt used, the response it generates, and then assess the result in terms of accuracy, clarity, depth, and overall user experience, so that I can see side-by-side which models perform best, where they fall short, and what unique strengths or limitations each one shows.

## Output
### Case 1: Summarizing Text

#### Prompt:
“Summarize the following text into three sentences: Space exploration is entering a new era with private companies developing reusable rockets, lowering launch costs, and expanding access to orbit. Alongside these advancements, there are concerns about space debris, planetary protection, and international regulations. Collaboration between governments, research institutions, and private industry is essential for sustainable exploration.”

#### Outputs & Results

ChatGPT
Private companies are revolutionizing space travel with reusable rockets that cut costs and expand orbital access. However, challenges like debris, planetary protection, and regulation persist. Governments, researchers, and industry are working together to ensure responsible exploration.

Accuracy: ✅

Clarity: ✅

Conciseness: ✅

Overall Quality: Excellent

#### Claude
Space travel is entering a commercial phase with reusable rockets reducing costs. This growth raises concerns over debris and planetary safety. Governments and industry must collaborate to create sustainable practices.

Accuracy: ✅

Clarity: ✅

Tone: Slightly formal

Overall Quality: Very Good

#### Bard (Gemini)
Reusable rockets are making space cheaper and more accessible. Concerns about debris and safety remain. Partnerships between governments and companies aim to manage these risks.

Accuracy: ✅

Clarity: ✅

Depth: Limited

Overall Quality: Moderate

#### Cohere Command
The new era of space exploration is driven by reusable rockets that cut costs. Yet, risks from debris, planetary contamination, and weak regulation remain significant. Global collaboration is essential to ensure safe expansion into space.

Accuracy: ✅

Clarity: Good

Tone: Technical

Overall Quality: Good

#### Meta AI
Space exploration is becoming cheaper due to reusable rockets. Still, debris and safety rules are issues. Governments and companies are working together.

Accuracy: ✅

Clarity: Fair (simplified)

Overall Quality: Average

### Case 2: Technical Q&A

#### Prompt:
“What is the role of wearable health technology in modern healthcare systems?”

#### Outputs & Results

#### ChatGPT
Wearable devices track real-time health data like heart rate, sleep, and activity, enabling early detection and continuous monitoring. They empower patients with insights while supporting doctors with valuable clinical information. These devices also integrate with telemedicine and preventive care models.

Result: Excellent – detailed, accurate, clear

#### Claude
Wearables provide ongoing monitoring of vital signs and activity. They help doctors manage patients remotely and improve preventive care. Their data is key to early detection of health issues.

Result: Very Good – concise but accurate

#### Bard (Gemini)
Smartwatches and wearables track health metrics. They help people and doctors keep an eye on health. This makes healthcare more proactive.

Result: Fair – correct but oversimplified

#### Cohere Command
Wearable health devices act as continuous data collectors, offering metrics on vitals, sleep, and activity. They support preventive medicine, clinical decision-making, and telehealth by feeding structured data into digital systems.

Result: Good – technically sound, enterprise style

#### Meta AI
Wearables measure things like heart rate and steps. They help monitor health and can connect with doctors.

Result: Average – correct but minimal depth

### Comparative Overview
<img width="925" height="347" alt="image" src="https://github.com/user-attachments/assets/e88be9af-0ef1-43c5-a37c-f89a302b6f8c" />

### Case 3: Summarization – Smart Cities
#### Prompt:
“Summarize the following passage into a short paragraph: Smart cities integrate digital technologies, sensors, and data-driven systems to improve urban living. They enhance efficiency in transportation, energy, and public services, while also promoting sustainability. Key challenges include data privacy, cybersecurity, and equitable access.”

#### Model Outputs

ChatGPT: Smart cities use digital technologies and data systems to improve transport, energy, and public services while enhancing sustainability. They face hurdles like privacy, cybersecurity, and ensuring equal access.

Claude: Urban areas are becoming smarter through connected technologies that boost efficiency and sustainability. Privacy, security, and fairness remain pressing issues.

Bard (Gemini): Smart cities use sensors and data to improve services and sustainability. But privacy and access challenges remain.

Cohere Command: Smart city systems optimize transport, energy, and services through data-driven approaches. Still, concerns about data protection, cybersecurity, and equitable use persist.

Meta AI: Smart cities improve transport, energy, and services but still struggle with privacy and fairness.

### Evaluation
<img width="980" height="342" alt="image" src="https://github.com/user-attachments/assets/45215f22-ca76-4799-ab25-488ef0a7159a" />

## Result

ChatGPT: Best performer—detailed, clear, accurate, and versatile.

Claude: Strong competitor—clear and polished, slightly less detailed.

Cohere Command: Reliable, enterprise-style clarity, but formal tone.

Bard (Gemini): Simplified, beginner-friendly, lacks advanced depth.

Meta AI: Simple and functional, but limited in detail.

Overall Ranking

⭐ ChatGPT (OpenAI)

⭐ Claude (Anthropic)

⭐ Cohere Command

⭐ Bard / Gemini (Google)

⭐ Meta AI



