# Who are the carnivores?

# Abstract

With increasingly dire climate change forecasts, concerned individuals are asking how they can minimize their carbon footprint. Recent research suggests that reducing one's consumption of meat, in particular beef, is one of the highest impact actions an individual can take. To examine this topic, we will explore the trends in meat consumption in the U.S. by analyzing the prevalence of meat in recipes frequented online. Specifically, we plan to extract the ingredients, time and location of clicks from a recipe database. Using this information, we will explore the link between meat consumption and various key factors such as time of year, rural and urban locations, average regional income or historic events (i.e. the Paris Climate Agreement, mad cow disease outbreak). Finally, we hope to directly relate this data to the issue of climate change by estimating a rating reflecting the carbon footprint of meat in recipes and the environmental impact of consumers' diets. 


# Research questions

1. How can we rate the carbon footprint of the meat in a recipe?

2. How does meat consumption vary between different regions?

3. How does meat consumption vary over time?

4. How does meat consumption vary with temperature and season?

5. Example questions to characterize the carnivores further:

    a.) Is the hypothesis that rich people eat more meat valid?
    
    b.) Does rural or urban population eat more meat?
    
    c.) Is the meat consumption affected by media coverage of animal diseases or environmental effects?

6. What general statements can we conclude from our findings?


# Dataset
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

We plan to use the "Cooking Recipes" dataset. As described in the associated paper's [source](http://infolab.stanford.edu/~west1/from-cookies-to-cooks/), the dataset contains data from 14 distinct high-traffic pages. As the websites are in English, we decided to focus our project on the US where the number of clicks would be more representative than in a non-English speaking country. 
As we want to focus on meat ingredients, we checked that ingredients are tagged in HTML, then we'll have to categorise such ingredients in sub-categories (poultry, beef, fish, etc.). We will mostly focus on ingredients and quantities (which might need to be converted to metric) and might consider ratings. We will also look into number and geo-location of clicks on the recipes. 

To enrich our study, we will have to include datasets on the US population including geographical location and/or income. We will also link in media coverage of food-related topics such as animal disease or environmental issues such as climate agreements or elections. To do this we will either identify a set of events we deem relevant and attempt to observe the effects in the data, or examine the data and search for possible explanations of the trends. Finally, we can also study the relationship between meat consumption and food costs as found in [the USDA database](https://www.ers.usda.gov/data-products/fruit-and-vegetable-prices/fruit-and-vegetable-prices/#Vegetables). 

# A list of internal milestones up until project milestone 2

1. **Nov. 11th - Data exploration:**

    a.) Load recipe data
    
    b.) Transfer any relevant data from HTML files into a treatable data form such as dataframes
    
    c.) Extract and clean data about ingredients, quantities, number of clicks, regional and time information
   
    d.) Categorise meat ingredients in relevant sub-categories. 

2. **Nov. 15th - Environmental impact:**

    a.) Define a formula to rate the environmental impact of the meat ingredients in a recipe
  
    b.) Rate and analyze ratings of recipes with meat ingredients.

3. **Nov. 18th - Meat consumption:**

    a.) Quantify the meat consumption regionally and over time in the US
    b.) Look at different levels of granularity in the geographical information (state, cities, suburbs).

4. **Nov. 23rd - The Carnivores:**

    Characterize the meat eating population (carnivores) by anlyzing the research questions
    
    a.) Find relevant datasets to answer research questions (if applicable)
    
    b.) Use our datasets to reevaluate our research questions and hypotheses
    
5. **Nov. 25th - Milestone 2:**

    a.) Define which research questions we want to study in depth for the final project submission.
    
    b.) Document our findings for final MS2 submission 
    
    c.) Plan next steps for Milestone 3 and final presentation

# Questions for TAa

1. Do you think this project is too ambitious for us? (Please note that we are "beginners" in data science)

2. What would be the smartest way to access the information from so many html files?
