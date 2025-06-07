# deep-learning-challenge
Used: Student collaberation, ChatGPT, Xpert Learning for resources
Report:
Introduction and Methodology
For this project, I created a neural network model to predict whether charity applications would be successful or not. The goal was to train the model on past charity application data, which includes information such as application type, classification, and income amount, and then use it to predict the outcome of future applications.

The first step was cleaning the data. I removed irrelevant columns like EIN and NAME because they didn’t help with the prediction. I also handled categories that were rare by grouping them under "Other" so they wouldn’t confuse the model. After cleaning, I used a technique called one-hot encoding to turn non-numeric data into numbers that the model could use.

I then built a simple neural network using TensorFlow. The network has three layers: one for input, two hidden layers that learn from the data, and an output layer that makes the final prediction. I trained the model for 100 steps (called epochs) and used an optimizer called Adam to improve the model over time.

Results and Evaluation
After training the model, I tested it using new data that it hadn’t seen before. The model’s results were as follows:

Accuracy: 53%

Loss: 1.18

The accuracy means the model got the prediction right 53% of the time, which is a bit better than random guessing. However, it’s clear the model could be better. The loss of 1.18 shows that the model made some errors, but it’s not terrible. The loss value needs to go lower for better predictions.

I could improve the model by trying different settings, like adjusting the number of layers or tweaking the learning process. A model like Random Forest could also work well for this problem, as it uses multiple decision trees and is easier to tune and interpret compared to neural networks.

Conclusion
In conclusion, the neural network worked but didn’t perform as well as I hoped. Its accuracy of 53% is a good start, but with more adjustments or by using a different model like Random Forest, it could do much better. More tuning and testing are needed to improve predictions for charity applications.
