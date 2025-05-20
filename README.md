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
``` 
## Setup

- Download the dataset from Kaggle:  
  https://www.kaggle.com/datasets/hugodarwood/epirecipes  
  Or use Kaggle API in Google Colab to download directly.

- Load the dataset into the notebook.

- Run the notebook cells sequentially to execute data cleaning, feature engineering, and model code.

## Usage

- Input your available ingredients as a comma-separated list.

- The system calculates scores and recommends the top matching recipes.

- View matched and missing ingredients, recipe rating, and coverage percentage.

Example usage snippet:

```python
user_ingredients = ['eggs', 'onion', 'cheese', 'tomato']
recommendations = recommend_recipes_with_missing(user_ingredients, recipes)
print(recommendations)
```
## Future Improvements

- Add dietary and allergen filters (vegan, gluten-free, etc.)
- Implement ingredient substitutions for missing items
- Develop a standalone web or mobile app frontend
- Incorporate user feedback for continuous recommendation tuning
- Enhance nutritional scoring with personalized goals

## Project Structure

- `RecipeRecommender.ipynb` — main Jupyter notebook with full implementation and interactive UI
- `README.md` — project documentation
- (Optional) Dataset files or scripts for data loading

## License

This project is open-source and available under the MIT License.

## Acknowledgments

- Dataset provided by Epicurious Recipes Dataset on Kaggle  
- Thanks to the open-source community and contributors of pandas, ipywidgets, and other libraries

---

Feel free to reach out if you have questions or want to contribute!
