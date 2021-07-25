<h1 align ="center">Hyperparameter-Tuning</h1> 
<h3>This is a repository for the medium article published under ADG VIT on Hyper parameters tuning.</h3>

<h4>Hyperparameters are configuration variables that govern the training process itself.
For example, part of setting up a deep neural network is deciding how many hidden layers of nodes to use between the input layer and the output layer, 
and how many nodes each layer should use. These variables are not directly related to the training data.</h4> 

<br>
<hr> </hr>

<h3>This repo consists of</h3>

- The .ipynb (Jupyter Notebook/Google collab) file of the FULL CODE. 
- The code snippets (.ipynb) which are attached in the article. 
- The Breast cancer dataset used.

<br>
<hr> </hr>

<h2 align ="center">Dataset</h2>
<h3>The dataset used is Breast Cancer Wisconsin (Diagnostic) Data Set.</h3>
<h4>The full dataset can be accessed from<a href="https://www.kaggle.com/uciml/breast-cancer-wisconsin-data"> HERE.</a></h4>
<br>

| Variable |Definition | Key |
| --- | --- | --- |
| id | ID number |
| diagnosis | The diagnosis of breast tissues | M = malignant, B = benign |

<br>
<h4>Ten real-valued features are computed for each cell nucleus: </h4>

| Feature | Defintion |
| --- | --- |
| Radius | Mean of distances from center to points on the perimeter |
| Texture | Standard deviation of gray-scale values |
| Perimeter |
| Area |
| Smoothness | Local variation in radius lengths |
| Compactness | Perimeter^2 / area - 1.0 |
| Concavity | Severity of concave portions of the contour |
| Concave points | Number of concave portions of the contour |
| Symmetry | 
| Fractal dimension | "coastline approximation" - 1 |
<h4>Class distribution:</h4>

| Total True values | Diagnosed Type |
| --- | --- |
| 357 | (B) benign |  
| 212 | (M) malignant |

<br>
<hr> </hr>

<h2 align = "Center">More Information</h2>

<h4>Where the model parameters specify how to transform the input data into the desired output, the hyperparameters define how our model is actually structured.</h4>
<h4>But unfortunately, there’s no one universal way to calculate “which way should one update the hyperparameters to reduce the loss and increase the efficiency?” 
(For e.g. The learning rate(α) of gradient descent, a method typically used in linear regression algorithm) in order to find the optimal model architecture. 
Thus, we generally resort to experimentation to figure out what works the best.</h4>

<h3>The tuning methods used here are:</h3>

<ol>
  <li><h4><h3>Grid Search </h3> Define a search space as a grid of hyperparameter values and evaluate every position in the grid. </h4></li>
  <li><h4><h3>Random Search </h3> Define a search space as a bounded domain of hyperparameter values and randomly sample points in that domain. </h4></li>
  <li><h4><h3>TPOT</h3> TPOT is a Python Automated Machine Learning tool that optimizes machine learning pipelines using genetic programming. </h4></li>
  <li><h4><h3>Bayesian Optimization</h3> Bayesian optimization is an approach to optimizing objective functions that take a long time (minutes or hours) to evaluate. </h4></li>
</ol>

<br>
<h2 align = "center"> END </h2>
