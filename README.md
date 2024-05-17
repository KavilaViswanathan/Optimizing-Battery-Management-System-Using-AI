# Battery Management System Optimization

This repository contains code for optimizing battery management systems using various machine learning algorithms. The focus is on predicting the Remaining Useful Life (RUL) of batteries and implementing optimization strategies based on the predictions.

## Table of Contents
- [Introduction](#introduction)
- [Data](#data)
- [Feature Engineering](#feature-engineering)
- [Models](#models)
- [Results](#results)
- [License](#license)

## Introduction

Battery management systems (BMS) play a crucial role in ensuring the efficient and safe operation of batteries, particularly in electric vehicles and renewable energy storage systems. This project aims to predict the Remaining Useful Life (RUL) of batteries using machine learning models and optimize battery management strategies accordingly.

## Data

The dataset used in this project is the NASA Battery Dataset, which contains data on the charging and discharging cycles of batteries. The dataset includes various parameters such as voltage, current, and temperature. You can download the dataset from [this link](https://www.kaggle.com/datasets/patrickfleith/nasa-battery-dataset/data).


## Feature Engineering

The feature engineering process involves selecting specific rows of data, aggregating statistical features, and calculating the RUL based on the selected rows. Key steps include:
- Selecting a random row from the latter half of each data file.
- Aggregating statistical features (mean and standard deviation) before the selected row.
- Calculating the RUL as the difference between the final time and the time of the selected row.

## Models

Three different machine learning models are trained and evaluated to predict the RUL of batteries:
- RandomForestRegressor
- GradientBoostingRegressor
- XGBRegressor

Each model's performance is evaluated using Mean Absolute Error (MAE) and R-squared (R2) scores.

## Results

The performance of each model is compared using bar charts for MAE and R2 scores. Feature importance is also analyzed for the best-performing model (XGBoost).
![Model Comparison](https://github.com/KavilaViswanathan/Optimizing-Battery-Management-System-Using-AI/assets/140960627/3de97250-1e58-4f5e-8e97-a0bd7ecf9dbe)

## license
MIT License

Copyright (c) 2024 KavilaViswanathan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

