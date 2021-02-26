# Welcome!


## Introduction

This exercise will mimic a routine day in the life of a data scientist. It will cover the tasks such as data extraction, dataset creation, cleaning, processing followed by exploratory data analysis which will lead to building of some statistical models which are specific to the problem solving in the domain of a data driven venture capital.


## Loading the dataset

The dataset is available for the purpose of this exercise is in the format of a JSON file. Most of the data which is stored in the backend is in the format of JSON. The objective for a data scientist to accomplish the business purposes through analytics is to obtain the data in the tabular format. Now, the first steps towards making sense of the data is to start reading it. In the directory that you've cloned, read the file `founders.json` into a variable called `founders`.


Now, your objective is to inspect the structure of the JSON file. Once you've made some observations about the JSON file, you may write your observations about the JSON file in not more than 200-300 words. Feel free to go as indepth as you like. Remember, that it is a learning exercise and you're free to express the best out of your observation skills.

`File your replies here`

Now, once you've read and understood the structure of the JSON file, now we will attempt to convert the file that we have read into a tabular strcutured dataframe for the purposes of anlytics. In order to do that, load the relevant libraries and convert the JSON file that you've read as the `founders`variable into a pandas dataframe with the same name `founders` in such a way that each row corresponds to one organisation. Now, examine the dataframe and clean it for any missing values and write you actions in about 50-100 words. Print the result.

`File your replies here`

Once the dataframe is read into the correct format, let us start extracting information out of this tabular structured dataframe. The first task is to create an attribute called `co_founder_names` which essentially refers to the creation of all the co-founders corresponding to an organsation. Remember, that since you've read the file and processed the dataframe in such a way that each row corresponds to one organisation uniquely, this attribute `co_founder_names` should be a list of all the co-founders of that particular organisation.

for e.g. 

----------------------
|index| co_founder_name|

|1.   | [rodolphe-ardant, jordane-giuly]|




## Statistical Modelling

Once we have the dataset prepared about the entrepreneurs, the final task is about the creation of a statistical model that has the capability of exploiting the dataset. Now, in order to create a statistical model we need the label for training the model. Further, before we create the label, we first have to understand the classes of the label. In this case, the two classes for the labels are successful and struggling which is strictly as per the investment thesis of the organisation. Now, in order to assign the two classes to our data points, the criterion is-

* Any entrepreneur having raised Series A or more is deemed to be successful otherwise he is considered struggling
* This cretierion is strictly based on the investment thesis of the organization and in no way it is a broad judgement of one's capability


