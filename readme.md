# Austin Animal Center Exploration: Findings
## by Antonio Vargas


## Dataset

The intake and outcomes tables are public tables provided by the city of Austin. Both tables contained an animal ID, and thus was able to generate a “stay-ID” for each row, which is the concatenation of the animal-ID and the index-number of that particular animal’s visit. I could then join the tables by the stay-ID, and generate the length of stay by generating the timespan between the intake and outcome timestamps. The joined dataset is stored as the file "austin-animal-center_stays_in_the_center.csv".

## Summary of Findings

Across the entire population, the type of animal (dog, cat, wildlife, livestock, etc...) and the intake-type (adoption, euthanasia request, etc...) revealed major correlations with the stay-lengths. Thus, I also explored correlation amongst subpopulations dogs, dog-adoptions, cats, and cat-adoptions.

Across the subpopulations, the exploration didn’t yield a single strong correlation or inverse correlation, yet a number of significant correlations were found across the population and subpopulations, thus indicating that it would be possible a build a multivariate predictive model that could potentially predict the stay-length of a new dog or cat intake.

## Key Insights for Presentation

In the exploration, the covariance table for the covariance across the entire population was really useful in identifying that the wildlife intakes accounted for a great deal of interdependence amongst the variables. Finding that wildlife intakes accounted for a lot of the correlation in the stay-length also helped indicate that the subpopulations should be explored separately, as it does make sense the rabid-bat intake (bats are common in Austin) is a fundamentally different intake than a dog intake to be held for adoption. 
