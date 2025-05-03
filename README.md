# Logistic_Regression

We know that Linear Regression Model is used to make continuos numerical prediction whereas a Logistic Regression is used to predict the probability of a given outcome.

https://developers.google.com/machine-learning/crash-course/logistic-regression/sigmoid-function

Logistic Regression: Calculating a probability with the Sigmoid Function:
--------------------------------------------------------------------------
a. Many problems require a probability estimate as an output. 
b. Logistic Regression is extremely efficient mechanism for calculating probabilities.
c. you can use the returned probability in either of the following two ways:
      1. Applied "as is.
      2. Converted to a binary category such as True or False, Spam or Not Spam, '0' OR '1'

Sigmoid Function (means 'S' shaped):
-------------------------------------
a. Sigmoid function ensures its output repesnts a probability. i.e. It always ensures that the output is always between 0 and 1.
b. The logistic function has the same characteristics as mentioned above
c. The standard logistics is also known as Sigmoid function 
d. As the input to the sigmoid function increases, the output of the sigmoid function approaches but never reaches 1. 
e. As the output to the sigmoid function decreases, the output of the sigmoid function approaches but never reaches 0

Logistic Regression models are trained using the same process as the Linear Regression models, but with two distinctions:

  a. Logistic Regression models use Log Loss  as the loss function instead of Squared loss.
  b. Applying Regularization is critcal to avoid overfitting.

Log loss:
---------
a. In the Linear regression module, you used squared loss (also called L2 loss) as the loss function. Squared loss works well for a linear model where the rate of change of the 
   output values is constant. 
b. However, the rate of change of a logistic regression model is not constant. The sigmoid curve is s-shaped and is not linear. When the log-odds (z) value is closer to 0, small 
  increases in result in much larger changes to y than when z is a large positive or negative number. If you used squared loss to calculate errors for the sigmoid function, as 
  the output got closer and closer   to 0 and 1, you would need more memory to preserve the precision needed to track these values.
  So the loss function for the logistic regression is Log loss. The Log Loss equation returns the logarithm of the magnitude of the change, rather than just the distance from 
  data to prediction.
  For formula see the link:   https://developers.google.com/machine-learning/crash-course/logistic-regression/loss-regularization

Regularization in logistic regression:
--------------------------------------
  a. Regularization, a mechanism for penalizing model complexity during training
  b. Regularization is extremely important in logistic regression modeling.
  c. Without regularization, the asymptotic nature of logistic regression would keep driving loss towards 0 in cases where the model has a large number of features. Consequently, 
     most logistic regression models use one of the following two strategies to decrease model complexity:
          1. L2 regularization
          2. Early stopping: Limiting the number of training steps to halt training while loss is still decreasing.



