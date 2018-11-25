# TITLE

# Abstract
With increasingly dire climate change forecasts, concerned individuals are asking how they can minimize their carbon footprint. Recent research suggests that reducing one's consumption of meat, in particular beef, is one of the highest impact actions an individual can take. To examine this topic, we will explore the popularity and prevalence of meat in recipes. Specifically, we plan to extract the ingredients from a recipe database and calculate the carbon footprint of recipes 

Finally, we hope to directly relate this data to the issue of climate change by estimating a rating reflecting the carbon footprint of meat in recipes and the environmental impact of consumers' diets. 

# Research questions

1. How can we rate the carbon footprint of the meat in a recipe?

2. Does the recipe rating depend on the presence of meat and the carbon footprint? Are recipes with lower carbon footprints rated higher or lower?

3. What trends emerge by clustering similarly named recipes or recipes with shared tags?

4. Is there any relationship between the carbon footprint or the presence of meat and the publish date?

5. Can we find similar recipes that have lower carbon footprints?

6. What general statements can we conclude from our findings?


# Dataset

We plan to primarily use the "Cooking Recipes" dataset which is 2.5GB and in the form of HTML files. As described in the associated paper's [source](http://infolab.stanford.edu/~west1/from-cookies-to-cooks/), the dataset contains data from 14 distinct high-traffic recipe sites.

To enrich our study, we will have to include datasets on....estimated carbon footprint of ingredients.


# A list of internal milestones up until project milestone 2
Steps accomplished:

1. **Data exploration:**

    a.) Loaded recipe data
    
    b.) Extracted and cleaned data about ingredients and quantities.
    
        -
   
    d.) Categorised meat ingredients in relevant sub-categories. 

2. **Environmental impact:**

    a.) Defined a formula to rate the environmental impact of the meat ingredients in a recipe
  
    b.) Rated and analyze ratings of recipes with meat ingredients.

3. **Nov. 25th - Milestone 2:**

    a.) Redefined which research questions we want to study in depth for the final project submission.
    
    b.) Document our findings for final MS2 submission 
    
    c.) Plan next steps for Milestone 3 and final presentation


# Milestone 2 Update: 

After thoroughly exploring our data we discovered that we do not have the access logs referenced in the original paper so we had to redefine our project scope and goals to focus more fully on the recipe database. Instead of analyzing the consumer trends over time and geographic location, we will examine the meat prevalence in recipes as it relates to rating, publishing date and other recommended recipes. We limited our search to htmls of recipes, filtering out the web pages that have multiple recipes (i.e. "BBQ Recipes for 4th of July", "Salad ideas"). Our method for extracting the quantity of meat is not fool-proof: all quantities are  ....FINISH


# Next Steps: Analysis
Using the cleaned dataframe we created for milestone 2, we will begin analysis

# Questions for the TAs

