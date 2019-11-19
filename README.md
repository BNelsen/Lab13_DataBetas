Lab13_DataBetas

Lab 13: World Indicators
Energy and Environment
11/11/2019
Overall Description of Lab 13

Due: 5:00PM Sunday, November 24, 2019 on OSF

The team will come up with one overall question and an answer to that overall question based on findings from subquestions. Each teammate will generate findings based on posing and answering (at least) one subquestion.

In this lab you will practice:

    finding and importing data
    joining datasets
    tidying data
    making plots that tell the narrative of the data
    generating hypotheses you can test based on data
    using the map functions
    plotting histograms and determining what constitutes an “extreme” value in the distribution
    answering questions based on statistical tests of data
    combining findings together to make statistically sound conclusions about important/interesting questions.

Overall question

Your data science team has been hired by the EPA to investigate several world environmental and energy data sets.

Each individual will do the following:

    Take one or two environmental and energy data sets, and come up with an interesting question
    Use a map function to calculate a summary statistic (e.g. mean, median, etc.)
    Use a permutation test to show asses whether there is a difference in some variable for two different countries in a single data set, or use a permutation test to analyze a correlation between a variable in an environmental data set and a variable in an energy data set.

These tasks should briefly be summarized in the individual sections. Then, decide which individual question is most interesting based on the relevance of the questions and the statistical tests, and explain the results and why this question is interesting in the team section. Create a plot that shows (visually) the answer to your overall question. Make a data-based conclusion.
Dataset

You will be using data from http:www.gapminder.org/data. First look through the “Lab Tasks” and “Submission Instructions” sections below and then find a Gapminder dataset or several datasets under “Environment” and “Energy” that you think will be interesting to analyze and can help you address an interesting question.
Lab Tasks

Each lab member should come up with and address a subquestion, and then each team should consolidate the findings and choose a single overall question that is most interesting.

Each team member will be required to perform a permutation test so each team member should choose a subquestion that lends itself to being analyzed via a permutation test.

Each team member will also be required to use at least one map function in their analysis from section 21.5 in R for Data Science. This does not have to be the main finding, but can be part of the exploratory analysis.

Note that you may investigate other data sets if you feel that they pose more interesting questions. As long as you perform the above tasks in your analysis, any data sets from gapminder are okay to explore.
Permutation Test Review

To perform a permutation test, you do the following

    Write down the null and alternative hypotheses, e.g., if you want to know if two groups A and B have the same mean then null hypothesis is H0:μA−μB=0

and the alternative is H1:μA−μB≠0

.

Determine your test statistic. The test statistic is often suggested by the null hypothesis. So, in the example above, the null hypothesis is that the population means (μA
and μB) are the same (i.e., the difference is zero) so the test statistic we will use to test this hypothesis is the difference in sample means x¯A−x¯B

    Mix up the group labels, calculate the test statistic for the mixed-up labels, and store this value of the test statistic.

    Repeat step three 999 more times

    Plot a histogram of the distribution of the 1,000 values of the test statistic from steps 3 and 4

    Where does the real data summary statistic fall in the distribution generated from step 5? Answer this with a percentile.

    Make a conclusion about whether or not to reject the null hypothesis based on the percentile from step 6.

Submisison Instructions

Your lab report should have a team section at the top followed by individual team member sections.

The team section should EXPLICITLY AND DIRECTLY address and contain the following points:

    What is the overall research question and why is it interesting/important?
    Briefly describe the dataset(s) that you are using and any preprocessing of the data your team did
    A summary answer to the overall research question. Include a brief description of the reasons for your answer.

Each team member’s individual section should EXPLICILTY AND DIRECTLY address and contain the following points (not necessarily in the order below):

    What is the subquestion you are addressing?
    The code for the map function you used and a brief description of what the code is doing
    A description of the permutation you performed and its results. Your description should contain the following:
        state explicitly the null and alternative hypotheses (i.e., step 1 in “Permutation Test Review”),
        what test statistic you are using (i.e., step 2 in “Permutation Test Review”),
        a histogram of the distribution of the test statistic (i.e., step 5 in “Permutation Test Review”),
        the percentile where the real data summary falls in the distribution (i.e., step 6 in “Permutation Test Review”),
        what conclusion you are drawing from the permutation test (i.e., step 7 in “Permutation Test Review”)
    A data-based conclusion/answer to your subquestion

