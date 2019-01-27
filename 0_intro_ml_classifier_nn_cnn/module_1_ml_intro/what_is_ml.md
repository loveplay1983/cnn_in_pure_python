# What is machine learning?? 
* Machine learning is a kind of scientific method of getting the expected result by learning the known data that is keep changing and 
adjusting the parameters consistantly until  the error approaches to __"ZERO"__. 
* The key to get it done are __"Math, Computer Science and Patience"__.

# Basic terms
* Machine learning - It is very similar to human study, you need tons of input data set in order to train the model, in another words, the algorithm which will be used to predict the future result by reading the unseen input data.
* The more input data you have, the higher chance you could train your model successfully.
* The __essence__ of ML is to approach is the best result of "Goodness of fit", not deduction in mathematical way, in another words, there is no certain known model like in math operation for us, you need to optimize the parameters of the algorithm until you approach the best possible result.
* Featrues - Pick the appropriate features for training. 
    * Input data X and labeled target Y
    * Binary classification and multiple classification
    * For discrete data there is __classfication__ problem, for continuous data there is __regression__ problem
* How it works
    * The essence of ml model is the __"Mapping"__ between feature X value and the labeled target Y - y=f(x, w) where w is the parameters, mainly weights and bias
    * For binary classification, Y = {+1, -1}, for multi-classification, Y = {|y|>2}, for regression, y={R}
    * How?? We let the very fist model predict the result by input data and get the result  Y_hat, Y_hat = f{xm w} and the result then compare with the labeled target Y and catch the error, we then optimize and change the parameters until the error approach its possible minima and the learned parameters is the best result we approach which can be used to predict the unseen data in the future task.
    * Things needs to notice - The testing data must be unseen data set for the sake of the performance of generalization.

