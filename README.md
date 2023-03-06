# Amazon_Vine_Analysis
Big Data and AWS

## Overview
The purpose of this analysis was to determine whether or not there is bias in Amazon reviews based on whether the account is enrolled into the Vine program or not.

Extracting over 1,500+ reviews from Amazon concerning video games, it was handily determined that there is zero bias in the rankings towards Vine reviews versus non-Vine reviews. Namely, there was not a single review that came from a Vine enabled account - they were all non-Vine results.

## Results
### "Is there any positivity bias towards reviews in the Vine program?"
There is not. Based on our determination, there are no reviews present that were generated in an account that was paid by Vine.

IMAGE HERE

### "How many reviews total were there?"
All told, there are 1,685 records that were retreived from the video game review dataset. All of these fall under non-Vine accounts, none are Vine enabled.

IMAGE HERE

IMAGE HERE

### "How many reviews were 5 stars, and how many per account type? What is the percentage?"
There are a total of 631 5-Star ratings present, all of which came from the non-Vine accounts. Of the total review count, they make up 37.45% of the reviews. Perhaps unsurprising, as gamers tend to review bomb depending on the game's reception and the developer's week one response. See the lifecycle of No Man's Sky for a better look at review fluidity based on developer repsponse. Overall, the theme is that there will be a lower proportion of 5-star reviews on games as a whole, unless it is a niche category being considered.

IMAGES HERE

## Summary
Overall, it can be safely said there is no positivity bias towards Vine accounts, at least in this dataset. That isn't to say it isn't present anywhere, but it is easily determined there is no bias in the video game set as Vine account reviews don't exist in the first place. Above images and files contained within will further highlight this. Additional analysis that could be conducted to further reinforce the findings would be simple: run the data through Python as a loaded CSV instead of directly into PySpark, using different queries and syntax to verify that nothing slipped through. Luckily, with a data set this cut and dry, there is not much more to do in the way of confirming every response in the "Vine" column is "N", which in turn confirms positivity bias cannot exist.