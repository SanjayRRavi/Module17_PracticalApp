Location of Jupyter Notebook within GitHub: https://github.com/SanjayRRavi/Module17_PracticalApp/blob/main/prompt_III.ipynb (Detailed work and plots are shown here)

Business Problem Statement: 

Many times, businesses face the issue of having to target multiple potential customers thru phone calls to each individual (potential client), and unsure whether or not that individual will buy the product being advertised. Banks are no exception. This data here is from a Portuguese banking institution. The goal here is to investigate which features (characteristics of an individual) would be the most relevant for the purchasing decision, which is if a customer says "yes" or "no" to subscribing to a term deposit plan, and also creating a model that predicts what types of customers are most likely to say "yes".  This will help the banks redirect their limited resources towards contacting only the customers who are more likely to subscribe.

Findings (Summary & Conclusions):
* Logistic regression has higher precision score compared to the other 3 models, which are decision tree, SVC (support vector classifier), and KNN (k-nearest neighbors). Recommendation is to use logistic regression to create the predictive model.
* Precision for logistic regression has been calculated to be 0.83.
* In logistic regression, probability threshold can be adjusted to optimize for precision.
* Precision is the necesary metric to use, since we want to minimize the false predictions of customer saying "yes" (false hopes that customer will purchase term deposit plan from the bank) but the actual action is "no" (deciding not to purchase the term depost plan from the bank).
* The most important features or characteristics for the bank to investigate in order to maximize likelihood of customers deciding to subscribe to the term deposit plan are:
  * contact: Focus on the clients where contact type is cellular instead of telephone.
  * emp.var.rate: Focus on the clients with lower employment variation rate.
  * poutcome: Outcome of the previous marketing campaign needs to be "success". One of the plots in this Jupyter Notebook shows that for the previous marketing campaign of "success", majority of clients decided to subscribe to this plan.
  * cons.price.idx: Focus on the clients with higher consumer price index.
