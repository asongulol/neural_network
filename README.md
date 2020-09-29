# Neural Network

We attempted to  our knowledge of machine learning and neural network model to create a classifier that is capable of predicting whether or not charity will be successful if funded by Alphabet Soup. The model used the charity dataset. The software language used were Python 3.7, Scikit-Learn, and the Tensorflow platform. Please refer to the notebook 
__Neural_Networks_Alphabet_Soup_Challenge.ipynb__.

Here are the major findings and activities:

__✓ How many neurons and layers did you select for your neural network model?__

Based on trial and error I chose to have 20 neurons in the first level, and 8 neurons in the second level. This appeared to provide the best accuracy results at 75.55%

__✓ Were you able to achieve target model performance?__

Using the LeakyRELU activation model, 50 epochs and 20:8 neuron ratio provided the highest accuracy level in the optimizations that I tried.

__✓ What steps did you take to try and increase model performance?__

I attempted the following optimizations to increase level performance:

1. I bucketed values less than 25,000 for the ASK_AMT variable to remove noise and help increase the accuracy of the model.I also bucketted the NAMES variable grouping all values less than 100.
2. I tried doubling the number of neurons in the first layer from 10 to 20.
3. I tried adding more neurons to the second layer from 8-12.
4. I tried a different activation method (RELU to LeakyRELU).
5. I tried decreasing the alpha level to 0.1

__With all the optimizations I was able to get to a best accuracy value of 75.55%  and a loss of 49.64%. __

✓ If you were to implement a different model to solve this classification problem, which would you choose and why?

I also tried the Random Forest Model and got a pretty good predictive accuracy of 75.4%

I also tried Logistic Regression and the accuracy was 73.9%.

Therefore, I would probably choose the Random Forest Model because it gave an accuracy level only 0.15% less than the neural network model without sacrificing speed.
