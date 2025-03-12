# Product-Recommendation-systems-based-on-Customer-Behaviour
This project builds an AI-driven recommendation system using customer browsing and purchase history to provide personalized product suggestions. It aims to enhance customer engagement and boost sales by delivering tailored recommendations based on user behaviour.

![image](https://github.com/user-attachments/assets/1c16c051-a860-42fb-9474-aa3156fd8235)
  
## 1. Introduction
In the rapidly evolving landscape of e-commerce, **personalized recommendations** are fundamental to enhancing customer engagement and increasing sales. This project develops an **AI-driven product recommendation system** using **collaborative filtering techniques** to analyze **customer browsing and purchase history**. By leveraging **user behavior and product similarity**, the system suggests highly relevant products, improving customer experience and driving revenue growth for **Trafilea**.

## 2. Background
The exponential growth of online shopping has led to an overwhelming number of product choices for customers. Effective recommendation systems help mitigate decision fatigue by guiding customers toward products aligned with their preferences. **Trafilea**, as a leading tech-commerce company, requires a sophisticated recommendation engine to:
- **Enhance product discovery** by recommending items based on browsing and purchase behavior.
- **Increase cross-selling and upselling** through intelligent product pairing.
- **Leverage AI-powered techniques** to personalize customer experiences at scale.
- **Improve customer retention** by offering relevant recommendations tailored to each user.

This project focuses on developing an AI-driven recommendation system that not only enhances customer satisfaction but also optimizes business revenue by predicting and recommending products with high conversion potential.


## 3. Data Collection and Processing
### **Data Sources**
The dataset consists of:
- **orders.csv** → Tracks customer purchases.
- **order_items.csv** → Links customers with purchased products.
- **customers.csv** → Associates orders with customers.
- **products.csv** → Contains product details.
- **product_category_name_translation.csv** → Translates product categories.

### **Data Preprocessing Steps**
- Handling missing values and outliers.
- Converting timestamps to `datetime` format.
- Normalizing numerical values (e.g., price, weight, dimensions).
- Encoding categorical features for model training.
- Creating a **user-item interaction matrix** for recommendation modeling.

## 4. Exploratory Data Analysis (EDA)
### Price and Product Dimension Distribution
![Boxplot of Prices and Dimensions](images/output_34_0.png)

The boxplot analysis shows that **prices, weights, and dimensions of products exhibit significant outliers**. This suggests the need for **data normalization and potential filtering** to avoid skewed recommendations and improve model performance.

### Relationship Between Price and Shipping Cost
![Price vs Shipping Cost](images/output_35_0.png)

The scatter plot reveals a **positive correlation between product price and shipping cost**, but with **high variance**. This indicates that **shipping fees are not strictly proportional** to product prices, suggesting that pricing strategies vary across categories.

### Best-Selling Product Categories
![Top 10 Best-Selling Categories](images/output_40_0.png)

The **top-selling product categories** include:
- **Bed & Bath**
- **Health & Beauty**
- **Sports & Leisure**
- **Furniture & Decor**

These categories represent the **most in-demand products**, making them ideal targets for personalized recommendations and promotional strategies.

### Customer Purchasing Behavior
![Customer Purchase Behavior](images/output_42_0.png)

The analysis indicates that **the majority of customers are one-time buyers**, while only a **small fraction are repeat buyers**. This highlights the **importance of personalized recommendations** to enhance customer retention and encourage repeat purchases.

### One-Time vs. Repeat Buyers
![One-Time vs Repeat Buyers](images/output_47_0.png)

**Repeat buyers tend to purchase from specific categories more frequently than one-time buyers**. This suggests that loyalty-driven strategies, such as **targeted discounts and personalized product suggestions**, can increase customer lifetime value.

### Purchase Preferences Across Categories
![Purchase Preferences Across Categories](images/output_49_0.png)

Categories such as **Bed & Bath, Health & Beauty, and Furniture & Decor attract more repeat buyers**, indicating that these segments have high potential for **customer loyalty programs and retention strategies**.

### Average Price by Category
![Average Price by Category](images/output_52_0.png)

The **highest-priced categories** include:
- **Computers**
- **Home Appliances**
- **Musical Instruments**

High-value items may require **different recommendation strategies**, such as **bundled offers, installment plans, or targeted promotions** to drive conversions.

### Purchase Frequency Across Price Ranges
![Purchase Frequency Across Price Ranges](images/output_55_0.png)

Products in the **medium price range dominate purchases**, while **low and high-priced products see lower frequency**. This suggests that high-priced items may require **discounts or promotional strategies** to boost sales.

### Correlation Between Product Categories and Prices
![Correlation Heatmap of Product Categories & Prices](images/output_58_0.png)

The heatmap shows **strong correlations between product categories and price range**, meaning that certain categories are consistently priced within specific price tiers. This insight can be leveraged for **price-based recommendation strategies**.


## 5. Methodology
### **Recommendation Approaches**
#### **1. User-Based Collaborative Filtering**
- Identifies users with similar purchase histories.
- Recommends products that similar users have purchased.
- **Best for:** Personalized recommendations.

#### **2. Item-Based Collaborative Filtering**
- Finds similar products based on purchase patterns.
- Recommends products frequently bought together.
- **Best for:** Cross-selling and related product suggestions.

#### **3. Hybrid Recommendation System**
- Combines user-based and item-based approaches.
- Generates recommendations considering **both user preference and product similarity**.
- **Best for:** Improving diversity in recommendations.

## 6. Results
- **User-based filtering** provided highly **personalized** recommendations.
- **Item-based filtering** effectively suggested **complementary products**.
- The **hybrid approach** delivered the most balanced recommendations.
- **Cold-start problem** (new users/products) was mitigated using **popularity-based recommendations**.

## 7. Recommendations
- **Personalized Promotions:** Tailor marketing campaigns based on recommendation trends.
- **Real-time Recommendations:** Deploy AI models to update suggestions dynamically.
- **Bundle Offers:** Suggest frequently co-purchased products as discount bundles.
- **Cold-Start Solutions:** Introduce trending/popular products for new users.

## 8. Future Work
- **Deep Learning-Based Recommenders** → Implementing **Neural Collaborative Filtering** and **Transformer models**.
- **Context-Aware Recommendations** → Factoring in seasonality, location, and user intent.
- **A/B Testing** → Evaluating recommendation impact on **customer engagement**.
- **Multilingual Support** → Expanding product recommendations for non-English users.

## 9. Conclusion
This **AI-powered recommendation system** for **Trafilea** improves product discovery and enhances customer experience. By integrating **collaborative filtering** and **hybrid modeling**, the system ensures **highly relevant and diverse** product recommendations, ultimately boosting e-commerce sales.

