# Group Research Project Report

## Team Members:
1. Karthik Ramu 2. Nargus Batool 3. Mohammadali Ghaderi

## Declaration
...

## Executive Summary
...

## Introduction
...  

## Methodology
This study adopted a quantitative, survey-based design to explore attitudes toward AI in customer service among university-aged respondents. A structured online questionnaire allowed us to capture standardized ratings on multiple constructs and to link these two basic demographic and behavioral variables.

### Data collection and population

Google Forms survey was used to gather data. The link was shared via university WhatsApp groups, cohort chats, and personal social media networks. The target population was students and young adults (approximately 18–34 years old) who frequently interact with digital services and are thus prone to meet AI-powered customer support in areas such as banking, e-commerce, and travel. Participation was compulsory and non-identifying. We did not obtain names, email addresses or other direct identifiers. The dataset eventually used for the analysis contained 62 valid responses after the exclusion of incomplete or inconsistent entries.

### Survey instrument and measures

The questionnaire included Likert-scale items grouped into six constructs informed by prior research on AI acceptance and technology adoption (Bristows, 2019; Granlund and Lundström, 2024):

- Helpfulness (five items) – perceived ability of AI tools to provide useful and accurate support.
- Convenience (four items) – time-saving, availability, and suitability for simple queries.
- Ease of Interaction (six items) – clarity, smoothness, and perceived effort when interacting with AI.
- Trust (five items) – perceived reliability, credibility, and alignment with customers’ best interests.
- Preference for AI (four items) – relative preference for AI versus human agents in routine tasks.
- Behavioral Intention (five items) – willingness to reuse, recommend, and continue relying on AI tools.

All attitudinal items were rated on a five-point Likert scale from 1 (“Strongly disagree”) to 5 (“Strongly agree”). Demographic questions covered age group, gender, education level, region, self-reported comfort with new technologies, and frequency of interacting with AI customer service tools.

### Data preparation and analytical tools

The final data set was first exported as survey_final.csv and then analyzed using Python on the Google Colab platform. For cleaning and transforming data, the panda’s library was utilized, whereas descriptive and inferential statistics were carried out with pingouin and scipy.stats, and lastly, the ANOVA and regression models were created with statsmodels. The process of visualization included the use of matplotlib, seaborn, and sometimes plotly for the exploratory plots in the notebook. A composite score for each construct was calculated by taking the average of the corresponding Likert items for each respondent. These composites became the primary variables for our analyses. The cleaned dataset and the steps of the analysis are presented in the file 1.ipynb.

### Analysis Plan and Hypotheses

Our research analysis followed the study's recommendations for small-sample survey research (n ≈ 60) and first provided descriptive statistics (means and standard deviations) for each construct. Subsequently, it correlated the variables Helpfulness, Convenience, Ease of Interaction, Trust, AI Preference, and Intention to Use using Pearson’s r. One-way ANOVA was then applied to conduct group comparisons based on the participants' self-reported tech comfort and the frequency of their AI customer service use. The regression modeling technique was utilized to assess the collective predictive power of Trust, Helpfulness, and Convenience for either AI Preference or Behavioral Intention. The major hypotheses that guided the analysis were that Trust would be positively related to AI Preference in customer service (H1); the influence of Trust on Preference would be through Convenience (H2); the differences between Trust and Preference would be significant for self-reported tech comfort (H3); the difference between Trust, Convenience, and Ease of Interaction would be significant for AI usage frequency (H4), and the multi-predictor model of Trust, Helpfulness, and Convenience would account for a large share of the variance in AI Preference or Behavioral Intention (H5). 

---

## Results
... 

## Discussion
... 

## Recommendations
... 

## Reflection on Team Process

Our group applied the Agile and Kanban methodologies learned during the SKIB353 course to carry out the project in an efficient manner. A team Kanban board was used to organize the tasks, which were survey design, data cleaning, coding in Python, and writing, while at the same time preventing overload and increasing visibility. The short meetings enabled us to quickly change our plans and fix any problems that arose. Although initially, not all the team members were confident using Python, its use helped with the reproducibility and analytical depth, and GitHub was the tool that made the async collaboration the smoothest one. The adoption of an iterative agile mindset was what allowed us to continuously improve our work and, finally, produce a report for OmniAssist that was clear and data-driven.

---

## References and Appendices

### References

* Bristows LLP (2019) *Artificial Intelligence: Public Perception, Attitude and Trust*. London: Bristows LLP.
* Bryman, A. (2016) *Social Research Methods*. 5th edn. Oxford: Oxford University Press.
* Field, A. (2018) *Discovering Statistics Using IBM SPSS Statistics*. 5th edn. London: Sage.
* Granlund, J. and Lundström, D. (2024) *Unveiling the Impact of AI-Powered Chatbots on Customer Acceptance in Sweden*. Bachelor thesis. Mälardalen University.
* Nature HSSC (2024) ‘Exploring the mechanism of sustained consumer trust in AI chatbots after service failures: a perspective based on attribution and CASA theories’, *Humanities and Social Sciences Communications*, 11, pp. 1–15.
* Pallant, J. (2020) *SPSS Survival Manual*. 7th edn. Maidenhead: McGraw-Hill Education.
* Schulz, P.J. et al. (2023) ‘Modeling the influence of attitudes, trust, and beliefs on endoscopists’ acceptance of artificial intelligence applications in medical practice’, *Frontiers in Public Health*, 11, 1301563.
* SKIB353 Module Materials (2025) *Skills for Data Analysts: Empirical Research Guidance*.
* University Moodle Resources, Weeks 1–3.
* Wang, X., Lin, X. and Shao, B. (2022) ‘How does artificial intelligence create business agility? Evidence from chatbots’, *International Journal of Information Management*, 66, 102535.

---
### Appendices Appendix

#### A. Survey questionnaire (full list of Likert items and demographic questions). 

##### Survey on Public Attitudes Toward AI in Customer Service 

###### Introduction Text 

Thank you for taking part in this short anonymous survey about customer service experiences.  
Your responses will help us understand how people perceive the use of artificial intelligence (AI) tools such as chatbots and virtual assistants in customer service.  
The survey takes about 5 minutes to complete.  

---

#### Section 1: Screening and Background 

*(To ensure participants have basic familiarity with the topic.)*  

1. Have you ever interacted with an AI-based customer service tool (for example, a chatbot or virtual assistant)?  
   - o Yes  
   - o No  
   - o I’m not sure  

2. How often do you interact with AI customer service tools?  
   - o Frequently  
   - o Occasionally  
   - o Rarely  
   - o Never  

3. In which of the following service areas have you experienced AI-based customer service? (Select all that apply)  
   - o Retail or online shopping  
   - o Banking or financial services  
   - o Telecommunications or internet services  
   - o Travel or hospitality  
   - o Healthcare  
   - o Other sectors  
   - o I have not used any  

---

#### Section 2: Perceived Helpfulness of AI 

*(5-point Likert scale: 1 = Strongly Disagree → 5 = Strongly Agree)*  

4. AI customer service tools help me find the information I need efficiently.  
5. AI systems are able to provide accurate answers to my questions.  
6. AI tools make it easier to solve simple service-related issues.  
7. I am usually satisfied with the results provided by AI customer service systems.  
8. AI customer service tools improve my overall experience with the company.  

---

#### Section 3: Perceived Convenience 

*(5-point Likert scale)*  

9. Using AI customer service tools saves me time.  
10. AI systems are available whenever I need assistance.  
11. I find it easy to access AI-based support on company websites or apps.  
12. The process of interacting with an AI chatbot or assistant is straightforward.  
13. AI-based customer service helps me resolve issues without waiting in line for human support.  

---

#### Section 4: Perceived Trust 

*(5-point Likert scale)*  

14. I believe AI customer service tools provide reliable information.  
15. I trust AI chatbots to handle my customer queries properly.  
16. I feel confident that AI systems respond to my requests accurately.  
17. I consider AI-based customer service tools credible.  
18. I believe AI assistants are designed to serve customers’ best interests.  

---

#### Section 5: Perceived Frustration (Low-friction Focus) 

*(5-point Likert scale — all positive phrasing to avoid emotional/negative tone)*  

19. I find it easy to communicate my needs when using AI customer service tools.  
20. AI systems usually understand my questions correctly.  
21. Interacting with AI systems feels smooth and efficient.  
22. AI tools guide me clearly through the support process.  
23. AI-based customer service meets my expectations most of the time.  

---

#### Section 6: Preference for Human vs. AI Interaction 

*(5-point Likert scale)*  

24. AI customer service is suitable for handling simple inquiries.  
25. I prefer using AI tools when I need quick answers.  
26. I am comfortable relying on AI systems for common service tasks.  
27. I believe human agents should focus on complex issues, while AI handles routine ones.  
28. I would be willing to use AI customer service again in the future.  
29. I would recommend AI-based customer support to others.  
30. I believe companies benefit from using AI alongside human customer service teams.  

---

#### Section 7: Demographic Information 

*(Optional and non-intrusive — no personal data)*  

31. What is your age group?  
   - • Under 18  
   - • 18–24  
   - • 25–34  
   - • 35–44  
   - • 45–54  
   - • 55–64  
   - • 65 or older  

32. What is your gender?  
   - • Male  
   - • Female  
   - • Non-binary / other  
   - • Prefer not to say  

33. What is your highest level of education completed?  
   - • High school or equivalent  
   - • Some college or diploma  
   - • Bachelor’s degree  
   - • Master’s degree  
   - • Doctorate or higher  
   - • Prefer not to say  

34. Which region or country do you currently live in?  
   - • Africa  
   - • Asia  
   - • Europe  
   - • North America  
   - • South America  
   - • Oceania  

35. How comfortable are you using new technologies in daily life?  
   - • Very comfortable  
   - • Somewhat comfortable  
   - • Neutral  
   - • Slightly uncomfortable  
   - • Very uncomfortable  

---

#### Response Scale Reminder 

All attitude statements (Questions 4–30) use a 5-point Likert scale:  

1 = Strongly Disagree  
2 = Disagree  
3 = Neutral  
4 = Agree  
5 = Strongly Agree  

---

### Construct Mapping 

| Construct                  | Question Numbers |
|----------------------------|------------------|
| Helpfulness                | 4–8              |
| Convenience                | 9–13             |
| Trust                      | 14–18            |
| Frustration (low-friction) | 19–23            |
| Preference                 | 24–30            |
| Demographics               | 31–35            |

--- 