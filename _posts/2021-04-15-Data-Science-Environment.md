---
published: true
description: A logical, reasonably standardized, but flexible project structure for doing and sharing data science work.
categories: [data_science]
title: Data Science Project Environment
---
![](/assets/images/ds_project.jpg?raw=true){: .center-image }
# Step by step procedure to setup any data science project.

## Basic setup
1. Install cookiecutter

   ```
   conda install cookiecutter
   ```

2. Starting a new project

   ```
   cookiecutter https://github.com/drivendata/cookiecutter-data-science
   ```
   
3. Create a virtual environment

   ```
   conda create -n virtual-env-name python==3.8
   conda activate virtual-env-name
   ```
   
4. Install all the [general packages](https://gist.github.com/alokrajg/4070069eb7f4253864b494eb91a0d013) for data science

   ```
   conda install --file requirements.txt
   ```
   or
   
   ```
   conda install pip
   pip install -r requirements.txt
   ```
   
5. Open jupyter lab for data exploration and analysis
   
   ```
   jupyter lab
   ```
   
