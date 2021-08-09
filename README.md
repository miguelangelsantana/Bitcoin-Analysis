
# Predicting Cross Selling Opportunities
#### Health Insurance Cross Selling

Author: Miguel Santana

#### Project Methodology
An insurance company provides health insurance to its customers. The client would like to build a model that predicts whether current customers would be interested in vehicle insurance provided by the company. The dataset includes customer demographic and vehicle information including gender, age, region, vehicle age, damage, policy premium and sourcing channel. 

This project will follow the OSEMN process: Obtain, Scrub, Explore, Model, Interpret. The Kaggle data set can be located [here.](https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction)

### Project Variables

![!](/images/data.jpg)

#### Customer Interest / Data Imbalance

![!](/images/customerinterest.png)

### Dimensionality Reduction | PCA and K-Means Clustering

![!](/images/elbow.png)

![!](/images/cluster.png)

## Statistical Modeling

#### Imbalanced Model Comparison

![!](/images/imbalancedmodel.png)

**While the results may look attractive, a useful model will be able to accurately classify customers in a balanced data set.**

### Balanced Model

![!](/images/balanced.png)

Light Gradient Boosting Machine offers a higher F1 score with similar accuracy and precision. LGBM will be our selected model. 

### Model Analysis

![!](/images/ROC.png)

![!](/images/featimp.png)

![!](/images/shap.png)

## Interpret Variables, Customers that ARE interested

![!](/images/agestat.jpg)

![!](/images/genderstat.jpg)

![!](/images/prev_ins.jpg)

![!](/images/veh_dam.jpg)

## Conclusion
When considering cross selling opportunities, the client should focus on marketing to customers between the ages of 35 and 50 that have not been previously insured and currently have a damaged vehicle with an emphasis on male customers.

## Future Work
This analysis does not interpret whether this specific demographic is a good insurable risk. Future work should include underwriting and rating guidelines to appropriately measure risk and price premiums for a full product analysis in these specific markets.  

For any additional questions, please reach out via email at santana2.miguel@gmail.com or on [LinkedIn.](https://www.linkedin.com/in/miguel-angel-santana-ii-mba-51467276/)

##### Repository Structure:

```

├── README.md               <- The top-level README for reviewers of this project.
├── cross_sell.ipynb     <- narrative documentation of analysis in jupyter notebook

```