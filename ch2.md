# Chapter 2
### What is ML?
Machines observe a pattern and attempt to imitate it in some way that can be either directly (supervised) or indirectly (unsupervised)

#### Supervised Learning:
 - Useful for taking what you know as input and transforming it into what you want to know <br>
 - Monday Stock Price -> Supervised Learning -> Tuesday Stock Price<br>
 - Trains a supervised classifier<br>
 - Train the model on existing data so that it could predict future values of that dataset<br>   
 - Deals with labeled data<br>

#### Unsupervised Learning
 - Transforms one dataset into another; the dataset that it transforms into is not previously known or understood
 - "find patterns in this data and tell me about them"
 - Clustering dataset into groups; if it learns 10 clusters its common for these labels to be the numbers 1-10 (each datapoint assigned to a cluster)
 - Dataset turns from a bunch of datapoints to a bunch of labels.
 - List of datapoints -> Unsupervised Learning -> List of cluster labels
 - All forms of unsupervised learning can be viewed as a form of clustering

	** The algorithm doesn’t tell you what the clusters are, it just tells you, "hey, I found some structure. It looks like there are groups in your data" **
	


## example: of trying to fit a square peg into the correct hole
### Parametric learning
 - Tends to use trial and error and try everything until it works

### Nonparametric learning
 - Tends to count the sides of the peg

### Supervised parametric learning:
 -  Fixed number or knobs
 - The model would take in data and transform it into a prediction factor. It would then use this factor to try and predict future outcomes. If it succeeds then it will adjust the knob for that predictor depending on whether or not the factor helped in making the right prediction.
 - This can be thought of as a search algorithm - youre searching for the right knob configuration by trying configurations then adjusting them and retrying (parametric part - brute force)
 #### 3 steps to SPL in the analogy of sports: 
#### 1. Predict 
 - Gather sports stats, send them through machine, and make a predicton about the probability that the team will win.
#### 2. Compare to the truth pattern
 - Compare the prediction (say 98%) with the pattern we want. If they lose then the truth is 0%.
 - This steps says if the model predicted this upcoming loss.
#### 3. Learn the pattern
 - Adjust the knobs by studying how much it was off by (98%) and what the data was at the time of prediction.
 - Turns the knobs to make a more accurate reading the next time
 - The next time this step saw the same sports stats the prediction would be lower than 98%. Each knob represents the prediction's sensitivity to different types of input data. That change is the learning process.

#### Unsupervised parametric learning:
 - ** unsupervised is all about grouping data **
 - Uses knobs to group data - but has several knobs for each group
 - At a very high level, they adjust parameters to transform the input data into its subscribing groups
	
#### Nonparametric learning:
 - Number of parameters is based on data, not predefined.

#### Summary:
> In summary, there are 4 different algorithms to choose from. All models are either supervised or unsupervised and parametric or non parametric. Parametrises is about the way the learning is stored and often the method for learning.	
A parametric model is characterized by having a fixed number of parameters, whereas a non parametric model's number of params is infinite or otherwise, determined by data