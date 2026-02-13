# Federal-Min-Wage-and-Inflation-Rate-Regression
A regression that shows how strong of a correlation the Federal minimum wage has on inflation 

Using Inflation rate as the depoendent variable, I tried determining if the federal minimum wage had any correlation with inflation, to then preform a causal analysis.
  * Inflation Rate is the dependent variable
  * Federal minimum wage is the treatment variable
  * Earnings, Housing Price, Interest Rates, Labor Force, Personal consumption, Production and Money Supply were all independet variables to build the model
  * Data was collected from the FRED, BLS and Social Security

After Combining and Cleaning the data, this is the correlation matrix that was constructed:

<img width="940" height="788" alt="CH" src="https://github.com/user-attachments/assets/05977114-b2e8-4019-982e-f428ba984d63" />

After building the correlation matrix, we ran an Initial Regression

<img width="532" height="738" alt="REG_1" src="https://github.com/user-attachments/assets/be650bf6-2fc3-4b38-810a-5817ceb50697" />

The model had a good R^2 value, showing that our variables are good at predicting inflation, however not every variable was statistically significant, with quiete a few having a P-Value abouve 0.05.
This first model also didn't lag inflation rate, which is necessary as these data sets are annual averages, rather than quarterly or monthly points.

After removing the unimportant variables, and lagging the inflation rate, this is the new regression model:

<img width="507" height="652" alt="REG_2" src="https://github.com/user-attachments/assets/e11075ab-6b1b-4e19-8a8c-297dc99306d1" />

Still has a high R^2 value, which shows the independent variables are still important for determing the dependent variable.
However, the P-Value for the Minimum Wage is 0.184, far above the 0.05, showing that this value is NOT statistically significant when predicting the Inflation rate.

We can interpret that, due to the low correlation Minimum wage has on Inflation, that a causal analysis is unnecessary, and that a change in the Minimum wage doesn't much impact the inflation rate.
But how much can we increase the Min Wage to, before it does? Conventional Economic Theory proves that increasing wages does impact inflation, so the new question here is how much can we increase the min wage before we sstart seeing statistical significance?

That is another question for another day, but right now, the general agreement is that it should be increased to around $15.00, however after the Covid Pandemic and the economic challenges that followed, there is increasing arguments for it to be pushed even higher.
