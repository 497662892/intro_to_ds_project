# Dynamic-Programming-Project
The final project for Introduction to Data Science

Student Name: Jiajian Ma

Student ID: jm10850

## Introduction

This project is the implementation of my final project "Distribution-Aware Synthetic Sample Selection for Enhanced Model Generalization in Polyp Segmentation"

The high level idea of this work is to propose a synthetic data sample strategy that can **aware both of the distribution of original data and the already selected data when sampling**. To overcome the limitation of "random selection" and "prediction base selection".

![image](https://github.com/497662892/intro_to_ds_project/blob/main/imgs/visualization.png)

Intuitively, we can observe that, compared to the random selection strategy, our proposed strategy can collect more samples in the OOD regions, thereby theoretically increasing the diversity of the feature space more effectively (a and b). Compared to the prediction-based selection method, our strategy effectively avoids clustering of selected sample points and maintains the integrity of feature space distribution (c and b).

## Code

In this repo, we provide the code for the implement of our proposed method and the visualization of the result in **"implementation.ipynb"**. Due to the size of the data (>10GB) we assuming that we have obtained the feature maps of each images. For detail of how we get them, can refer to the **"visualization_logging.ipynb"**, which is not runnable because of lack of data. 

If you are interested in the data augmentation and polyp segmentation part, you can refer to https://github.com/497662892/Ai-Security-Final-Project, it also provide the full code and data we used in this experiment.

## files and folders

logs: the folder to store the logs of the experiment (testing)

feature_maps: the folder to store the feature maps of the original and synthetic images

data: the folder to store the data of the experiment, which only include the csv file (no images)

final_report.pdf: the report of the project