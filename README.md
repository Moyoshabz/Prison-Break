# Helicopter Prison Escape Analysis

![iamge_1](./images2/prisonbreak.jpg)

# Hey There!,

## Project Overview
This project analyzes historical data on helicopter prison escape attempts, sourced from [Wikipedia](https://en.wikipedia.org/wiki/List_of_helicopter_prison_escapes#Actual_attempts). The analysis answers key questions such as:

1. **In which year did the most helicopter prison escape attempts occur?**
2. **In which countries do the most attempted helicopter prison escapes occur?**
3. **In which countries do helicopter prison breaks have a higher chance of success?**
4. **How does the number of escapees affect the success of an escape?**
5. **Which escapees have done it more than once?**
   
  **Bonus**
  
6. **Dashboard with Key Statistics of the Analysis.**


The analysis includes data cleaning, exploration, visualization, and a summary presented on a Python-generated dashboard.

## Prerequisites
Ensure you have the following installed on your machine:

- Python 3.x
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  - `helper.py` 
  - `matplotlib`
  - `seaborn`
  - `dash`
 
## Analysis Process

### 1. Data Collection
The data was scraped from the Wikipedia page "[List of helicopter prison escapes](https://en.wikipedia.org/wiki/List_of_helicopter_prison_escapes#Actual_attempts)" and imported into a Jupyter Notebook for analysis.

---

### 2. Data Cleaning
Steps:
- Removing/dropping column(s).
- Adopted imputation for missing prisoner name
- Converted date fields to year objects for easy analysis.
  
---
### 3. Data Exploration and Visualization

#### Question 1: In which year did the most attempts occur?
- Grouped the data by year and counted the number of attempts.
- Find the Max and Min Year
- Created a bar chart to visualize the trends over time.

![iamge_1](./images2/stat.png)

The year with the most helicopter prison escape attempts was **1971**. This year saw the escape of **Joel Kaplan** from the Santa Martha Acatitla prison in Mexico City, using a helicopter. Kaplan and his cellmate boarded the helicopter in a daring escape that inspired the book **The 10-Second Jailbreak and the movie Breakout (1975).**
![iamge_1](./images2/movieposter.jpg)


![iamge_1](./images2/image0.png)

---

#### Question 2: In which countries do the most attempted helicopter prison escapes occur?
- Counted the number of attempts per country.
- Visualized the results using a table.

**France** had the highest number of attempted helicopter prison escapes.

![iamge_1](./images2/image4.png)

---

#### Question 3: In which countries do helicopter prison breaks have a higher chance of success?
- Calculated the success rate of escapes per country.
- Used a bar chart to show success rates.

**France** also had the highest success rate for helicopter prison escapes

![iamge_1](./images2/france.png)
![iamge_1](./images2/image1.png)

---

#### Question 4: How does the number of escapees affect the success?
- Analyzed the relationship between the number of escapees and the success of the escape.
- Created a scatter plot to illustrate the correlation and trend.

Analysis revealed a **positive** correlation between the number of escapees and the success rate.

![iamge_1](./images2/table.png)

![iamge_1](./images2/image2.png)


#### Question 5: Which escapees have done it more than once?
- Analyzed the prisoners who had escaped more than once.
- Created a barchart plot to illustrate the trend.

This analysis was **inconclusive** due to missing data. The names of the escapees in certain records were marked as “--” .
Missing data was imputed as **"Unknown"** for this analysis, but further research is required to validate results.

![iamge_1](./images2/image3.png) 

---

### 4. Dashboard Creation
A summary dashboard was built using Dash to present:
- Key statistics.
- Static visualizations for exploring the data.

![iamge_1](./images2/download.png)
