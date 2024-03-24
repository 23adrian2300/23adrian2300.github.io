---
layout: project
type: project
image: img/data_explorer/data_logo.png
title: "Data_explorer"
best: 3
date: 2024
published: true
labels:
  - Python
  - Flask
  - NextJS
summary: "This is a project created for software engineering classes."
---


## Description
This is a project designed to meet the requirements outlined at the bottom of the page. In short, the project aims to facilitate the analysis of CSV files.

Source: <a href="https://github.com/23adrian2300/Data_Explorer">Python/Data_Explorer</a>


## My Contributions at Work

As part of the work division, I was mainly assigned to backend tasks. There, I created appropriate routes that enabled operations such as file saving, setting the mean, updating files and columns, etc. Occasionally, I also made some small changes in the frontend, such as adding a button or improving the display of empty columns and rows in a different color.

## App appearance

On the main screen, you can see the loaded CSV file, and you can click on a column, save the entire file, or just individual columns.

<div class="text-center p-4">
  <img width="800" height="600" src="../img/data_explorer/main_screen.png" class="img-thumbnail" >

</div>

On the column screen, we see all parameters such as mean, median, etc. We can fill in empty cells or manually change them using the update option.

<div class="text-center p-4">
  <img width="800" height="600" src="../img/data_explorer/column_data.png" class="img-thumbnail" >

</div>

We can also compare two columns, where we get the most important information about them in one place.

<div class="text-center p-4">
  <img width="800" height="600" src="../img/data_explorer/compare_data.png" class="img-thumbnail" >

</div>

## Requirements

Project: Application for preliminary data analysis and visualization. Assumptions: Single-stage login. Data is retrieved from CSV files. Number of variables (up to 100). Expected functionalities:

- Automatic detection of data types with editing capability.
- Simple variable name changes.
- Basic 1D EDA descriptive statistics (appropriate to variable type) - expected suggestions.
- Basic visualizations of a single variable (appropriate to variable type) within a specified time range - expected suggestions.
- Filling in missing values / correcting outlier values for variables (appropriate to variable type) - expected suggestions (ability to easily return to point 3).
- Basic measures of dependencies between variables 2D EDA (appropriate to variable types) - expected suggestions.
- Basic visualizations of two/three variables (appropriate to variable types) within a specified time range - expected suggestions. Additionally:
- data retrieval by the user (CSV file) from a specified range (variable selection, case selection).
- ability to save generated plots in jpg and png formats. The output of the application is a "cleaned" data set for further analysis.
