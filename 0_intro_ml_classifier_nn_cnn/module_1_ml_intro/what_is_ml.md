# What is machine learning???
* Machine learning is a kind of scientific method of getting the expected result by learning the known data that is keep changing and 
adjusting the parameters consistantly until  the error approaches to __"ZERO"__. 
* The key to get it done are __"Math, Computer Science and Patience"__.

# Basic ideas
* Machine learning - It is very similar to human study, you need tons of input data set in order to train the model, in another words, the algorithm which will be used to predict the future result by reading the unseen input data.
* The more input data you have, the higher chance you could train your model successfully.
* The __essence__ of ML is to approach is the best result of "Goodness of fit", not deduction in mathematical way, in another words, there is no certain known model like in math operation for us, you need to optimize the parameters of the algorithm until you approach the best possible result.
* Featrues - Pick the appropriate features for training. 
    * Input data X and labeled target Y.
    * Binary classification and multiple classification.
    * For discrete data there is __classfication__ problem, for continuous data there is __regression__ problem.
* How it works
    * The essence of ml model is the __"Mapping"__ between feature X value and the labeled target Y - y=f(x, w) where w is the parameters, mainly __weights and bias__.
    * For binary classification, Y = {+1, -1}, for multi-classification, Y = {|y|>2}, for regression, y={R}.
    * How?? We let the very fist model predict the result by input data and get the result  Y_hat, Y_hat = f{xm w} and the result then compare with the labeled target Y and catch the error, we then optimize and change the parameters until the error approach its possible minima and the learned parameters is the best result we approach which can be used to predict the unseen data in the future task.
    * Things needs to notice
        * The testing data must be unseen data set for the sake of the performance of generalization.
        * Make sure the picked features are the __correlative__ properties instead of __irrelevant__ properties.
        * Optimization problem, how to optimize the parameters in order to get the best result of generalization of the model.
            * In mathemetical problem we often talk about the maximum and minimum, it is the similar concept to machine learning where we are actually finding the appropriate combination of parameters for __"ZERO" value of derivative__, i.e. the  minima of error data
            * It is not always the case, the __generalization__ performance is closely tied to the density of the training data, the different __training model(training function/algorithm)__ also does matter(which causes the cnn better optimized in image classification for example).
            * The big impact of overfitting and underfitting with training and testing data.
                * The example of overfitting.
                    * For example we have x input and y label with some __noisy__ data along side, when we training the input data we also __count the noisy data__, for making the error down to the minima, i.e. the fitting curve go through each of the individual data point specifically, therefor overfitting.
                    * We can use regularizatin method to reduce the chance of overfitting, i.e. put some limitations on the parameters, or we can add more training data which may help the algorithms detect neural signal better in order to avoid the overfitting problem.
                * On the other side we often encounter underfitting problem too, it is easy to overcome by adding more deeper layers of the neural networks, in machine learning we also call it __"learning capacity"__.
        * Machine learning process is consist of __3__ similar stages and data set, __training, developing and testing__, the result comes from developing stage may not the best since the data may be overfitting, so remember to test it, even couple more times.
        * Machine learning process contains __2__ types of parameter, super parameter and ordinary parameter.
            * For example, in __cnn__ we often see things like weight(parameter), layers(super parameter), for equation in mathematical notation, the __exponent__ is the super parameter(we can look it as __there are many different layers in neural networks__), and the coefficients a.k.a weight in nn, is called __parameter__.
            * __Super parameter__ is often man-made where __parameter__ is optimized through the __forward backward propagation__ which we will use in the later projects(weights or coefficients are coming from the optimization of the equation, i.e to get the best weight is to resolve the equation in math).
            * __Super parameter__ is influential for __model generalization__, for instance, the developing stage or the validation part is for figuring out the best value of super parameters.
        * How to enhance the performance of __model generalization__*
            * __First__  - create more layers, i.e more deeper learning network, therefore to make the cost function down to the minimum as well as to suppressing overfitting problem by regularization technic.
            * __Second__ - construct much better data set, including gain more data and make the extracted features more impressive, make sure the data set is in the proper data distribution, or the result will be mistakenly ouput.
        * The final output.
            * For __regression__, the output is a "real number".
            * For __classification__, the output is a "vector" or "0/1" in binary classification.

# Image classification

* It is rather trivial task for human to classify or detect the image object in this world.
* What computer sees from an image???
  * A large set of pixel data or __Matrix__ so to speak, for example, an image of pixel size 1280\*720 which means the image is stored as 1280\*720 matrix, each pixel is consist of __"R, G , B"__ channels value between 0 to 255 respectively.
  * Image is represented as __"H * W * C"__, height, width and color channel.
* Image classification challenge
  * There are many issues to cause the wrong prediction
    * Different angle of view
    * Size of the object
    * Morph of the object
    * Cover on the object
    * Brightness
    * Background 
    * Multiple Sub-Class differences

