# Deep Learning
 
<h2> OVERVIEW </h2>
The purpose of this analysis is to create an algorithm that will predict whether applications for funding will be successful. We will process the data and then design a neural network that will predict if an organization will be funded based on the features in our dataset.  

<h2> RESULTS </h2>
Data Preprocessing: 
•	Variable used as the target (output): “IS_SUCCESSFUL”	
•	Variable(s) used as the features (inputs)
o	NAME
o	APPLICATION_TYPE
o	CLASSIFICATION
o	AFFILIATION
o	USE_CASE
o	ORGANIZATION
o	STATUS
o	INCOME_AMT
o	SPECIAL CONSIDERATIONS
o	ASK_AMT
•	Variables that were focused on when testing and training the model
o	APPLICATION_TYPE
o	CLASSIFICATION
•	Variables used were focused on during optimization of the model
o	NAME
o	APPLICATION_TYPE
o	CLASSIFICATION
•	Variables that were removed from the data
o	EIN
o	STATUS
o	SPECIAL_CONSIDERATIONS

Compiling, Training, and Evaluating the Model:
Initially, we focused on the Application type and classification columns as well as using 110 neurons over 2 layers. When we ran our model, and it was 73% accurate in predicting which organizations would be funded. Then we optimized our model by adding a 3rd layer, used 140 neurons across those 3 layers and Sigmoid activation for the 2nd and 3rd layer, and focused on the name of the organization in addition to the application type and classification. After this we ran our model again and it was now 79% accurate. 

<h2> SUMMARY </h2>
Based on this we found that if the name of the applicant appears more than 5 times, if your application type is a T3, T4, T5, T6, T7, T8, T10, or T19, and if your classification is > 1000 you will have more success in getting funding.  I used the random forest model and found that the accuracy of the model was 78%, which is also a good prediction; however, it did not perform as well as the optimized neural network. 
