# News Headline Generator
We have built a web application using flask framework in python that generates headline for the given news body. This application can be used by bloggers, journalists etc. where they can easily come up with the summarized headline for the article/blog they are working upon. We attempt to reproduce the results in the paper:  [Generating News Headlines with Recurrent Neural Networks](https://arxiv.org/pdf/1512.01712.pdf)

## How to run the application
### Software:
* Install [Python](https://www.python.org/downloads/)
* Install [Anaconda](https://www.anaconda.com/download/)
* Install [Keras](https://keras.io/) 
* Install [Tensorflow](https://www.tensorflow.org/install/)
* Neural networks are computations heavy, GPU configuration is recommended.

### Data
We have used [All the news dataset from kaggle](https://www.kaggle.com/snapcrack/all-the-news/data)
Extract only title and content from the dataset. Later, we tokenized the title,content and saved it as a pickle file. We divided our data set into train, validation and test sets respectively.

## Train / test
Train() method inside “model_preparation.ipynb” notebook to train the model (run dependant functions first) <br>
Test() method inside “odel_preparation.ipynb” to test model (run dependant functions first)

## Running the web app
Run the app.ipynb notebook to start flask server and open web app


 






