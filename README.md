# Data Science job Analysis: São Paulo version
I first start understanding a model developed by Ken Jee and then I apply to São Paulo, Brazil.
## References
**Ken Jee's channel**:https://www.youtube.com/playlist?list=PL2zq7klxX5ASFejJj80ob9ZAnBHdz5O1t

**Model Reference:** https://github.com/PlayingNumbers/ds_salary_proj

**Web Scrapper (code):** https://github.com/arapfaik/scraping-glassdoor-selenium

**Web Scrapper (article):** https://towardsdatascience.com/selenium-tutorial-scraping-glassdoor-com-in-10-minutes-3d0915c6d905

# Project Steps
## Planning
## Data collection
## Data cleaning
Cleaning strategy
  - Salary: 
     - Remove (Glassdoor est.)
     - Remove df['Salary Estimate'] == -1
     - Remove $ and K
     - Create a column for 'Per hour': 1 if it is true, 0 if it is false
     - Create a column for 'Provided by employee': 1 if it is true, 0 if it is false
     - Create a column 'min_salary'
     - Create a column 'max_salary'
     - Create a column 'avg_salary'
  - Company name: remove the rating (text only)
      - My case, I have to remove /n as well
      - Job description: highlight the requirements (python, etc..)
  - State field
      - Split State and City in Location column
      - job_location and company_headquarters is in the same state: I decided to split Headquarters and get the state before compating.
      - Create a column 'same_state': 1 if it is true, 0 if it is false
   - Age of company
      - df['Founded'] == -1 : the company didn't provied the foundation year
   - Job description: I would you the tool from news categorization
## Exploratory Anaylsis
## Modeling
