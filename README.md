# Data Consulting Job/Assignment 

For this job/assignment, I was assigned to look into 4 things 
1. Estimation value of Sigma Learn
2. Birth rates and how it relates to primary school education
3. Markov chain to analyse the flow between the different type of schools 
4. Competitor analysis 

# Summary of the Folder 

- `data` folder contains the data I used for the analysis 
- `plots` contains the plots generated 
- `notebooks` contains the key notebooks involved in analysis and consulting 
    - `birth-rate-forecasting.ipynb` is the notebook where I train the time series model to predict the birth rate 
    - `data-consulting.ipynb` is the notebook where I provide analysis and market recommendation based on specifications of the assignment   

# Methodology Used 

For birth rates, I obtained data from the National Population Statistics from a Thai website which I had to clean and reformat. 
I visualised the trend of birth rates from around 2004 to 2025 in this current month. In addition to that, I also trained a time series model using XGboost to try to forecast the birth rates in the 2 years to come 

It was hard to find the actual population of students in each of the 3 school types I estimated the probability students are in each school by multiplying the probability of the school type as a proportion of all schools and the total number of primary school students in Thailand. For the markov chain itself, obtain the actual transition probabilities was immensely difficult as well so I have qualitative indicators and reasonings 

For the competitor analysis, I carried out competitor analysis is mostly all markets and identified the greatest competitor

# Thoughts in the Project 

Thing that held me back the most was the lack of data and information out there. It was hard to find actual values and actual prices of products. Some values and statistics required payment and some companies are not transparent with their pricing. 
Project was still fun and learnt alot. 

