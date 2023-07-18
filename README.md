# SpaceX launch analysis

**Capstone project from IBM Data Science Professional Certificate on Coursera.**

This project served as an opportunity for me to apply the skills I acquired during the various courses I completed over a span of approximately five months. By utilizing real-world datasets, I extracted, cleaned, explored, and analyzed data to gain valuable insights.

## Problem Statement

SpaceX has achieved remarkable success due to the cost-effectiveness of its rocket launches. The company promotes the Falcon 9 rocket launches on their website, advertising a price of $62 million, while other providers spend more than $165 million for each launch. This substantial cost-saving is primarily attributed to SpaceX's ability to reuse the first stage of their rockets. Consequently, determining whether the first stage will land successfully becomes crucial in estimating the launch cost.

The Falcon 9 launch process follows a standard rocket pattern consisting of two stages. 

![image](https://github.com/julionakama/SpaceX_Launch_Analysis/assets/123141709/3f486e7f-e248-43fc-8c48-fd82b069cfd6)

The payload is secured within the fairings, and the second stage aids in propelling the payload to orbit, although most of the work is performed by the first stage, which is considerably larger than the second stage. 

Unlike other rocket providers, SpaceX has developed the capability to recover and reuse the first stage, valued at 70% of the total cost of the rocket. However, there are instances where the first stage may not land successfully, resulting in a crash. Additionally, SpaceX may intentionally forgo recovering the first stage based on mission parameters such as payload requirements, desired orbit, or customer preferences.

## Objective
Help a new company (Space Y) determine the price of its rocket launches by compiling and analyzing Space X's track record of success in landing its first stages, creating dashboards and predicting the first stages' reuse with machine learning models.

## Methodology

Key files of interest in this directory are:
wrangle_act.ipynb: code for gathering, assessing, cleaning, analyzing, and visualizing data
wrangle_report.html: documentation for data wrangling steps: gather, assess, and clean
act_report.html: documentation of analysis and insights into final data
twitter_archive_enhanced.csv: Initial dataset
image_predictions.tsv: file downloaded programmatically
tweet_json.txt: file constructed via API
twitter_archive_master.csv: combined and cleaned data

Data Collection from 2 sources - i) SpaceX API & ii) Webscrapping from wikiepdia

Data Wrangling - Collected data was enriched by creating a landing outcome label based on outcome data after summarizing and analyzing features

EDA using SQL & Visualization

Interactive Visual Analysis by creating Dashboard

Machine Learning Predictive Analysis using Classification Models - Data that was collected until this step were normalized, divided in training and test data sets and evaluated by four different classification models (Logistic Regression, Support Vector Model, Decision Tree & K Nearest Neighbours Model), being the accuracy of each model evaluated using different combinations of parameters.

- `1_1_Data_Collection_with_API.ipynb`
- `1_2_Data_Collection_with_Web_Scraping.ipynb`
- `2_Data_Wrangling.ipynb`
- `3_1_EDA_with_SQL.ipynb`
- `3_2_EDA_with_Data_Visualization.ipynb`
- `4_1_Interactive_Data_Analytics_with_Folium.ipynb`
- `4_2_Spacex_Dash_App.py`
- `5_ML_Predictive_Analysis.ipynb`

## Conclusion

- The launch success rate has increased since 2013.
- The success rate improved as the flight number increases in CCAFS SLC 40.
- The site KSC LC-39A has the greatest landing success rate (76.9%).
- Success rates for light payloads launches are higher than the heavy load ones.
- Although few rockets were launched with more than 8,000 kg of Payload Mass, the most successful landing rates are for PO and ISS orbits.
- The site VAFB SLC 4E does not have experience launching rockets with more than 10,000 kg of Payload Mass.
- The orbits ES-L1, GEO, HEO and SSO have a perfect success rate. However, the most relevant is SSO because the other orbits had only one flight.
- Launch sites can be close to railways, highways and coastlines. In contrast, they are far away from the cities.
- For outcome prediction, SVM, KNN, Tree or Logistic Regression models can be used. They all have the same prediction accuracy (83.33%) for this dataset.



