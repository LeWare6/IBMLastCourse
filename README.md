# SpaceX launch analysis

This project served as an opportunity for me to apply the skills I acquired during the IBM Data Science Professional Certificate I completed over a span of approximately five months. By utilizing real-world datasets, I extracted, cleaned, explored, and analyzed data to gain valuable insights.

## Problem Statement

SpaceX has achieved remarkable success due to the cost-effectiveness of its rocket launches. The company promotes the Falcon 9 rocket launches on their website, advertising a price of $62 million, while other providers spend more than $165 million for each launch. This substantial cost-saving is primarily attributed to SpaceX's ability to reuse the first stage of their rockets. Consequently, determining whether the first stage will land successfully becomes crucial in estimating the launch cost.

The Falcon 9 launch process follows a standard rocket pattern consisting of two stages. 

![image](https://github.com/julionakama/SpaceX_Launch_Analysis/assets/123141709/3f486e7f-e248-43fc-8c48-fd82b069cfd6)

The payload is secured within the fairings, and the second stage aids in propelling the payload to orbit, although most of the work is performed by the first stage, which is considerably larger than the second stage. 

Unlike other rocket providers, SpaceX has developed the capability to recover and reuse the first stage, valued at 70% of the total cost of the rocket. However, there are instances where the first stage may not land successfully, resulting in a crash. Additionally, SpaceX may intentionally forgo recovering the first stage based on mission parameters such as payload requirements, desired orbit, or customer preferences.

## Objective
Help a new company (Space Y) determine the price of its rocket launches by compiling and analyzing Space X's track record of success in landing its first stages, creating dashboards and predicting the first stages' reuse with machine learning models.

## Methodology

The project was developed in Python using different libraries such as _BeautifulSoup, Pandas, Sqlite3, Numpy, Seaborn, Folium_ and _Dash_.

More detail about the methodology and most important results of each stage can be found in the following presentation: `Presentation_Winning_Space_Race_with_Data Science.pdf`

#### Data Collection
- Using SpaceX API: `1_1_Data_Collection_with_API.ipynb`
- Performing Web Scraping with BeautifulSoup on Wikipedia: `1_2_Data_Collection_with_Web_Scraping.ipynb`

#### Data Wrangling
- One hot encoding was applied to categorical values, and data cleaning of null values and non-relevant columns: `2_Data_Wrangling.ipynb`

#### Exploratory Data Analysis (EDA)
- Performing SQL queries: `3_1_EDA_with_SQL.ipynb`
- Creating visualizations with Seaborn: `3_2_EDA_with_Data_Visualization.ipynb`

#### Interactive Visual Analytics
- Building an interactive map with Folium: `4_1_Interactive_Data_Analytics_with_Folium.ipynb`
- Build a Dashboard with Plotly Dash: `4_2_Spacex_Dash_App.py`

#### Machine Learning Predictive Analysis
- Training classification models, including Logistic Regression, Support Vector Machine (SVM), Decision Trees and K-nearest neighbours (KNN): `5_ML_Predictive_Analysis.ipynb`


## Conclusions

- The launch success rate has increased since 2013.
- The success rate improved as the flight number increases in CCAFS SLC 40.
- The site KSC LC-39A has the greatest landing success rate (76.9%).
- Success rates for light payloads launches are higher than the heavy load ones.
- Although few rockets were launched with more than 8,000 kg of Payload Mass, the most successful landing rates are for PO and ISS orbits.
- The site VAFB SLC 4E does not have experience launching rockets with more than 10,000 kg of Payload Mass.
- The orbits ES-L1, GEO, HEO and SSO have a perfect success rate. However, the most relevant is SSO because the other orbits had only one flight.
- Launch sites can be close to railways, highways and coastlines. In contrast, they are far away from the cities.
- For outcome prediction, SVM, KNN, Tree or Logistic Regression models can be used. They all have the same prediction accuracy (83.33%) for this dataset.



