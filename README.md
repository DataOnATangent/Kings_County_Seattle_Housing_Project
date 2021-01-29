# Kings County Housing Project
 

Overview:
======
This project seeks to model housing prices in King County, Washington to predict housing prices. 

## Premise: 

Housing prices can be unpredictable but by looking at historical pricing and properly assessing which factors are driving prices we can begin to get a sense of where things are going. Using this information to help sellers and buyers alike make informed decisions about their homes. 

## Analysis Focus
1. Use visuals and data frames to evaluate the data.
2. Using that data to direct the evaluation of available variables.  
3. Creating a model to predict a test data set.

## Procedure

### Initial Findings 

We began our analysis by exploring the data set in general for outliers to explore and/or correct. Followed by exploring the variables against price for general correlation. Expectedly, price demonstrated a high correlation with factors like the number of bedrooms, overall size, and zip code. 

<p align="center">
  <img width="460" height="300" src=images/Bathrooms.png>
</p>

<p align="center">
  <img width="460" height="300" src=images/Bedrooms.png>
</p>

<p align="center">
  <img width="460" height="300" src=images/Grade.png>
</p>

<p align="center">
  <img width="460" height="300" src=images/Corr.png>
</p>


### Data Clean Up

The data did not require much clean-up but notably did require accounting for some errors and outliers in the bedrooms and bathrooms.


### Feature Creation 

While some factors were predictably correlated it was nevertheless necessary to look at more variables and groups through the creating of features that categorize home by size, and general condition. Additionally, other variables were transformed through the use of interaction to make it possible to explore correlations that might not have been possible to see until looked at as standalones.  

### Testing and Evaluation

Despite testing many features very, very few made it into the final model. This is largely due to problems they caused when using them to predict against hold out data. In the end, it was the same expected factors that made it into the final model along with a distance to Gas Works variable which also proved to be highly correlated with price.  

Using the wrapper method I was able to confirm that my chosen columns were very effective for predicting the price to within 141k with most columns ranging from 8% price correlation to 67% price correlation and accounting for 82% of the variation. 

## Conclusion 

While housing markets fluctuate often, it seems many of the factors that affect pricing remain reasonably consistent with the location still being by far the biggest factor, followed by the size of the house itself, and condition in close succession. 

## Repository Structure  
All working notebooks can be found in /working notebooks, project materials can be in /Project files, the images used above can be found in the imgaes folder, and copies of the my final notebook and other files can be found in /Former files. 


