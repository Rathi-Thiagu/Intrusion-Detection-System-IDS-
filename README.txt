UAV_DD-DV_Pickle.ipynb
	This file will load the dataset , visualize it and carry out preprocessing. Running this will file produce the pickle files needed for running the other files. 
	"f = h5py.File('pub_dataset1.mat')" Kindly mention the dataset paths in this line corresponding to all datasets.
	
UAV_Main_Baseline_ALL.ipynb
	Kindly run the "UAV_DD-DV_Pickle.ipynb" to create the pickle files.
	Running this file will develop models using Logistic Regression , KNN, LDA, Decision Tree , Bagging , Random Forest , Boosting and SVM. The raw dataset with complete feature set is used for training and testing.
	
UAV_Main_App1_v_1.ipynb
	Approach 1: This file combines the unidirectional and bidirectional dataset and then performs the binary classification for features 4, 5, 9, 10, 11, 12, 13, 14, 15, 16, 17 using Logistic Regression , KNN, LDA, Decision Tree , Bagging , Random Forest , Boosting and SVM.
	Kindly run this file after running the "UAV_DD-DV_Pickle.ipynb" as it uses the pickle file to import the dataset.
	
UAV_Main_App2_v_1.ipynb
	Approach 2: This file imports the dataset from the pickle file created after running "UAV_DD-DV_Pickle.ipynb". Lasso regression is used do the feature extraction and then the following models were developed. Logistic Regression , KNN, LDA, Decision Tree , Bagging , Random Forest , Boosting and SVM

UAV_Main_App3_PCA_ALL.ipynb
	Approach 3: This file uses PCA for dimensionality reduction from 54 to  5 in bidirectional dataset and 18 to 3 for unidirectional dataset. As a pre-requistie run the "UAV_DD-DV_Pickle.ipynb" to create the pickle files to be used here.
	

References :
https://www.analyticsvidhya.com/blog/2017/09/understaing-support-vector-machine-example-code/ - Code reference for Support vector Machines(SVM)
https://harvard-iacs.github.io/2018-CS109A/sections/section-5/solutions/ - Principal Component Analysis code reference