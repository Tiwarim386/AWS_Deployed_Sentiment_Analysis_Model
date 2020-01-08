# Deployed_Sentiment_Analysis_Model
Used BeautifulSoup to remove any HTML formatting that may have appeared.
Used NLTK to stem the words.



What this means is that when someone uses our web app, the following will occur.

To begin with, a user will type out a review and enter it into our web app.

Then, our web app will send that review to an endpoint that we created using API Gateway. This endpoint will be constructed so that anyone (including our web app) can use it.

API Gateway will forward the data on to the Lambda function

Once the Lambda function receives the user's review, it will process that review by tokenizing it and then creating a bag of words encoding of the result. After that, it will send the processed review off to our deployed model.

Once the deployed model performs inference on the processed review, the resulting sentiment will be returned back to the Lambda function.

Our Lambda function will then return the sentiment result back to our web app using the endpoint that was constructed using API Gateway.



## Future Tasks to make the project Stand Out

### 1 MAKE A BETTER WEB APP
   The web app in this project simply reports to the user whether the predicted sentiment was positive or negative. thinking of a better web app that uses the same model?

### 2 IMPROVE THE WEB APP APPEARANCE
   The provided web app is very simple and there is plenty of room for improvement h to stretch my web developer skills. Making a better front end and overall a better web-app.

### 3 IMPROVE THE MODEL
   The model chosen here is a straightforward RNN with a single hidden layer. There are many different model architectures that you could try to see if they improve the results. Will read research papers for better architectures and hyperparameters and then implementing them to improve the model.
