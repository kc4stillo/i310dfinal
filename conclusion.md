# Results

After defining and evaluating the performance of our chosen models (logistic regression and MLP), we found that our logistic regression model had an accuracy score of 
approximately 87% and our MLP model had an accuracy score of around 29%. One thing we wanted to mention is that our logistic regression model’s accuracy score was originally 
around 62% but when training our logistic regression model, we changed the initial solver (solver= “lbfgs”) to a solver called “newton-cg.” Newton-cg significantly improved 
the accuracy score of our logistic regression model.

Aside from that, by comparing the accuracy scores of both models, it can be seen that our logistic regression model is much higher in accuracy compared to our MLP model. 
This is significant because it suggests that the relationship between our input features and the target variable may not be as complex as we thought (more predominantly 
linear/simple). With this insight, the specific task of predicting marital status based on demographic characteristics can be sufficed with a linear model and one that 
may not require the complexities of MLP. Additionally, as mentioned in the section above, we used LIME to demonstrate the interpretability of our model. To do this, we explained 
the prediction using an example instance in our logistic regression model.

Shown in this image is what was generated using LIME. From this image, we reached the conclusion that ‘times_married’ is a big predictor of marital status. Additionally, we 
tested the fairness of our model using sci-kit-learn’s ‘classification_report’ to look at the f-scores.

From this report, we focused on the f-scores (circled in the image) to assess any biases in our model. The Logistic Regression model shows significant similarity across the 
f-scores, which indicates an ideal model. However, in an ideal scenario, the MLP model should have performed with similar accuracy and F-scores across different marital statuses 
but that is not the case. The MLP model shows significant disparities in precision, recall, and f1-score between marital status. This MLP model suggests a bias towards unmarried 
individuals, as the model is less accurate in predicting married individuals versus unmarried individuals, demonstrating unfairness towards married individuals.

## Conclusion

In conclusion, our analysis became evident that the logistic regression model stood out as the most precise classifier among the methodologies explored. Through Lime statistics, 
variables such as times-married, property value, and nativity surfaced as significant influencers, shedding light on key factors driving the predictive power of our model. 
Nevertheless, it's crucial to acknowledge the limitations encountered during our study, particularly in accessing users' personal information. This constraint poses a challenge, 
as it could potentially introduce biases, particularly when handling sensitive data.

As we look forward, there is a clear pathway for advancing our research. One avenue involves expanding our investigations to encompass diverse geographical regions. By conducting 
similar studies in different locales, we can not only validate the robustness of our findings but also foster a deeper understanding of how socioeconomic factors vary across populations. 
This comparative approach not only improves the range of our insights but also supports the transferability of our results, enabling policymakers and practitioners to make more informed 
decisions that resonate with the nuances of specific communities.

## Appendix

One of the main points made in the Q&A discussion was regarding how we would further the study. Although we were able to reach conclusions, we would obtain more well-rounded results 
by assessing other parts of the country. If we had more time and more resources, we would combine different datasets from around the country to reach a cohesive report. This could also 
be used as an element for another data scientist to be able to pick up from where we left off.
