
Food Recommendation System

This project is a Food Recommendation System that suggests dishes to users based on their preferences, dietary requirements, and past ratings. It combines content-based filtering and collaborative filtering techniques using Python, Pandas, and machine learning algorithms.

Table of Contents

Introduction
Features
Technologies Used
Installation
Usage
Data Description
Recommendation Methods
Results
Contributing
License
Introduction
The Food Recommendation System helps users discover dishes that match their preferences by analyzing various factors such as:

Dietary preferences (Vegetarian, Vegan, etc.)
Allergies (e.g., Nuts, Gluten)
Cuisine preference (Indian, Chinese, Italian, etc.)
Health goals (Low-carb, High-protein, etc.)
User ratings and feedback
It recommends dishes based on:

User profile and preferences (content-based filtering)
Past orders and ratings of similar users (collaborative filtering)
Features
Content-based Recommendations: Suggests dishes based on the user's dietary preferences, allergies, and cuisine preferences.
Collaborative Filtering: Recommends dishes by analyzing the past ratings and feedback of similar users.
User Profile Customization: Considers the user's health goals and dietary restrictions.
Dynamic Filtering: Excludes dishes containing ingredients the user is allergic to.
Technologies Used
Programming Language: Python
Libraries:
Pandas: For data manipulation and analysis
Scikit-learn: For machine learning algorithms
NumPy: For numerical operations
TF-IDF Vectorizer: For text feature extraction
Cosine Similarity: For calculating similarity between user preferences and dishes
Installation
To set up the project locally, follow these steps:

Clone the repository:

bash
Copy code
git clone https://github.com/your-username/food-recommendation-system.git
cd food-recommendation-system
Install the required packages:

bash 
Copy code
pip install pandas scikit-learn
Run the script:

bash
Copy code
python main.py
Usage
User Data: Provide user data including age, gender, dietary preferences, allergies, preferred cuisine, and health goals.
Dish Data: Input dish details such as cuisine, dietary tags, ingredients, calories, and spiciness level.
Order Data: Input historical order data including user ratings and feedback.
The system will output:

Top recommended dishes based on user profile
Suggestions using collaborative filtering based on similar users
Data Description
User Data:

user_id: Unique identifier for each user
age, gender: Demographics
dietary_preference, allergies: User-specific dietary information
preferred_cuisine, health_goals: Preferences for recommendations
Dish Data:

dish_id: Unique identifier for each dish
name, cuisine, dietary_tags: Dish details
ingredients, calories, spiciness: Nutritional information
Order Data:

order_id, user_id, dish_id: Identifiers for orders
rating, feedback: User feedback and ratings
quantity, total_price: Order details
Recommendation Methods
1. Content-Based Filtering
Uses user profile information like dietary preferences, allergies, and preferred cuisine.
Computes similarity scores between user preferences and dish attributes using TF-IDF Vectorizer and Cosine Similarity.
2. Collaborative Filtering
Utilizes the past ratings of users to identify similar users.
Employs Nearest Neighbors algorithm to find similar users based on their ratings.
Suggests dishes that have high ratings from similar users.
















