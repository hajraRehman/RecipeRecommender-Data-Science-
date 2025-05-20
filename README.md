# Recipe Recommendation System

A data science project that recommends recipes based on user-provided ingredients. This system analyzes a large recipe dataset, leveraging ingredient matching, coverage ratios, and recipe quality (ratings and nutrition) to suggest practical and relevant cooking options.

---

## Project Overview

Finding the perfect recipe based on what you have in your kitchen can be challenging. This project builds a data-driven Recipe Recommendation System that takes a list of ingredients you have on hand and suggests recipes you can make — highlighting matched ingredients and what’s missing to complete the recipe.

The system uses the Epicurious Recipes Dataset, which contains over 200,000 recipes with detailed ingredient lists, nutrition information, and user ratings.

---

## Features

- **Ingredient matching:** Compares user’s available ingredients with recipe ingredients  
- **Ingredient coverage:** Measures how much of the recipe’s ingredients are matched  
- **Recipe quality scoring:** Incorporates normalized recipe ratings and nutrition data  
- **Missing ingredients:** Lists what additional ingredients are needed for each recommended recipe  
- **Flexible matching:** Supports partial matches and ingredient subsets  
- **Interactive interface:** Users can input ingredients and get recommendations in a Jupyter notebook with widgets  

---

## Dataset

This project uses the [Epicurious Recipes Dataset](https://www.kaggle.com/datasets/hugodarwood/epirecipes) from Kaggle. The dataset includes:  

- Recipe titles  
- Ingredient presence as binary columns  
- Nutrition facts (calories, protein, fat, sodium)  
- User ratings and tags  

---

## Getting Started

### Prerequisites

- Python 3.7+  
- Jupyter Notebook or Google Colab  
- Required libraries: `pandas`, `ipywidgets`, `numpy`  

You can install the required libraries via pip:

```bash
pip install pandas ipywidgets numpy
