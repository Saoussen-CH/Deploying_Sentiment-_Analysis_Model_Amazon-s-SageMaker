# Deploying_Sentiment_Analysis_Model_Amazon_SageMaker
Deploying of a Sentiment  Analysis Model of movies reviews using the IMDB dataset on Amazon's SageMaker platform.

## Project Overview
This project is part of the requirements for the completion of the Udacity Deep Learning Nanodegree. It consists of constructing a recurrent neural network using LSTMs for the purpose of determining the sentiment of a movie review using the IMDB data set. This model is created using Amazon's SageMaker service. The model will be deployed using an API endpoint and Amazon Lambda and a simple web app which will interact with the deployed model.

## Setup Instructions

The notebook provided in this repository is intended to be executed using Amazon's SageMaker platform. The following is a brief set of instructions on setting up a managed notebook instance using SageMaker, from which the notebooks can be completed and run.

### Log in to the AWS console and create a notebook instance

Log in to the AWS console and go to the SageMaker dashboard. Click on 'Create notebook instance'. The notebook name can be anything and using ml.t2.medium is a good idea as it is covered under the free tier. For the role, creating a new role works fine. Using the default options is also okay. Important to note that you need the notebook instance to have access to S3 resources, which it does by default. In particular, any S3 bucket or objectt with sagemaker in the name is available to the notebook.

### Use git to clone the repository into the notebook instance

Once the instance has been started and is accessible, click on 'open' to get the Jupyter notebook main page. We will begin by cloning the SageMaker Deployment github repository into the notebook instance. Note that we want to make sure to clone this into the appropriate directory so that the data will be preserved between sessions.

Click on the 'new' dropdown menu and select 'terminal'. By default, the working directory of the terminal instance is the home directory, however, the Jupyter notebook hub's root directory is under 'SageMaker'. Enter the appropriate directory and clone the repository as follows.

```bash
cd SageMaker
git clone https://github.com/Saoussen-CH/Deploying_Sentiment_Analysis_Model_Amazon_SageMaker.git
exit
```

After you have finished, close the terminal window.

### Open and run the notebook

Now that the repository has been cloned into the notebook instance you may navigate to the SageMaker_Project.ipynb notebook.
