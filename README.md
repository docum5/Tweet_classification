# Tweet_classification

<p align="center">
  <img src="https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/workflowtweet.png?raw=true" />
</p>

## Table of Content
  * [The Problem](#the-problem)
  * [Goal](#goal)
  * [Assumption](#assumption)
  * [Dataset](#dataset)
  * [Overview](#overview)
  * [Workflow](#workflow)
  * [Model_and_architecture](#model_and_architecture)
  * [Evaluation_metrics](#evaluation_metrics)
  * [Conclusions](#conclusions)
  * [Obstacle](#obstacle)
  * [Technologies_Used](#technologies_used)


## The Problem
Since I joined Legal Analytics-Telkom Indonesia as a project-based talent, I got several projects to do, one of that is to do a Twitter analysis. I asked to identify whether tweets would become a topic in the news. 

Based on BBC Journalistic Guideline, there are six parameters that cause an issue to develop into news based on how to get it, including inspire, divert, educate, give, perspective, update, and keep me on trend. In this case, I asked to develop the educated point.

## Goal

**Goal: Predict/detect whether issues/information on Twitter is an educational, persuasive, or educational explanation.** 

**Model: Receive input in the form of Twitter text, and classify whether the tweet is educational or not
Input: Data twitter, etc.**

**Output: {“educate”: Binary, [“True”, “False”]}**
  
## Assumption

Educate: maintain and provide training (teaching, guidance, leadership) regarding morals and intelligence.

In the context of news, education is an activity that encourages the addition of knowledge and changes in attitudes, behaviour and skills of a person/group in a reasonable manner.

## Dataset
<p align="center">
  <img src="https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/Screenshot%202023-01-11%20at%2012.21.03.png?raw=true" />
</p>

Real Data          |  Input 
:-------------------------:|:-------------------------:
![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/datatweet1.png?raw=true)   | ![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/datatweet2.png?raw=true) 



## Overview
I deploy the model to the API using Fast API.


Homepage          | Get the data by id| Predict  | Search by Content/Category
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/Screenshot%202023-01-11%20at%2017.19.07.png?raw=true)   | ![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/Screenshot%202023-01-11%20at%2017.19.33.png?raw=true) | ![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/Screenshot%202023-01-11%20at%2017.20.16.png?raw=true)| ![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/Screenshot%202023-01-11%20at%2017.19.53.png?raw=true) 

**Demo Model**         
:-------------------------:
![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/Screenshot%202023-01-13%20at%2010.53.44.png?raw=true) 



## Workflow
Make a Custom function to modify the slang words          | Normalize the slang words| Cleaning the data 
:-------------------------:|:-------------------------:|:-------------------------:
![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/workflow1.png?raw=true)   | ![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/workflow2.png?raw=true) | ![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/workflow3.png?raw=true)

Apply Language Detector           | Filter just the Indonesian tweets  
:-------------------------:|:-------------------------:
![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/workflow4.png?raw=true)   | ![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/workflow5.png?raw=true) 



## Model_and_architecture
**IndoBERT Large Model (phase1 - uncased)-indobenchmark/indobert-large-p1**

<p align="center">
  <img src="https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/model.png?raw=true" />
</p>



## Evaluation_metrics

Evaluation Model on Data Testing         | Evaluation Model on Data Eval | Evaluation Matrics
:-------------------------:|:-------------------------:|:-------------------------:
![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/eval1tweet.png?raw=true)   | ![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/eval2twitter.png?raw=true) | ![](https://github.com/docum5/Tweet_classification/blob/main/portfojan2023/eval3tweet.png?raw=true) 

## Conclusions

The analysis results show that using the Indobert Pre-Trained Model in this Twitter analysis case can produce an accuracy of 95% with a True Positive Rate of 88% and a True Negative Rate of 97%.

## Obstacle

* The data used is still classified as imbalance, so it is necessary to add data to the minority class data.

* There is a need for further understanding of what kind of education is meant so that the output produced will be in accordance with the desired needs.

## Technologies_Used


![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://d3.harvard.edu/platform-digit/wp-content/uploads/sites/2/2022/04/demo-huggingface_optimized-370x200.png" width=170>](https://huggingface.co/) [<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c6/PyTorch_logo_black.svg/2560px-PyTorch_logo_black.svg.png" width=280>](https://pytorch.org/) [<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f4/Elasticsearch_logo.svg/1280px-Elasticsearch_logo.svg.png" width=200>](https://www.elastic.co/) [<img target="_blank" src="https://i.imgur.com/p0Nufjn.jpg" width=100>](https://fastapi.tiangolo.com/)

