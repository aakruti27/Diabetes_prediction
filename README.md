# Diabetes prediction with Streamlit app 

- The dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset. :blue_book:
  - The dataset can be found in diabetes.csv file 
  - We included age, number of pregnancies, glucose level, BMI, skin thickness, Insulin level and Diabetes pedigree function 

- The model that we used was SVM classifier with C=10, kernel='linear' because that was giving us the best performance with GridSearch :mag:
  - We exported this trained model as a pickle file, named "model_diabetes.pickle" :floppy_disk:
  - model_diabetes.pickle was used at the time of creating dashboard. 
  - With exported ML pickle model, we do not have to re train the model, and it makes the later process quick and easy. Pickle file is also sharable without having to share the whole ipynb file with preprocessing and training steps 

- We used streamlit to create a dashboard for this :desktop_computer:
  - Streamlit is a free and open-source framework to rapidly build and share beautiful machine learning and data science web apps. It is a Python-based library specifically designed for machine learning engineers.
  - The dashboard has easy to use interfact with sliders and text fields with a button in the end, which when clicked, outputs the prediction. 
  
 - This image shows prediction for person **not having diabetes**
  ![image_1](https://user-images.githubusercontent.com/52568409/221404424-2a50e182-530c-4b1f-927e-04776e5c3c44.jpg)

  
- This was run using Anaconda, with python version 3.9.13 :white_check_mark:. Note that "streamlit run" does not work with version 3.9.7 :negative_squared_cross_mark: 

- Click [here] (https://aakruti27-diabetes-predictionapp-st-trialapp-cxov5e.streamlit.app/) to check out the dibetes prediction web app
