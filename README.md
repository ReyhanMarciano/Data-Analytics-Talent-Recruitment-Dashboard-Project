***
Disclaimer: The company name "SearaBank" and the associated business scenario used in this project are entirely fictional and modeled for educational purposes as part of a structured case study brief. Any resemblance to actual companies, institutions, or real data is purely coincidental.
***

# SearaBank Talent Recruitment Dashboard 2026 

## Project Overview
In the fast-growing digital banking sector, talent acquisition efficiency directly impacts business agility and risk mitigation. This project focuses on analyzing recruitment data for SearaBank, a branchless digital bank operating via the Searah Mobile application. 

By conducting an end to end data analytics workflow from data cleaning and unpivoting complex candidate skill profiles in Google Sheets to building an interactive recruitment dashboard in Looker Studio, this project serves as a data driven screening solution to help HR accelerate time to hire and execute precision talent mapping.

## Business Problem
SearaBank's HR department is overwhelmed by manual resume screening and currently is facing a high organizational turnover and an urgent need for workforce expansion in 2026 due to flagship product growth (Seara Hub Pockets and Seara Smart-PayLater). They lack data visibility to quickly match applicants against strict, tier specific tool requirements needed for critical squad vacancies.

*   Recruitment Demands & Qualifications:
    To support operations, management has established a highly specific recruitment headcount allocation and technical requirements:
    *   Manpower Allocation:
        *   1 Senior Credit Risk Analyst allocated to the PayLater Squad.
        *   3 Junior Data Analysts distributed as follows:
            *   1 position for the PayLater Squad.
            *   2 positions for the Pockets Squad.
    *   Qualification:
        *   Senior Position: Candidates are expected to behave as experienced talent and must demonstrate technical mastery in upstream data engineering tools, specifically SQL and Python.
        *   Junior Position: Candidates are evaluated based on entry-level competency and are expected to focus on downstream business intelligence and data reporting tools, specifically Microsoft Excel and BI Platforms.

## Objective
To analyze candidate profiles, technical competencies, and application sources in order to automate early stage candidate screening, ensure an objective data driven recruitment process, and precisely fulfill targeted squad resource quotas.

## Key User Questions
*   What does the competency map look like for applicants regarding Excel and our multi-platform BI tools? In which specific platform do we have the highest concentration of potential top-tier junior talent to fulfill our squad needs?
*   Are Fresh Graduate applicants capable of matching the technical test pass rates for critical upstream tools (SQL and Python) when compared to Experienced candidates?

## Tech Stack & Tools Used
*   Data Cleaning & Transformation: Google Sheets
*   Data Visualization & Dashboarding: Google Looker Studio

## Project Workflow

1. Data Cleaning & Preprocessing (Google Sheets)
   *   Handled missing dataset records by replacing empty values with "-".
   *   Removed duplicates and performed text-casing standardization utilizing =PROPER and =REGEXREPLACE.
   *   Conducted geographic segmentation by grouping candidate locations by province using =IF and =VLOOKUP.

2. Data Transformation & Feature Engineering
   *   Wide-to-Long Text Transformation: Addressed the challenge of multi response string values in columns for candidate skills and motivations.
   *   Boolean Mapping: Applied a combination of =IF and =REGEXMATCH to split and convert text fields into distinct boolean columns, preparing the backend dataset for seamless data aggregation and accurate visualization filtering.

3. Exploratory Data Analysis (EDA)
   * Candidate demographic analysis
   * Competency level analysis
   * Recruitment source channel analysis
   * Cancicate motivation analysis

4. Dashboard Development
   * Designed interactive dashboard using Looker Studio.
   * Visualize data to support talent recruitment decision making

## Key Insights
### Talent Pool & Sourcing Channels: 
   * 56.7% of the 681 total applicants are Fresh Graduates, indicating an abundant supply of talent in the entry level market.
   * LinkedIn is the single most effective sourcing channel, attracting 80.6% of all applicants.
   * Candidate distribution remains heavily centralized in Java (led by West Java with 173 applicants and DKI Jakarta with 112).
### Skills & Multi-Platform BI Competency:
   * SQL (561 candidates) and Python (549 candidates) are the most widely mastered upstream technical skills among applicants.
   * For downstream BI tools, Power BI leads with 516 candidates, followed by Tableau (446) and Looker Studio (401).
    *   Among Fresh Graduates meeting junior criteria, the combination of Excel + Tableau heavily dominates with 224 candidates, drastically outnumbering Excel + Power BI (41) and Excel + Looker Studio (13).
### Upstream Level Skill Competitiveness:
   * Remarkably, 300 Fresh Graduate candidates successfully passed senior-level technical criteria (SQL & Python), proving that upstream technical proficiency is highly competitive among entry-level talent compared to the 203 qualified Experienced candidates.

## Strategic Business Recommendations

### 1. Fulfilling the Junior Data Analyst Quota (3 Positions)
*   PayLater Squad (1 Position needed): Streamline hiring by prioritizing candidates from the Excel + Tableau segment, leveraging the largest pool of qualified talent (224 candidates).
*   Pockets Squad (2 Positions needed): Since candidates with Power BI (41) and Looker Studio (13) competencies are highly limited, HR must fast-track the screening process for these specific clusters. Target the 69 Qualified Junior candidates as the primary funnel for immediate placement.

### 2. Fulfilling the Senior Credit Risk Analyst Quota (1 Position)
*   While Fresh Graduates show exceptional technical test scores in SQL and Python (300 candidates), it is highly recommended to prioritize the Experienced candidate pool (203 individuals) for final interviews. This high-risk position within the PayLater team requires deep contextual business expertise in risk management that goes beyond technical test performance.

## Dashboard Preview
![Searabank Talent Recruitment Dashboard](Dashboard/Searabank%20Talent%20Recruitment%20Dashboard.jpg)
