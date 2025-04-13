# Increasing Market Share of a Local Indian Cosmetic Brand 

## 🎯 Objective
Devise a data-driven strategy to increase market share for a **local Indian cosmetic company** in the booming **online beauty and personal care** industry.

## 🛍️ Industry Context
- **India's Online BPC Market (2023)**: ~$4.5B, ranked 4th globally.
- **Highly Competitive**: 180+ companies, 1000+ brands.
- **Complex Product Space**: 42 sub-categories, 2400+ variants.

## 📈 Strategy Framework: Ansoff Matrix
Focus only on *existing market strategies*:
- **Market Penetration**: Optimize pricing, availability, promotion, and segmentation.
- **Product Development**: Innovate new products or improve existing ones tailored to Indian consumer needs.

## 📊 Data Overview
Scraped from popular platforms (Amazon, Flipkart, Sephora, Ulta):
- **Attributes**: Name, brand, price, ratings, ingredients, category, subcategory, size, color, form, etc.
- **Cleaning**: Missing values imputed; products classified into Local vs Global, Premium vs Regular.

## 🧠 Data Science Approach

### 🧩 Market Segmentation
- **Problem**: Traditional EDA-based segmentation is biased and oversimplified.
- **Solution**: Used **K-Means Clustering** on features (price, rating, category, size, brand type, etc.).
- **Output**: 3 customer clusters for better product positioning.

### 💸 Price Determinants via Regression
- **Goal**: Understand key factors impacting pricing.
- **Model**: Lasso Regularized Linear Regression
- **Key Insights**:
  - **Global brands** priced higher.
  - **Form (e.g., serums, moisturizers)** correlates positively with price.
  - **Customer Ratings** impact pricing slightly.
  - **Certain ingredients** are clearly associated with Premium or Regular segments.

## 🧪 Ingredient Classification
- **Classified ingredients** by product class (Premium vs Regular).
- **Model Accuracy**: 84% using classification model.
- **Top Ingredients** identified for both tiers to guide new product development.

## 💡 Key Recommendations
- **Segment to Target**: Skincare & Bodycare Essentials (functional + sustainable).
- **Differentiated Pricing**:
  - Premium pricing for facial care.
  - Bulk pricing for body/haircare.
  - Emphasize high-value forms (e.g., serums).
- **Product Development**:
  - Tailor ingredients per price tier.
  - Maintain high product quality to retain high ratings.
- **Data Loop**:
  - Continuously integrate customer feedback and sales data for model retraining and strategic refinement.

## 🔄 Tools & Techniques
- K-Means Clustering (Segmentation)
- Lasso Regression (Price Drivers)
- Ingredient Classification (SVM, Regression)
- Truncated SVD (Visualization)
