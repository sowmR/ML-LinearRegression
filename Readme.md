# Linear Regression

**Formula:**

When there is only one feature (x) and one target(y)

y = mx+c

The above is the formula for line. m = slope/weight, c = intercept/bias.


There are multiple features:  x = [x1,x2,x3....xn]

y = b0+b1*x1+b2*x2....+bn*xn


**Pros:**

Very Simple to implement

Performs well on data with linear relationship

**Cons:**

Not suitable for data having non-linear relationship

Underfitting issue is possible

Sensitive to Outliers.


# Evaluation

The Following evaluation matrices are used to evaluate the efficiency of Linear model

#### Loss function: 

Loss function measures how far as predicted value is from the actual value. 

This will help in finding which parameter (weight, bias in this case) performs betters. 

Lower the loss function value, better the model will be. 


MSE = (∑(y−y ̂ )^2 )/n    
where,
 n=number of samples.
 y = actual value
y ̂=perdicted value.
![image](https://user-images.githubusercontent.com/26898960/145043935-533b9252-6d67-45f9-bbfb-ecb4cafd1479.png)


# optimization

determining best parameter for the model. 

In case of linear regression, optimization process should reduce the loss function so that the predicted value is more accurate. 


Gradient descent is the method used to optimize the linear regression model.


First, randomly initialize the parameters for the model (weight and bias in this case).

Then, change the parameter values through multiple iterations until a global minimum value is achieved. 

Formula for gradient descent:

weight = weight - L* Dw

bias = bias - L * Db

where,

L = Learning Rate,

Dw = Parital derivative of Loss function with respect to w

Db = Partial derivative of Loss function with respect to b



D_w  =  (−2)/n ∑129_(i=0)^n▒(x_i (y_i−y ̅_j )) ![image](https://user-images.githubusercontent.com/26898960/145042434-ddcb772c-7689-4c1f-852d-775dd2eaeb17.png)


D_b= (−2)/n ∑129_(i=0)^n▒(y_j−y ̅_i ) ![image](https://user-images.githubusercontent.com/26898960/145042387-4fa4ed4f-cb67-4192-8aee-11bc05428afa.png)




for a multivariant input, the formula is changed to 

w[i] = w[i] - L*Dw[i]

where , w[i] = i th weight.



