# **Final Survey Instrument: Public Attitudes Toward AI in Customer Service**

This survey instrument is organized into clearly defined construct blocks to support structured data collection and reproducible quantitative analysis. Each item is assigned an export-friendly variable label (e.g., `trust_2`, `helpful_1`, `intention_1`) to ensure compatibility with statistical tools such as Python, R, and SPSS.

The questionnaire follows established frameworks used in the study of human–AI interaction, including the Technology Acceptance Model (TAM) and the Computers Are Social Actors (CASA) perspective. The constructs measured include:

- **Helpfulness**
- **Convenience**
- **Trust**
- **Ease of Interaction**
- **Preference**
- **Behavioral Intention** (designated as the primary outcome variable)

The Behavioral Intention block is clearly separated and renumbered to allow direct use in regression modeling.  
All items are closed-ended, positively phrased, and intentionally free from negative wording, emotional prompts, double-barrelled wording, or privacy-intrusive questions.

This structure supports:

- Reliable scale construction  
- Clear variable grouping and naming  
- Correlation and regression analysis  
- Transparent interpretation of relationships between constructs  

Overall, the survey is designed to capture public attitudes toward AI-based customer service in a way that is methodologically consistent, data-ready, and aligned with best practices in empirical research.


---

## **Section 1: Screening / Background**

1. Have you interacted with an AI-based customer service tool (e.g., chatbot, voice assistant)?

   * Yes
   * No
   * Not sure
     → **Label**: `ai_experience`

2. How often do you use AI-based customer service tools?

   * Frequently
   * Occasionally
   * Rarely
   * Never
     → **Label**: `ai_frequency`

3. In which areas have you used AI-based customer support? *(select all that apply)*

   * Retail
   * Banking
   * Telecom
   * Travel
   * Healthcare
   * Other
   * I haven’t used AI-based support
     → **Label**: `ai_sector`

---

## **Section 2: Perceived Helpfulness (Construct: Helpfulness)**

Scale: `1 = Strongly Disagree` to `5 = Strongly Agree`

4. AI customer service tools help me find information quickly. → `helpful_1`
5. AI systems provide useful answers to my queries. → `helpful_2`
6. AI tools are helpful for solving routine problems. → `helpful_3`
7. I am satisfied with how AI systems assist me. → `helpful_4`
8. AI enhances the quality of my customer service experience. → `helpful_5`

---

## **Section 3: Perceived Convenience**

9. AI support tools save me time. → `conv_1`
10. AI systems are available whenever I need them. → `conv_2`
11. Accessing AI customer service is easy. → `conv_3`
12. Using AI systems is straightforward. → `conv_4`
13. I can resolve issues faster with AI than with human agents. → `conv_5`

---

## **Section 4: Perceived Trust**

14. I believe AI support tools provide accurate information. → `trust_1`
15. I trust AI chatbots to handle my requests. → `trust_2`
16. I feel confident relying on AI-based support. → `trust_3`
17. I believe companies use AI tools to genuinely help customers. → `trust_4`
18. I consider AI systems to be reliable. → `trust_5`

---

## **Section 5: Ease of Interaction (Frustration Avoidance)**

19. It is easy to explain my problem to an AI support system. → `ease_1`
20. AI tools usually understand my requests. → `ease_2`
21. Interacting with AI customer support feels smooth. → `ease_3`
22. AI-based systems guide me well through the process. → `ease_4`
23. I get my issues resolved efficiently with AI. → `ease_5`

---

## **Section 6: Preference for AI vs. Human Support**

24. AI is suitable for handling simple customer service queries. → `pref_1`
25. I prefer AI tools for quick, transactional support. → `pref_2`
26. AI is better suited for FAQs and basic requests than humans. → `pref_3`
27. AI and humans should work together in customer service. → `pref_4`
28. I am open to using AI-based support again in the future. → `pref_5`
29. I feel comfortable using AI tools for customer service. → `pref_6`
30. I would recommend AI-based customer service to others. → `pref_7`

---

## **Section 7: Behavioral Intention**

*(Now clearly labeled and optimized for regression as dependent variable)*

31. I would prefer AI-based support over human support for routine tasks. → `intention_1`
32. I would recommend companies that use AI for customer service. → `intention_2`
33. I will likely continue using AI-based support in the future. → `intention_3`

---

## **Section 8: Demographics (All Categorical, Coded)**

34. What is your age group? → `demo_age`

* Under 18
* 18–24
* 25–34
* 35–44
* 45–54
* 55–64
* 65+

35. What is your gender? → `demo_gender`

* Male
* Female
* Non-binary
* Prefer not to say

36. What is your highest completed level of education? → `demo_edu`

* High school
* Some college
* Bachelor’s degree
* Master’s degree
* Doctorate
* Prefer not to say

37. Which region are you currently living in? → `demo_region`

* Africa
* Asia
* Europe
* North America
* South America
* Oceania

38. How comfortable are you with new technologies? → `demo_techcomfort`

* Very comfortable
* Somewhat comfortable
* Neutral
* Somewhat uncomfortable
* Very uncomfortable

---

## Key Export/Analysis Guidance

| Variable Type            | Variable Labels              | Analysis Use                         |
| ------------------------ | ---------------------------- | ------------------------------------ |
| Likert Items             | `helpful_1` to `intention_3` | Mean scores, correlation, regression |
| Categorical Demographics | `demo_*`                     | Grouping factors / ANOVA             |
| Screening Variables      | `ai_experience`, etc.        | Filters, grouping, exclusions        |

---

## Implementation Tips

* all Likert questions to **“Required”**
* The **numeric values** (1 to 5) for Excel or CSV export
* variable labels (`trust_2`, `intention_1`, etc.) for column headers in data analysis in Excel or CSV file

