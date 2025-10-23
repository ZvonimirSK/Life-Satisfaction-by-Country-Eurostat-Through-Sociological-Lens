# Education, Digital Skills, and Life Satisfaction in Europe (ANCOVA Study, 2023)
This mini-project investigates how educational attainment (Bourdieu’s cultural capital) and digital competence (van Dijk’s digital divide framework) jointly relate to life satisfaction across European countries (EU-SILC & DESI 2023).
An Analysis of Covariance (ANCOVA) was used to test whether differences in life satisfaction between education levels remain significant after controlling for national digital skills.

# Theoretical Background

Bourdieu (1986) — Cultural capital in the form of education shapes access to symbolic and material resources, influencing subjective well-being.

van Dijk (2007) — Digital divide theory extends capital logic to digital participation: access, skills, and outcomes produce new social inequalities.

Digital capital therefore represents an additional dimension of stratification within Bourdieu’s framework.

Wallerstein (1974) — World-systems theory provides the macro-structural lens: countries differ in their integration into the “core–periphery” digital economy.
Future extensions of this analysis will test this spatial hypothesis using NUTS2 regional data.

# Research Questions & Hypotheses

| Research question                                                         | Null hypothesis (H₀)                                 | Alternative hypothesis (H₁)                                                 |
| ------------------------------------------------------------------------- | ---------------------------------------------------- | --------------------------------------------------------------------------- |
| RQ1. Are there differences in life satisfaction between education levels? | No mean differences across ISCED groups.             | Higher education predicts greater life satisfaction.                        |
| RQ2. Is national digital competence related to life satisfaction?         | No association.                                      | Higher *above-basic digital skills* correspond to higher life satisfaction. |
| RQ3. Does education moderate this relationship?                           | No interaction between education and digital skills. | The effect of digital skills varies by education group.                     |

# Data and Operationalization
| Variable                     | Source                    | Type                         | Description                                                    |
| ---------------------------- | ------------------------- | ---------------------------- | -------------------------------------------------------------- |
| `life_satisfaction`          | EU-SILC 2023              | Dependent variable           | Weighted index 1 = Low, 2 = Medium, 3 = High life satisfaction |
| `edu_group`                  | EU-SILC 2023              | Factor (IV)                  | Education levels (ISCED 0–2, 3–4, 5–8)                         |
| `above_basic_digital_skills` | DESI 2023                 | Covariate                    | % of population with advanced digital skills                   |

Unit of analysis is country × education level, Europe 2023
# ANCOVA
