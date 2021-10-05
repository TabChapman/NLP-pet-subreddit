## Readme for 'Is you pet a Jerk or a Bro?'

Cats and dogs are the two most common pets in the United States with 471 million dogs and 370 million cats. As an owner of a cat I’ve found that cats are unfairly labeled as jerks. At the same time dogs are considered man’s best friend when sometimes they can also misbehave. I wanted to see if dogs and cats really are their stereotype or does the data show otherwise. I used the subreddits r/AnimalsBeingBros and r/AnimalsBeingJerks because they were the two most common animal subreddits with positive and negative connotations. I used reddit API to transfer the data to a Dataframe. I then used Countvectorizer to transform the data for easier analysis.

1. I found that while the word dog is more likely to be used in r/AnimalsBeingBros, there wasn’t a huge difference with cat in a close second 
2. Cat was the number one word used in r/AnimalsBeingJerks but again, dog was number two at a close second 
3. Overall the top ten list were very similar with 6 words dog, cat, animal, cute, dogs, and funny found in both lists. 

For the model I used a random forest model with the TDIFvectorizer for a better result. Overall it was hard to get a good model from the data. I was forced to use the post titles because most of the posts were pictures or videos of which many had nothing to do with the content of the post. Additionally, many of the posts were just people posting pictures of their cute pets with no regard to how ‘jerky’ or ‘broey’ their pet is. Ultimately, my best result was with a 0.615 for the test data after optimizing hyperparameters with a grid search. 
