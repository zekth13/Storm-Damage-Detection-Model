# Tropical storm damage detection model

This is an EY Open Science Data Challenge Program 2024 - Storm Damage Assessment.

## Objectives

The goal of the challenge is to develop a machine learning model to identify and detect “damaged” and “un-damaged” coastal infrastructure (residential and commercial buildings), which have been impacted by natural calamities such as hurricanes, cyclones, etc.

## Methodologies
<ol>
    <li>Convert the Pre_Event_San_Juan.tif files to jpg files</li>
    <li>Annotate the jpg files using LabelMe</li>
    <li>Download the annotated images in YOLOv8 required format </li>
    <li>Split the images into train, test and Val dataset</li>        
    <li>Train the YOLOv8 model</li>
    <li>Test and validate the model</li>
</ol>

## Prerequisites
<ul>
    <li>os</li>
    <li>random</li>
    <li>shutil</li>
    <li>warnings</li>
    <li>matplotlib</li>
    <li>ultralytics</li>
    <li>sklearn.model_selection</li>
    <li>rasterio</li>
    <li>osgeo</li>
    <li>PIL</li>
    <li>zipfile</li>
</ul>

## Install

Basic dependencies stated in requirements.txt

To install dependencies: `pip install -r requirements.txt `

## Project Organization
------------

    ├── LICENSE
    ├── README.md                           <- The top-level README for developers using this project.
    ├── data
    │   ├── interim                         <- Intermediate data that has been transformed
    │   │    └── YOLO txt                   <- Folder contain annotated images with YOLOv8 format
    │   ├── processed                       <- The final, canonical data sets for modeling.
    │   │    └── Train folder
    │   │    └── Test folder
    │   │    └── Val folder     
    │   │    └── classes.txt
    │   │    └── notes.json
    │
    ├── models                              <- Trained and serialized models, model predictions, or model summaries
    │   └── YOLOv8_model.pkl                <- YOLOv8 model
    │
    ├── notebooks                           <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                                           the creator's initials, and a short `-` delimited description, e.g.
    │                                           `1.0-jqp-initial-data-exploration`.
    │   └── YOLOv8.ipynb                    <- Notebook to create model
    │
    ├── references                          <- Data dictionaries, manuals, and all other explanatory materials.
    │   └── Phase-1 Benchmark Notebook      <- Sample Jupyter notebook to create the model
    │       2024 V0.5 1.ipynb
    │   
    ├── src                                 <- Source code for use in this project.
    │   └── features                        <- Scripts to turn raw data into features for modeling
    │         └── merge_dataset.py          <- Scripts to combine annotation images folders  into single file
    │         └── split_train_test_val.py   <- Scripts to split the dataset to train files, test files and validate files
    │
    └── requirements.txt                    <- The requirements file for reproducing the analysis environment, e.g.
                                                generated with `pip freeze > requirements.txt`

## Contributors

Abdullah Syarafuddin Hassan
Muhammad Aliff Izzuddin Mohamed Anuar
Nurul Filzah Abdul Hadi
