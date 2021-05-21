[Everyday Things](https://github.com/vmsmith/EDT/blob/master/README.md)  

### Intuitive Statistics  

#### Introduction  

I have taken a lot of statistics courses in my day—at both undergraduate and graduate levels—and this document is written in the spirit of things I wish I had known when I was getting started. Too often statistics books begin with the math, and do not present an intuitive understanding of either what's going on, or where you're headed. Hopefully, if you don't know anything about statistics and are curious, this will provide you with a few points to help you understand what it's all about.

#### Accuracy vs Understandability  

Many beginning statistics books make a point that there is often a tradeoff between accuracy and understandability. One can develop very complex models, with many variables, that describe or predict something very accurately, but the models are so complex as to not be understandable at the common sense level. What does it mean to say that some outcome is a function of the square root of negative pi? 

A person who owns a chain of shoe stores, for example, and wants to know what he or she has to do to increase sales, probably won't want a very accurate model that has complex numbers and converging infinite series that correlate shoe sales with sidewalk conditions and tidal ranges. That person would probably be happier with a slightly less accurate model that contains linear relationships between, say, web site ads and Twitter activity. Or something like that. (And actually, the proper tools for the shoe store owner would probably be a data warehouse and pivot table, but this was just an example.)

With that in mind, what follows is geared towards understandability, at the expense of accuracy. People who really know and understand statistics may take issue with certain things, and from an accuracy point of view they would be correct. But what follows is accurate enough for developing an initial grasp of fundamental statistical concepts.

#### Probability vs Statistics  

The two are related, but they are not exactly the same. If I had to try to capture the difference in one or two lines, it would be something like this: 

* Statistics is, in a certain sense, backwards looking. Data has been collected, and from it things are said.  
* Probability is, in a certain sense, forward looking. You are trying to predict the likelihood of events.

That's a huge generalization, and some people will take issue with it, but I think it's good enough for this discussion.

#### Types of Statistics  

There are different types of statistics. Descriptive statistics, inferential statistics, and predictive statistics come immediately to mind. Some might add diagnostic statistics, prescriptive statistics, and one or two more. The three I mentioned are probably the most common, and it's good to know the differences among them. 

*Descriptive statistics* basically looks at an entire group (a "population") and describes it. That entire group might be all the students at a university, where a descriptive statistic might be, "54% of the student body is female, and 46% of the student body is male." Or, "The average age of the student body is 23 years and 4 months." Or, "The average family income of the student body is 

*Inferential statistics* basically takes samples of a population and tries to make inferences about the overall population from which the sample was drawn. This often happens when it's too difficult to get data from each and every element of the population. 

*Predictive statistics* takes samples, and tries to predict things that might be outside the sample range.

Again, these are big generalizations, but good enough for now.

#### Types of Probability  

I mention this because probability and statistics go hand in hand.

There are three generally accepted types of probability, and not distinguishing among them can cause a lot of grief.

*A priori* probabilities are associated with things like games of chance: dice, roulette, etc. The probabilities are baked in. For example, if a die is fair, you know that there is a 1 in 6 chance it will roll the number "1". Period. You don't have to roll the die 1,000 times and do the math; you know from the nature of the situation itself.

Empirical probabilities are essentially based on the frequencies of past events. When a meteorologist says there's a 70% chance of rain, it essentially means that 70% of the times there have been similar conditions in the past, it has rained. Or, if there’s a weather model, the model shows rain 70% of the time.

Subjective probabilities are just what they sound like. They're something like intuitions based on personal experiences. Imagine an experienced teacher on the first day of class. He or she looks around the room, and within some period of time might identify the kids he or she thinks will be troublemakers, and puts them in the front row. Something like that.

If you read Nassim Nicholas Taleb, he came up with something called the Ludic Fallacy. "Ludic" comes from the Latin word *ludus*, meaning "game." The fallacy is in mistaking situations characterized by empirical or subjective probabilities for *a priori* (game) situations. 

####  Measures of Central Tendency  

This is a core statistical concept. You want one number (or one expression) that can best be used to describe or infer or predict. In one-dimensional models, this is often called an *average*. And there are several types of average. The most common types are mean, median, and mode (but there are a few more).

#### Measures of Dispersion  

This goes hand in hand with measures of central tendency. Having come up with one number (or expression) that describes something, you want to know how all the data points relate to it.

The most widely known measure of dispersion is probably standard deviation. This is often used when the mean is used as a measure of central tendency. In a normal distribution ("bell curve"), the mean is in the middle, and about 68% of the data will fall within plus or minus one standard deviation of it. About 95% of the data will fall within plus or minus two standard deviations of it. And about 99.7% of the data will fall within plus or minus three standard deviations of it. Here's a visual:

[Standard deviations](https://en.wikipedia.org/wiki/Standard_deviation#/media/File:Standard_deviation_diagram.svg)

Another common measure of dispersion is quantiles. This is often used when the median is the measure of central tendency. With quantiles, you divide the distribution into equal parts. A really common visual for this is the box plot, which shows the median and four *quartiles*. Here is an example:

[Box plot with quartiles](https://en.wikipedia.org/wiki/Box_plot#/media/File:No_Outlier.png)

The red line is the median: half the data points are on one side, and half on the other. The blue box contains two quartiles (one on each side of the median), or 50% of the data. The two "whiskers" at the end signify the upper and lower bounds of the data.

#### Epsilon Theory

If I had to reduce the difference between math and statistics to one thing, it would be the Greek letter epsilon. And this is really the essence of much of statistics.

Suppose we have a group of 30 young men, and we are interested in heights. When the topic of heights comes up, we could rattle off all 30 heights. Or, we could say something like, “The average height is 5’9”, plus or minus.”  The “plus or minus” means that no one is really 5’9” (well, maybe someone is), but that everyone is that average height plus or minus something.

In statistical terms, we would say, “The average height is 5’9” + e,” where “e” is epsilon. And epsilon is a shorthand way of saying “plus or minus” something.

Epsilon is the error term. 

And here is the essence of statistics: We try to come up with some measure of central tendency—be it a number or an expression of some sort—such that 
