# Analyze-A-B-Test-Results

Introduction:

For this project, we will be working to understand the results of an A/B test run by an e-commerce website.

The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. 

Our goal is to work through this notebook to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

Table of Contents:

* Introduction

* Part I - Probability

* Part II - A/B Test

* Part III - Regression



OBSERVATIONS:

From the above results,

* The probability of individual conversion is 0.11959708724499628

* The probability of conversion, when individual was in the treatment group is 0.11880806551510564

* The probability of conversion, when individual was in the control group is 0.1203863045004612

* The probability of individual, received new page is 0.5000619442226688

* The propability of new page is round 50% which does not prove that all new treatment page will be more converted.



A/B TEST:
hypothesis test:

š»0: Pššš¤ - Pššš <= 0

š»1: Pššš¤ - Pššš > 0

GRAPH:

p_diffs = np.array(p_diffs)
plt.hist(p_diffs)
plt.xlabel('p_diff values')
plt.ylabel('Frequency')
plt.title('p_diff simulation plot')

![image](https://user-images.githubusercontent.com/81925727/117196494-6589d500-ad9b-11eb-8609-947ac5d2d476.png)


CONCLUSION:

These results are based on the given dataset. There may be limitaions due to incorrect data or missing values.

From this analysis, after regression, it is observed that p_value between US and CA is varied. So there is no evidence to reject the null hypothesis. We can accept the null hypothesis and can reject the alternate hypothesis.
