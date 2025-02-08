# COE379L_Prog1

<h3>What did you do to prepare the data?</h3>
I prepared the data by first checking the file type of the given data set. Then, I read the csv file using pandas. After reading the csv file, I check the the shape, size, and data types of the raw data. After that, I check if there are duplicate rows and remove them. Finally, I fill in the missing or invalid values by using the mode method. Finally, I perform one-hot encoding on categorical variables such as age group, breast_quad_..., etc. 

<h3>What insights did you get from your data preparation?</h3>
After preparing the data, I noticed that the target variable (class) is imbalanced with significantly more no-recurrence cases as compared to recurrence cases. This meant that splitting the data into training and testing data needs to be more carefully handled. I also noticed that tumor size and inv-nodes were strong predictors of recurrence, where larger tumors meant a higher risk. I also noticed the most missing values where in node-caps. 

<h3>What procedure did you use to train the model?</h3>
To train the model, I split the data using stratified split (80% train, 20% test). Then I perform classification using the K-Nearest Neighbor Classifier, K-Nearest Neighbor Classifier using Grid search CV, and Linear classification. 

<h3>How does the model perform to predict the class?</h3>
The model performs well in predicting the class. The high precision of the model correctly identifies true recurrence cases (false negatives), however, it has lower recall causing it to miss some recurrence cases (false negatives). 

<h3>How confident are you in the model?</h3>
I am moderately confident in my model because the model accuracy is greater than 50% and the f1 score is greater than 75%. However, a tabular dataset is very noisy and not very good for predictive modeling. 
