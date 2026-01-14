# Key Resume Attributes Impacting Job Callbacks

This repository contains the data analysis with causal inference techniques and code for the final project of **Stanford University's STATS 209: Causal Inference**. This study revisits the landmark research by Bertrand and Mullainathan (2004) regarding labor market discrimination, applying modern causal inference frameworks to evaluate how race and gender impact job application callback rates.

## Project Overview

The primary goal was to determine if observed differences in callback rates are causally linked to race and gender perception or influenced by other covariates. We utilized a dataset of fictitious resumes sent to help-wanted ads in Boston and Chicago, where names were randomly assigned to suggest specific racial and gender identities (e.g., "Emily" vs. "Lakisha").

### Key Questions

* Does the perception of race (White vs. African American) significantly impact callback rates? 


* Does gender (Male vs. Female) serve as a primary driver for callbacks? 


* How does resume quality interact with race and gender to influence employer interest? 



---

## Methods

We employed several statistical frameworks to ensure a robust assessment of causal impacts:
* **Fisher’s Randomization Test (FRT):** Used to test the sharp null hypothesis of no treatment effect through permutation-based distributions.

* **Neyman’s Causal Inference:** Used to estimate the Average Treatment Effect (ATE) and construct 95% confidence intervals.

* **Stratification:** Analysis was performed across different industries (e.g., Manufacturing, Finance, Wholesale) to identify sector-specific biases.

* **Matched Pairing:** We utilized propensity score matching to compare similar candidates and isolate the effects of race, gender, and resume quality.


---

## Key Findings

### 1. Racial Discrimination

We found **strong evidence** of racial disparities in callback rates.

* FRT for race yielded a remarkably small p-value (), providing robust evidence against equal callback rates.


* Neymanian inference confirmed a significant treatment effect, with a 95% confidence interval for race between 0.0168 and 0.0473 (excluding zero).



### 2. Gender Dynamics

While the overall impact of gender appeared insignificant, the data revealed nuances related to occupational segregation:

* The overall p-value for gender was 0.379, failing to reject the null hypothesis.


* However, the dataset was heavily skewed, with significantly more women applied to traditionally "feminine" roles like secretarial and clerical positions.



### 3. Industry Specifics

Racial disparities were most pronounced in specialized or high-professionalization sectors:

* Significant differences were found in **Finance, Insurance, and Real Estate**, **Business and Personal Service**, and **Wholesale and Retail Trade**.



### 4. Resume Quality Payoff

Resume quality does not benefit everyone equally:
* **White women** benefit the most from higher quality resumes.

* **Black men** benefit the least, with results suggesting that employers may discount their credentials.

* **Black women** likely benefit from a better resume more than black men, though their average effect is still less than half that of white women.


---

## Conclusion

Our analysis confirms that racial discrimination remains a persistent barrier in the labor market. While gender differences in callbacks were less apparent, the study highlights how occupational segregation and the "discounting" of credentials for minority groups complicate the hiring landscape.

## Authors

* **Allie Kika Cemalovic** (Ph.D. Civil Engineering, Stanford) 


* **Mitty Yu** (M.S. ICME Data Science, Stanford) 


* **Qingqing Yu** (M.S. ICME MCF, Stanford) 
