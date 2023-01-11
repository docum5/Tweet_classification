# Tweet_classification

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


## Overview
I deploy the model to the API using Fast API.

Link: [https://flight-price-prediction-api.herokuapp.com/](https://flight-price-predict-api.herokuapp.com/predict)

[![](https://github.com/docum5/Flight-Price-Prediction/blob/main/DEMOO.PNG?raw=true)](https://flight-price-predict-api.herokuapp.com/predict)

[![](https://github.com/docum5/Flight-Price-Prediction/blob/main/demo22.PNG?raw=true)](https://flight-price-predict-api.herokuapp.com/predict)

## Workflow


## Model_and_architecture
 

## Evaluation_metrics


## Conclusions

The analysis results show that using the Indobert Pre-Trained Model in this Twitter analysis case can produce an accuracy of 95% with a True Positive Rate of 88% and a True Negative Rate of 97%.

## Obstacle

* The data used is still classified as imbalance, so it is necessary to add data to the minority class data.

* There is a need for further understanding of what kind of education is meant so that the output produced will be in accordance with the desired needs.

## Technologies_Used


![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://d3.harvard.edu/platform-digit/wp-content/uploads/sites/2/2022/04/demo-huggingface_optimized-370x200.png" width=170>](https://huggingface.co/) [<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c6/PyTorch_logo_black.svg/2560px-PyTorch_logo_black.svg.png" width=280>](https://pytorch.org/) [<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f4/Elasticsearch_logo.svg/1280px-Elasticsearch_logo.svg.png" width=200>](https://www.elastic.co/) [<img target="_blank" src="https://i.imgur.com/p0Nufjn.jpg" width=100>](https://fastapi.tiangolo.com/)

