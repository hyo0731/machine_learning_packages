# Machine learning packages

### Motivation
To learn various ways of machine learning, how to use 'python sklearn packages'    
and learning about polynomial regression using 'python numpy, matplotlib packages.'    

### Build Status
There are 2 projects (midterm project + finalterm project)  

I have finished midterm project and I compute the polynomial regression with many degrees.  
I have finished finalterm project and I got accuracy 0.975(97.5%).  

### Code Style 

Both project I use python language.  
In midterm project I mainly use numpy and matplotlib.  
In finalterm project I mainly use numpy, matplotlib and sklearn packages.  

### Screenshots

**Midterm Project** 

The part loading packages and datas points.  

![20211221_171211](https://user-images.githubusercontent.com/92132775/146901070-76a82a2f-cda1-4bad-9af1-c01df0ee03c0.png)

Computing Vandermonde matrix.  

![20211221_171236](https://user-images.githubusercontent.com/92132775/146901126-c2c1eaf7-5157-4302-a70f-b46e2a7d1578.png)

Compute the coefficient of Polynomial regression and print results.  

![20211221_171259](https://user-images.githubusercontent.com/92132775/146901167-24668eb6-1784-4425-8238-8256722fe30f.png)

**Finalterm Project**

The part loading packages and datas points.

![20211221_161158](https://user-images.githubusercontent.com/92132775/146900965-61f42620-ad9a-46f4-9f68-c6c3bcd7706c.png)

The part classification with logistic regression algorithm.

![20211221_161956](https://user-images.githubusercontent.com/92132775/146901025-216c32b3-5af2-4363-90d5-f2d08dc55c5c.png)

### Tech/Framework used

**Midterm Project**  

If data points are in square matrix, we can make a inverse matrix.
But if it is not a square matrix, we have to make a pseudo inverse matrix.
So I make a pseudo inverse matrix using np.linalg.pinv() function in numpy.

**Finalterm Project**  

I used logistic regression algorithm for face recognition.
I used these parameters.

1. random_state = 0 (to see the changes of accuracy)
2. C (inverse of regularization strength)
3. penalty (I choose 'l2')
4. solver (I choose penalty 'l2' so I can choose 'newton-cg', 'lbfgs', 'liblinear', 'sag', 'saga'.
5. And I finally choose 'newton-cg')
6. class_weight (If not given, default = None)
7. max_iter (Maximum number of iterations taken for the solvers to converge, default = 100)

### Features

**(Midterm Project)**  
I have computed with various degrees and found there is underfitting, overfitting phenomenon.

**(Finalterm Project)**  
Many people use Support Vector Machines algorithm for classification. But I used logistic regression algorithm for classification. I made algorithm and code simple and I got hight accuracy by finding optimize hyper-parameters.

### Code Examples

**Midterm Project**  
Compute matrix. Using codes with numpy packages.
np.zeros(), np.column_stack(), np.ones(), np.matrix(), np.concatenate()
np.dot(), np.linalg.pinv(), np.asarray()

**Finalterm Project**  
Creating classification and fit and predict. Using codes with logistic regression.
sklearn.linear_model.LogisticRegression(), fit(), predict()

### Installation
Of course you should install python. Here is a link to download python.  
https://www.python.org/downloads/windows/  

**intstalling sklearn**  
*pip install scikit-learn*  

### Tests
**(Midterm Project)**  
You can modify degrees of mine or change data points you want.
Also there is another way to compute vandermode matrix so try with another way.

**(Finalterm Project)**  
There are various hyper-parameters in logistic regression.
So if you want to test this algorithm using other parameters, you can modify hyper-parameters of logistic regression and also you can test it with your own data points.

### How to Use
**(Midterm Project)**  
You have to load numpy, matplotlib packages, data points you want.
Show data points using matplotlib packages.
Choose degree and make matrix and compute a Vandermonde matrix using numpy packages.
Compute coefficients of polynomial regression and show polynomial regression using matplotlib packages.

**(Finalterm Project)**  
I have made algorithms and codes simple, so it is easy to use.
You have to load packages, data points you want.
If packages and data points are ready, choose algorithm you want (In my case: logistic regression).

1. you should create classification object in sklearn packages.
2. fit the object to training data sets [using fit(,)].
3. predict the label of test data point [using predict()].


### License
MIT license
