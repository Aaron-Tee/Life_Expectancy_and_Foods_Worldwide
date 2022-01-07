# Life_Expectancy_and_Foods_Worldwide
This is a data analysis of how eating habits relate to life expectancy.

We are going to look at the life expectancies of particular countries. I specifically want to focus on the dietary impacts on how long a person will live. We already know that humans that eat healthier diets live longer.
(two articles citing evidence of such)
https://time.com/4855506/healthy-diet-live-longer/
https://www.nejm.org/doi/full/10.1056/NEJMoa1613502
I would assume that there would then be a correlation between those countries that eat healthier diets and longevity. I would assume that there will be other factors that correlate to life expectancies, but I hope to show that there are high correlations to healthy diets and how long people live.

We will be using 3 datasets
This dataset is from https://www.kaggle.com/kumarajarshi/life-expectancy-who and lists countries of the world and their life expectancy among other considerations.
This dataset is was found from https://www.globaldietarydatabase.org/complete-survey-metadataand lists countries of the world and their dietary consumptions.
Each of the prior datasets lists countries of the world but one labels them as with their 'ISO3' which is an abbreviation, and the other lists the countries by name. This third dataset is one where we will use to match the name of the country with its 'ISO3' abbreviation.


Looking at life expectancy, we see that the mean value is 71 years old, with 51 and 88 years old at the extremes.
I have noticed that there are many negative and positive correlations. The closer we are to 1.00 or -1.00, the more closely the relationship is between the variables. 

There are correlations that relate to life expectancy. The schooling level that a person will reach is the factor that correlates closest (77%) to how long a person will live. BMI only has a 45% correlation. Coffee intake has one of the lowest correlations of 6.8%. The second strongest correlation to life expectancy is if a person lives in Sub-Saharan Africa which is 72%. This is a negative correlation as people tend to live longer if they do not live in the Sub-Saharan Africa region. These are not the factors that I thought would correlate closest to life expectancy.
While these are interesting data relationships. We still want to see if there is a correlation between foods and life expectancy.

We will look at two diets, one who would eat meat and all other foods, and the other that eats no animal products. The reason for this analysis is that we know that many scientists have spoken out in the 21st century regarding the negative health impact of eating animal products.
(articles citing evidence for above statement)
https://pubmed.ncbi.nlm.nih.gov/26780279/
https://www.science.org/doi/10.1126/science.aam5324
https://www.healthline.com/nutrition/plant-based-diet-vs-vegan


There is a very low relationship between foods and life expectancy. We can see that the correlation between life expectancy and those that eat meat is only 5%, while if a person does not eat meat their correlation is a bit higher at 10%. This means that overall a person that does not eat meat should live slightly longer than one who does eat meat.

The overall correlation negating the negative and the positive effects of different foods is only 22% for meat-eaters and 20% for those that do not eat meat. This shows that there is a relationship between what you eat and how long you live. While 22% (for animal product eaters) looks higher than the 20% (for the non-animal eaters) this does not show an increase in longevity, only a higher correlation.

There must be a larger underlining effect that causes life expectancy to raise and lower. While food does come into play looking at how long a person will live, it is not as significate of a correlation compared to where you live, your BMI, and your education.

Linear regression is commonly used for predictive analysis and modeling. For example, it can be used to
quantify the relative impacts of age, gender, and diet (the predictor variables) on height (the outcome variable).
​
https://www.displayr.com/what-is-linear-regression/

We will be using R scores to determine how close our computer model is to the actual data.
The coefficient of determination or R squared is a statistical measure of how close the data pairs in a set are to their fitted regression line. This measure ranges from 0 to 1, indicating the extent to which the dependent variable in a data set is predictable. - https://www.kite.com/python/answers/how-to-calculate-r-squared-with-numpy-in-python#:~:text=The%20coefficient%20of%20determination%20or,to%20their%20fitted%20regression%20line.&text=An%20R%20squared%20of%200,can%20be%20predicted%20without%20error.
 
After training models we have two best fits.

Ridge Regression gives us an 80.9% chance of correctly predicting our Life Expectancy Score.

Random Forest Regressor gives us a 98% chance of correctly predicting our Life Expectancy Score. 

As we can see there are relationships between foods that people eat, their education, where they live, their BMI, and their life expectancy.
While this is the case, my hypothesis that food greatly influences a person's life expectancy worldwide is a bit off. We can see from the above data that food does affect a person's longevity, but other factors give much more influence.
We were able to determine that those who eat a diet of no animal products do have a greater lifespan, but this is not as large of a relationship as was initially thought our data would show.
We can take the data and find enough correlations to reach a close accuracy of predicting a person's lifespan. It is interesting that how educated a person is and where they live in the world still affects a person's lifespan greater than what they eat.
The next steps to take would be looking at newer data of this variety to see if the correlations I found would be true while using another dataset.
We could use this data to try and equalize the life expectancy gap in places where people simply live shorter lifespans due to global location or education.
Is it feasible or possible to level the playing field of people around the globe based on location or education, when it comes to life expectancy?
