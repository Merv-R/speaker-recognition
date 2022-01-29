Below is the execution order of the python files submitted.
------------------------------------------------------------------------

Note: 
	- All the folder structure in "./spectrogram_images" , "./training_data", "./testing_data" has been created and are empty. This folder structure has been used in program and data is dumped in corresposding folders like training_data, testing_data once we run below mentioned files.


1) 	Generate_Spectorgrams.py

			- All the audio files will be converted into spectrogram image files 

2)		CNN_train_main.py

			- Performs 90:10 train/test split and builds a 3 layer CNN model 
	
3)		Split_train_val.py

			- Split train data for training and validation

4)		Testing_CNN.py

			- Use the test sample from step 2 to see how model performed on test data
			- 'Speakerresult_1.csv' is created which contains the acutal and predicted Speaker information

5) 	Performance_Analysis.py

			- Using the 'Speakerresult_1.csv' we analyse the F1 , Accuracy, Precision and Confusion matrix of the model.


Additional note:
---------------------

- Since building a model takes a lot of time, we have also included the model file that we built during our testing saved as "speakermodel_1.h5'. The model file can be loaded directly and evaluate the results for cases where we want skip model building

- There is folder 'smallcorpus_custom_Dataset' which contains sample data with 5 speakers and this is the data set that was used for our model evaluate metric screenshots and reference images.

System Requirements:
------------------------------

• Python 3.6.x​
• Libraries: NumPy, LibROSA​
• Python Packages: TensorFlow, Keras​
• Virtualenv or Anaconda