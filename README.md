# fraud_detection


## Introduction
This is fraud detection system built with the Decision tree and Random Forest Algorithms. The Idea is was to build a system that detects anomalous behaviour(s) in a list of transactions.

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

The ```decision_tree.ipynb``` 
