# SignificanceTestingT-TestExample
T-tests: Comparing the means of two groups


Paired Sample T-Test.

This test is used when you have two measurements on the same subject or item, typically in a "before-and-after" scenario. It's powerful because it controls for individual-level variations.

Scenario: Testing the Effectiveness of a Sales Training Program
You are a data scientist at a company that has just put its 10-person sales team through an expensive new training program. The management wants to know if the program was effective at increasing sales.

To measure this, you have the monthly sales figures for each salesperson for the month before the training and the month after the training.

Some salespeople improved, but a couple did not. A paired t-test will tell you if the average improvement is statistically significant.

Step 1: Formulate the Hypotheses
For a paired t-test, your hypotheses are about the mean of the differences. Let μ 
d be the mean difference in sales for the entire population of salespeople.

Null Hypothesis (H 0): The training program has no effect. The mean difference in sales is zero.

H0

Alternative Hypothesis (Ha): The training program is effective. The mean difference in sales is greater than zero.

H(a):μd >0


Step 2: Choose a Significance Level (Alpha)
We'll use the standard alpha level.

Alpha (α): 0.05
Step 3: Calculate the Key Statistics of the Differences
First, we calculate the mean and standard deviation of our "Difference" column.

Step 4: Calculate the Paired T-Statistic
The formula for the paired t-statistic is simpler than the independent test's formula:
​
The standard deviation of the differences (3.27)


So, your calculated t-statistic is approximately 4.25.

Step 5: Determine the P-value
You compare your t-statistic to a t-distribution with n-1 degrees of freedom. In this case, 10 - 1 = 9 degrees of freedom.

For a t-statistic of 4.25 with 9 degrees of freedom, the p-value is very small.

P-value ≈ 0.001


Step 6: Make a Conclusion
Compare the p-value to your alpha level.

Is p-value (≈ 0.001) < alpha (0.05)? Yes.
Because the p-value is much smaller than the significance level, you reject the null hypothesis.

Conclusion: The results are statistically significant. There is strong evidence that the sales training program leads to a meaningful increase in sales. The improvement is not just due to random chance. You can report to management that the investment in the training program appears to be effective.


