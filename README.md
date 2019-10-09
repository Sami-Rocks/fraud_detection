# fraud_detection


## Introduction
This is fraud detection system built with the Decision tree and Random Forest Algorithms. The Idea was to build a system that detects anomalous behaviour(s) in a list of transactions.

In this project, i used the features below to train the algorithm.
```
type: [ 0,1,2,3 ]
category: [ 0, 1, 2, 3 ]
business_id: <string> 
expired: [ 0, 1 ]
status: [ 0, 1, 2 ]
amount: <number>
time_difference: [0-180]
```
The ```label``` is either ```FRAUD``` or ```NOT_FRAUD```

The ```decision_tree.ipynb``` file contains the modeling building stages and the ```data.csv``` files is the data the model was trained on.

## The API
The ```main.py``` file is the API. It takes a POST request of a raw data, example 
```
[[2,0,339,0,6677,2230.09,38547]]
```
It response with a prediction ```"['FRAUD']"``` or ```"['NOT_FRAUD']"``` base on the input data.

### Setting up localy
#### Step 1
Clone of download files into the same folder.
#### Step 2
(Assuming you have python installed on your computer)
Pip install the following if you don't have the already
```
Flask, request, jsonify
numpy
pickle
json

```
### Step 3
Open your terminal or command prompt; redirect to the location of the files and run ```python main.py```.

Now you can send a POST request to the url, ```http://127.0.0.1:5000/```.

### NOTE
> Make sure the server is ruuning before sending the request. 
> Sample POST data to send is ```[[2,0,339,0,6677,2230.09,38547]]```
