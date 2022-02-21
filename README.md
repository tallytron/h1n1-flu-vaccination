# h1n1-flu-vaccination

## Problem statement

With infection diseases spreading, the strain on the health care system can be excessive if the population does not accept the available vaccines to protect themselves and others.

## Objective

The government is looking to build a model that will predict how likely the population is to take the H1N1 and Seasonal flu vaccine

## Data set

To build this model, the data from National 2009 H1N1 Flu Survey was used where there were 35 available features for each respondent of the survey. The features ranged from opinions on the diseases to socioeconomic characteristics such as Income, Race and Sex.

## EDA

Does age play a role in vaccine acceptance?

![image](https://user-images.githubusercontent.com/80222038/154826836-73543501-c896-4e0b-8b83-4a0d41d52546.png)
 
 Based on the graph above indicates that as age increases people are more likely to get vaccinated. It's interesting to note that there is relatively a higher rate of vaccination for seasonal flu compared to the H1N1 vaccine.
 
 How effective is the vaccine according to respondents?
 
 ![image](https://user-images.githubusercontent.com/80222038/154826878-b1f3b1e6-742b-4e8a-af37-62351d7f5c14.png)

It's interesting to see that people in the higher age bracket are saying its effective to get vaccinated for the seasonal flu, however, there is a low percentage of people advocating for the H1N1 vaccine.

What role do doctor's recommendations play in promotiong vaccines?

![image](https://user-images.githubusercontent.com/80222038/154826983-a87a0015-d0ab-4dff-9ced-9516b6f3b68f.png)

In the graph above, it indicates that people are more likely to get vaccinated for the seasonal flu compared to the H1N1 flu.

An overview of the data processing

![image](https://user-images.githubusercontent.com/80222038/154827058-e433e6de-d948-432e-ad19-06b8f07fa09d.png)

![image](https://user-images.githubusercontent.com/80222038/154827081-6730e430-da1f-4bcd-8a7a-f6662effa3b6.png)
For the pre-processing, columns with having more than 45% nan values were dropped.

![image](https://user-images.githubusercontent.com/80222038/154827112-d834fc44-b19d-490d-b750-ac8f7a8f8063.png)
I did one-hot encoding, label encoding and ordinal encoding. A pipeline was built to fit it easily into the training and testing set. A series of models were built and ran eventually which led to LGBM and XGBoost having the best AUC and accuracy. 

## Model prediction

![image](https://user-images.githubusercontent.com/80222038/154827207-d890a504-d5f5-43f6-860e-53a55fad02d1.png)

![image](https://user-images.githubusercontent.com/80222038/154827220-af979c2b-c09d-447b-a339-22874c17a9fb.png)

To study feature importance, I used SHAP value which showed the top 4 features that were having an impact on the model.

![image](https://user-images.githubusercontent.com/80222038/154827242-fdb4af8a-d770-4d87-bf8f-8cc36dcfd622.png)

## Cost Summary

Please note that this cost is just an estimate and based off from research from different medical sites. This cost does not represent the actual market value nor the full cost, this is just to provide an idea to the audience on how much the cost will be if the US government decides to invest in the model. This is purely just for personal learning purposes.

![image](https://user-images.githubusercontent.com/80222038/155000051-2917cfc6-12e0-4217-ae88-2562f707a57a.png)


## Recommendations

![image](https://user-images.githubusercontent.com/80222038/154827287-2d51f20a-78d1-42a4-89b8-414678c03189.png)

![image](https://user-images.githubusercontent.com/80222038/154827293-86e952e4-0060-4470-a9d8-a8ecee9327ef.png)

