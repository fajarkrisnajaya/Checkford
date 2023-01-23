## About
Fordpredictor is a web application that uses linear regression to predict the prices of used Ford cars. It is developed as a final project for a college course that aims to demonstrate the capability of machine learning in solving real-world problems. The app allows users to input various parameters such as the model, year, mileage, and additional features of the car, and returns an estimated price for the vehicle. The dashboard for the application is sourced from Kaggle and provides a user-friendly interface for viewing the predictions and inputting data. The app is built using Flask, a Python web framework, and utilizes pre-trained linear regression models. It is a useful tool for people who are planning to buy or sell a used Ford car as it provides an estimated value of the car based on the input parameters.

This project is intended for educational and demonstration purposes only. It is available on Github for anyone who is interested in learning about machine learning and web development using Flask and Python

### Prerequisites
You must have Scikit Learn, Pandas (for Machine Leraning Model) and Flask (for API) installed.

Flask version: 0.12.2
conda install flask=0.12.2  (or) pip install Flask==0.12.2

### Project Structure
This project has four major parts :
1. model.py - This contains code fot our Machine Learning model to predict employee salaries absed on trainign data in 'hiring.csv' file.
2. app.py - This contains Flask APIs that receives employee details through GUI or API calls, computes the precited value based on our model and returns it.
3. template - This folder contains the HTML template (index.html) to allow user to enter employee detail and displays the predicted employee salary.
4. static - This folder contains the css folder with style.css file which has the styling required for out index.html file.

### Running the project
1. Ensure that you are in the project home directory. Create the machine learning model by running below command from command prompt -
```
python model.py
```
This would create a serialized version of our model into a file model.pkl

2. Run app.py using below command to start Flask API
```
python app.py
```
By default, flask will run on port 5000.

3. Navigate to URL http://127.0.0.1:5000/ (or) http://localhost:5000

You should be able to view the homepage.

Enter valid numerical values in all 3 input boxes and hit Predict.

If everything goes well, you should  be able to see the predcited salary vaule on the HTML page!
check the output here: http://127.0.0.1:5000/predict

