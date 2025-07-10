# Title: Mental Health and Screen Time in Youth
# Objective: Looking at the intersection of and possible relationship(s) between mental health and screen time in children to young adults (age <30ish).
# Data source: Kaggle
https://www.kaggle.com/datasets/aniruddhawankhede/mental-heath-analysis-among-teenagers (Direct mental health/screen time w/ ages 13-18 (15.5 yr mean))
  Data Type(s): User ID is an integer (numeric). Age is an integer (numeric). Gender is categorical (string). Social media hours is a float (numeric). Excersize hours is a float (numeric). Sleep hours is a float (numeric). Screen time hours is a float (numeric). Survey stress score is an integer (numeric, ordinal). Wearable stress score (stress measured by wearable devices) is a float (numeric). Support system is categorical (string).
  Restrictions: Age range of 13-18 is limited. Changes are not tracked over time. Wearable stress scroe range uses a different scale than survey. No geographic or demographic context is provided.
  Pros: Histogram shows minimal variation between age groups, which is ideal because there is no age bias in the data. No missing values. Float values easy to clean. Can handle mixed data types (floats and integers) in the same dataset. Large sample size (5000 participants). Age range 13-18 is highly relevant for screen time research. Clean, well-structured dataset with clear variable definitions. 
  Cons: Will need to clean the dataset of every column except for age, screen time hours, and survey stress score. Limited age range may not generalize to broader population. Confounding variables such as exercise and sleep are not being analyzed by could influence results. 
# Data pulling (where/how did you get it?): Kaggle. 
# Data cleaning (what choices did you make/what was selected/deleted and why?):
  We chose to remove every column except for age, screen time hours, and survey stress score by selecting only these three for a new dataframe. We did this because these three columns are the only ones necessary for our data analysis, and the other columns only crowd the data. Screen time hours is a float by default, so we wanted to round these numbers to the nearest integer to match the other variables. We did this by using the .astype('int') function on our new dataframe.
# Visualization reflections:
# Insights (Where is this helpful? What conclusions should be drawn?):
