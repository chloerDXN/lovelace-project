# TITLE

# Abstract
With increasingly dire climate change forecasts, concerned individuals are asking how they can minimize their carbon footprint. Recent research suggests that reducing one's consumption of meat, in particular beef, is one of the highest impact actions an individual can take. To examine this topic, we will explore the popularity and prevalence of meat in recipes. Specifically, we plan to extract the ingredients, quantities, and ratings from a recipe database and calculate the carbon footprint of recipes. After ranking the data based on this carbon fooprint, we hope to directly relate this data to the issue of climate change by exploring the environmental impact of consumers' diets based on their ingredients.

# Research questions

1. Is there any correlation between the recipe tags and its carbon footprint?

2. Does the recipe rating depend on the presence of meat and the carbon footprint? Are recipes with lower carbon footprints rated higher or lower?

3. What trends emerge by clustering similarly named recipes or recipes with shared tags?

4. Is there any relationship between the carbon footprint or the presence of meat and the publish date?

5. Can we find similar recipes that have lower carbon footprints?

6. What general statements can we conclude from our findings?


# Dataset

We plan to primarily use the "Cooking Recipes" dataset which is 2.5GB and in the form of HTML files. As described in the associated paper's [source](http://infolab.stanford.edu/~west1/from-cookies-to-cooks/), the dataset contains data from 14 distinct high-traffic recipe sites. Each site typically has a different format which we will do our best to document in order to extract the necessary information. Some html files lead to recipes that are grouped together strangely and which we ignored.

To enrich our study, we will have to include a dataset from https://www.greeneatz.com/foods-carbon-footprint.html which estimates the greenhouse gas emissions that result from the growth, processing and transportation of food. The dataframe we used is a selection from the top 16 worst foods to consume. 

# A list of internal milestones up until project milestone 2
Steps accomplished:

1. **Data exploration:**

    a.) Loaded recipe data
    
    b.) Extracted and cleaned data about ingredients and quantities.
   
    c.) Categorised meat ingredients in relevant sub-categories. 

2. **Environmental impact:**

    a.) Defined a formula to rate the environmental impact of the meat ingredients in a recipe
  
    b.) Rated and analyze ratings of recipes with meat ingredients.

3. **Nov. 25th - Milestone 2:**

    a.) Redefined which research questions we want to study in depth for the final project submission.
    
    b.) Documented our findings for final MS2 submission 
    
    c.) Planned next steps for Milestone 3 and final presentation


# Milestone 2 Update: 

After thoroughly exploring our data we discovered that we do not have the access logs referenced in the original paper so we had to redefine our project scope and goals to focus more fully on the recipe database. Instead of analyzing the consumer trends over time and geographic location, we will examine the meat prevalence in recipes as it relates to rating, publishing date and other recommended recipes. We limited our search to htmls of recipes, filtering out the web pages that have multiple recipes (i.e. "BBQ Recipes for 4th of July", "Salad ideas"). Our method for extracting the quantity of meat is not fool-proof: the numbers that appear in the ingredient list (i.e. '1 kg beef') are extracted along with the unit. Any fractions are converted to decimal and the total extracted numbers are summed. This may give us a few false values in cases where the quantities are represented strangely: '1 packet (15 ounce) of chicken broth' will extract a total quantity of 16 ounces (converted to kg) of chicken, which is not accurate. While, we're hoping that these instances are relatively few, we will need to verify that our data is not being corrupted by our extraction method.


# Next Steps: Analysis
Using the cleaned dataframe we created for milestone 2, we will begin analysis of the research questions above.
1.) Explore basic relationships between ratings, ingredients and carbon footprint
2.) Examine the ratio of recipes with meat to those without. Does this depend on the tags?
3.) Attempt clustering by tags and examine trends
4.) Formalize "story" based on observations
5.) Prepare presentation and final story
# Questions for the TAs
1) Is there a better way to extract quantities from datasets?
2) Is there a better way to generalize the format of websites or is it necessary to determine the schema for every website?
