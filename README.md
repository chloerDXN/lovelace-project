# Meet the meat

# Abstract
With increasingly dire climate change forecasts, concerned individuals are asking how they can minimize their carbon footprint. Recent research suggests that reducing one's consumption of meat, in particular beef, is one of the highest impact actions an individual can take. To examine this topic, we will explore the popularity and prevalence of meat in recipes. 

For this project, we extracted data from nearly 30'000 recipes in order to understand whether the presence of meat influenced the popularity of a recipe and whether it is possible to suggest similar recipes with a lower carbon footprint. 

# Research questions

1. Is there any correlation between the recipe ratings and its carbon footprint? Are recipes with lower carbon footprints rated higher or lower?

2. What are the average/median quantities of meat in recipes and how do they influence the overall carbon footprint of the recipe?

2. What trends emerge by clustering similarly named recipes or recipes with shared tags?

3. Can we find similar recipes that have lower carbon footprints?

4. What general statements can we conclude from our findings?


# Dataset

We used the "Cooking Recipes" dataset which is 2.5GB and in the form of HTML files. As described in the associated paper's [source](http://infolab.stanford.edu/~west1/from-cookies-to-cooks/), the dataset contains data from 14 distinct high-traffic recipe sites. Each site typically has a different format which we did our best to document in order to extract the necessary information. Some html files lead to recipes that are grouped together strangely and which we ignored. In our final dataset, we have kept recipes from four websites which all had common data we used for our analysis such as ratings and serving size.

To enrich our study, we included a dataset from the [Environmental Working Group’s Meat Eater’s Guide](http://static.ewg.org/reports/2011/meateaters/pdf/methodology_ewg_meat_eaters_guide_to_health_and_climate_2011.pdf) which estimates the CO2 equivalent footprint that results from the growth, processing and transportation of food. The dataframe we used is a selection from the top 8 worst foods to consume in terms of carbon equivalent impact. We also considered as "meat" other animal protein sources such as cheese and eggs which also have a high environmental impact.

# A list of internal milestones up until project milestone 3
Steps accomplished:

1. **Data exploration:**

    a.) Loaded recipe data on the full dataset (around 30'000) points
    
    b.) Extracted and cleaned data about ratings and serving size
   
    c.) Extracted tags from some websites then dropped this field of research as it was not compatible with many webiste formats
    
    d.) Saved the dataset as CSV to upload it in data analysis notebook

2. **Data Analysis:**

    a.) Performed statistical analysis of our dataset
    
    b.) Analysed the relationships between ratings and meat ingredients
    
    b.) Analysed the prevalence of different types of meat in recipes by extracting median amounts of meat ingredients
    
    c.) Clustered the recipes by title and analysed the relationships with ratings
  
3. **Dec. 16th - Milestone 3:**

    a.) Redefined our research questions in accordance with the extracted data
    
    b.) Documented our findings for final MS3 submission 
    
    c.) Planned next steps for final presentation


# Milestone 3 Update: 

For Milestone 3, we refined our data extraction and performed the extraction on the full dataset. From the original 90'000 files we managed to extract 30'000 recipes with data satisfying our analysis goals. We saved our new dataset to a CSV file in order to upload it into a new data analysis notebook (our submission for MS3).

Through basic statistical analysis, we realised some datapoints had exagerated carbon footprints as a result from our data extraction methods. We discovered that the carbon footprint of a recipe had little influence on the overall ratings, however, the lowest impact recipes have the bet rating, meaning we wouldn't feel bad suggesting a recipe having a lower footprint to a user willing to lower their cooking impact. Through clustering, we discovered main groups of recipes, whether types of dishes with a small amount of clusters or more in detail types of dishes with a large amount of clusters.


# Next Steps: Preparing poster presentation

For the poster presentation, we would like to find new ways to visualise our data in a meaningful way as well as extract more information about the carbon footprint per meat ingredient. 

1.) Extract carbon footprint per ingredient per recipe 

4.) Formalize "story" relevant to a poster presentation

5.) Prepare presentation and final poster

# Contributions of group members
Alex: Clustering and extract ratings
Nadine: Statistical analysis
Chloe: Extract tags and meat ingredient analysis
