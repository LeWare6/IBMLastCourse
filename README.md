# SpaceX launch analysis

**Capstone project from IBM Data Science Professional Certificate on Coursera.**

This project served as an opportunity for me to apply the skills I acquired during the various courses I completed over a span of approximately five months. By utilizing real-world datasets, I extracted, cleaned, explored, and analyzed data to gain valuable insights.

## Problem Statement

SpaceX is successful because their rocket launches are relatively inexpensive. SpaceX advertises Falcon 9 rocket launches on its website with a cost of 62 million dollars; other providers cost upwards of 165 million dollars each, much of the savings is because SpaceX can reuse the first stage. Therefore, if we can determine if the first stage will land, we can determine the cost of a launch. Spaces X’s Falcon 9 launch like regular rockets. There are three stages of a rocket launch. The payload is enclosed in the fairings. Stage two, or the second stage, helps bring the payload to orbit, but most of the work is done by the first stage. This stage does most of the work and is much larger than the second stage. This stage is quite large and expensive. Unlike other rocket providers, SpaceX's Falcon 9 can recover the first stage. Sometimes the first stage does not land. Sometimes it will crash. Other times, Space X will sacrifice the first stage due to the mission parameters like payload, orbit, and customer.

In this project, you will take the role of a data scientist working for a new rocket company - Space Y that would like to compete with SpaceX founded by Billionaire industrialist Allon Musk. My job is to determine the price of each launch. I did this by gathering information about SpaceX and creating dashboards for the team. I also determined if SpaceX will reuse the first stage. Instead of using rocket science to determine if the first stage will land successfully, I trained a machine learning model and use public information to predict if SpaceX will reuse the first stage.

Key files of interest in this directory are:
wrangle_act.ipynb: code for gathering, assessing, cleaning, analyzing, and visualizing data
wrangle_report.html: documentation for data wrangling steps: gather, assess, and clean
act_report.html: documentation of analysis and insights into final data
twitter_archive_enhanced.csv: Initial dataset
image_predictions.tsv: file downloaded programmatically
tweet_json.txt: file constructed via API
twitter_archive_master.csv: combined and cleaned data


