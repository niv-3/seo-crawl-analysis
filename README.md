\# SEO Crawl Analysis with Python



\## Overview



This project explores how changes in sitemap inclusion relate to Googlebot crawling behaviour across groups of web pages.



Using Python and pandas, I cleaned and analyzed crawl data, compared page groups across different time periods, normalized crawl activity to account for group-size differences, and used visualizations and robustness checks to evaluate whether observed changes were meaningful.



The project demonstrates practical data-analysis skills including data cleaning, exploratory analysis, metric definition, time-series analysis, comparison groups, visualization, and interpretation of results.



\## Business Question



The analysis investigates whether changes in sitemap inclusion are associated with changes in Googlebot crawl frequency.



The main questions were:



\- How frequently does Googlebot crawl the analyzed pages?

\- Does crawl behaviour change after sitemap-related changes?

\- Are the observed changes different from pages used as a comparison group?

\- Do the results remain consistent when equivalent time periods are compared?

\- Are there other page characteristics that could help explain the observed behaviour?



\## Tools \& Technologies



\- Python

\- pandas

\- NumPy

\- Matplotlib

\- Jupyter Notebook

\- Data cleaning and transformation

\- Time-series analysis

\- Exploratory Data Analysis (EDA)



\## Analysis Workflow



\### 1. Data Preparation



The source data was cleaned and transformed into an analysis-ready structure.



This included:



\- parsing dates

\- grouping observations

\- identifying relevant page groups

\- preparing crawl-frequency metrics

\- checking page characteristics



\### 2. Crawl-Frequency Analysis



Googlebot crawl activity was analyzed across the different page groups.



To make groups of different sizes comparable, crawl activity was normalized using metrics such as crawls per page per day rather than relying only on raw crawl counts.



\### 3. Before vs. After Comparison



Crawl behaviour was compared across periods before and after the relevant sitemap changes.



The analysis examined whether the affected page group experienced a meaningful change relative to the comparison group.



\### 4. Daily Trends



Daily crawl behaviour was visualized to identify changes over time.



A 7-day rolling average was also used to reduce daily noise and make the underlying trend easier to interpret.



\### 5. Robustness Check



To reduce the risk of drawing conclusions from unequal time windows, I repeated the comparison using matched 17-day periods.



In this comparison:



\- the sitemap-related group showed approximately a \*\*27.8% decline\*\*

\- the comparison group remained relatively stable at approximately \*\*0.6% decline\*\*



This strengthened the evidence that the groups behaved differently during the analyzed period.



\## Interpretation



The analysis identified a substantial difference in crawl behaviour between the sitemap-related pages and the comparison group.



However, the results should not be interpreted as proof that the sitemap change itself caused the decline.



Other technical, temporal, or page-level factors could contribute to the observed behaviour.



The analysis therefore treats the result as an observed association that would require additional evidence or experimentation before making a causal claim.



\## Additional Analysis



The notebook also explores:



\- category-level crawl behaviour

\- page-level characteristics

\- meta-robots information

\- differences between page groups

\- alternative time-window comparisons



These checks were used to better understand the data and test whether the primary result was robust.



\## Key Skills Demonstrated



\- Python data analysis

\- pandas data manipulation

\- Metric definition and normalization

\- Time-series analysis

\- Before/after measurement

\- Comparison-group analysis

\- Data visualization

\- Robustness testing

\- Translating analytical results into business conclusions

\- Distinguishing correlation from causation



\## Repository Structure



```text

seo-crawl-analysis/

│

├── README.md

├── seo\_crawl\_analysis.ipynb

└── .gitignore

```
## Data



The original source dataset is not included in this public repository.



This repository is intended to demonstrate the analytical methodology, code structure, visualizations, and interpretation rather than redistribute the source material.



\## About Me



I am an MSc Computational Sciences student at Freie Universität Berlin with a BSc in Computer Science. My interests include data analytics, SQL, Python, business intelligence, product analytics, and building data-driven solutions.



More projects are available on my GitHub profile:



https://github.com/niv-3



