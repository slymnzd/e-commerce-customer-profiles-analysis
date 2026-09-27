# E-Commerce Customer Profiles Analysis

## Project Overview

This project analyzes e-commerce customer data to identify and understand different customer profiles based on their **demographic and behavioral characteristics**.

The analysis focuses on customer purchasing behavior, engagement, customer value, and product preferences. Customers are grouped into **Demographic Profiles** and **Behavioral Profiles**, which are then analyzed individually and in combination.

The project aims to provide a structured understanding of the customer base and identify customer groups that can support more targeted business and marketing decisions.

---

## Project Objective

The main objective of this project is to create **Customer Profiles (CP)** based on defined demographic and behavioral parameters and to understand the characteristics and purchasing behavior of each profile.

The analysis aims to identify differences between customer groups in terms of:

* Customer value
* Purchasing frequency
* Revenue contribution
* Product preferences
* Customer behavior and engagement

---

## Dataset

The dataset contains **17,049 e-commerce transactions** from **5,000 unique customers** and includes demographic, purchasing, behavioral, and customer experience variables.

### Main Data Categories

* **Customer Demographics:** Age, Gender, City
* **Purchase Information:** Product Category, Unit Price, Quantity, Discount Amount, Total Amount
* **Customer Behavior:** Session Duration, Pages Viewed, Returning Customer
* **Customer Experience:** Delivery Time, Customer Rating
* **Transaction Information:** Order ID, Customer ID, Date, Payment Method, Device Type

Additional variables such as **Age Group** and **Discount Status** were created during the data preparation stage. **Demographic Profiles** and **Behavioral Profiles** were created later as part of the analysis.

---

## Data Cleaning & Preparation

The dataset was reviewed and prepared before conducting the analysis.

The main preparation steps included:

* Checking the dataset structure and data types
* Checking for missing values
* Checking for duplicate records
* Converting the **Date** column to datetime format
* Creating **Age Group** categories
* Creating **Discount Status** based on discount usage

The prepared dataset was then used for Exploratory Data Analysis and subsequent Customer Profile analysis.

---

## Exploratory Data Analysis

Exploratory Data Analysis (EDA) was conducted to understand the main characteristics and patterns within the dataset before customer profiling.

The analysis examined:

* Customer age groups and gender distribution
* Customer distribution by city
* Product category distribution
* Quantity and pricing characteristics
* Returning customer behavior
* Discount usage
* Session duration and pages viewed
* Customer ratings
* Delivery time

The EDA provided an initial understanding of customer and purchasing patterns and helped define the variables used in the subsequent analysis.

---

## Analysis

The main part of the project focuses on creating and analyzing **Customer Profiles (CP)** to understand differences in customer characteristics, purchasing behavior, and customer value.

### Demographic Profile Analysis

Customers were grouped into **Demographic Profiles** using their **Age Group** and **Gender** characteristics. The profiles were created at the unique customer level rather than at the transaction level.

A total of **13 Demographic Profiles** were created, representing different age and gender combinations, together with an **Others** group for customers who did not fall into the predefined demographic groups.

The profiles were compared using:

* Customer Count
* Total Order Count
* Order Count per Customer
* Total Amount
* Average Amount per Customer
* Revenue Contribution (%)

The profiles were also examined based on their product category preferences and loyalty-related purchasing behavior.

A performance scoring approach was used to compare the demographic groups across the selected metrics and identify profiles with stronger overall performance.

### Behavioral Profile Analysis

Behavioral Profiles were created to capture differences in **customer purchasing and engagement behavior**.

The profiling process was performed at the **customer level**. Customer transactions were first aggregated to calculate behavioral indicators. Customers were then classified into behavioral levels, combined into behavioral patterns, and mapped to predefined Behavioral Profiles.

The profiling process considered five main behavioral dimensions:

* **Pages Viewed** — browsing and platform engagement
* **Session Duration** — time spent on the platform
* **Returning Customer Behavior** — level of returning purchase behavior
* **Discount Usage** — proportion of orders made with a discount
* **Quantity** — average quantity purchased per order

Based on combinations of these behavioral characteristics, **15 predefined Behavioral Profiles** were created, together with an **Other** group for patterns that did not match the predefined profiles.

The Behavioral Profiles include:

* **Standard**
* **No Disc. Standard**
* **Loyal**
* **Discount-Oriented**
* **Engaged**
* **No-Disc. Engaged**
* **Disc.-Oriented Engaged**
* **Disc.-Engaged Loyal**
* **Quick Buyers**
* **Bulk Buyers**
* **Disc.-Oriented Quick**
* **No-Disc. New Customers**
* **Quick Explorers**
* **Slow Explorers**
* **Disc.-Oriented New Customers**
* **Other**

These profiles were then analyzed based on customer count, purchasing frequency, customer value, average purchase quantity, revenue contribution, and product category preferences.

A performance scoring approach was also applied to compare Behavioral Profiles across multiple customer and purchasing metrics.

### Demographic & Behavioral Profile Analysis

The final stage combined **Demographic Profiles** and **Behavioral Profiles** to provide a more detailed view of the customer base.

Each customer was analyzed according to both their demographic and behavioral characteristics, allowing profile combinations to be compared in terms of:

* Customer Count
* Average Amount per Customer
* Total Amount
* Product Category Preferences

This analysis was used to identify the **highest-value Demographic & Behavioral Profile combinations** and to examine how customer behavior differs across demographic groups.

The combination analysis showed that **customer volume and customer value do not necessarily follow the same pattern**, highlighting the importance of analyzing both dimensions together.

---

## Key Insights

The Customer Profile analysis revealed several important differences between **customer volume, purchasing behavior, and customer value**.

### Customer Base Structure

The demographic analysis shows that the customer base is largely concentrated in the **25–44 age range**. Among the demographic groups, **D8** has the highest number of customers with **758 customers**, followed by **D7** with **738 customers**.

However, customer count alone does not explain customer value. The demographic performance analysis shows that the largest customer group is not necessarily the strongest-performing group across all value-related metrics.

### Behavioral Profiles Drive Customer Value

The Behavioral Profile analysis revealed a clear difference between the size of a customer group and its economic contribution.

**Standard** is the largest Behavioral Profile with **946 customers**, making it the most common behavioral pattern in the customer base. However, **Loyal** customers, despite being fewer in number, demonstrate stronger purchasing performance across multiple indicators.

The performance scoring confirms this difference:

* **Loyal — 17 stars**
* **Standard — 9 stars**
* **Bulk Buyers — 6 stars**
* **Disc.-Engaged Loyal — 4 stars**
* **Other — 4 stars**

This indicates that the most common customer behavior is not necessarily the behavior that creates the highest customer value.

### Revenue Concentration

Revenue analysis further highlights the importance of specific behavioral groups.

**Loyal customers generate 22.30% of total revenue**, representing the largest revenue contribution among Behavioral Profiles. Standard customers contribute **18.72%**, while Engaged customers contribute **8.14%**.

These results show that a relatively small number of Behavioral Profiles account for a substantial share of total revenue.

### Purchase Frequency and Customer Value

The analysis of **Order Count per Customer** and **Average Amount per Customer** shows a **positive relationship between purchasing frequency and customer value**.

The **Loyal** profile is particularly notable because it performs relatively strongly on both dimensions.

This indicates that repeat purchasing behavior is an important characteristic when identifying higher-value customers within the dataset.

### Different Profiles Show Different Product Preferences

Product preferences are not identical across Behavioral Profiles.

For example:

* **Quick Explorers** show their highest category share in **Books (17.02%)**.
* **No-Disc. New Customers** show their highest category share in **Fashion (16.13%)**.
* **Other** customers show their highest category share in **Sports (16.35%)**.
* **Slow Explorers** show their highest category share in **Books (15.86%)**.

These differences indicate that Behavioral Profiles can provide additional information about **what different types of customers prefer to purchase**, beyond simply measuring how much they spend.

### Demographic + Behavioral Combinations Reveal Higher-Value Groups

Combining the two profiling dimensions provides a more detailed view of customer value.

The largest customer combinations are:

* **D7 + Standard — 153 customers**
* **D5 + Standard — 144 customers**
* **D6 + Standard — 137 customers**

However, the highest-value combinations are different:

* **D5 + Loyal — 821,831.79**
* **D7 + Loyal — 780,904.41**
* **D6 + Loyal — 704,780.61**

All three of the highest-value combinations are associated with the **Loyal** Behavioral Profile.

This is one of the key findings of the project: **the customer groups with the largest number of customers are not necessarily the groups generating the highest customer value**.

### Overall Finding

The analysis demonstrates that looking at customers from only one perspective can hide important differences.

**Demographic Profiles** help explain **who the customers are**, while **Behavioral Profiles** help explain **how they behave and purchase**. Combining both dimensions makes it possible to identify customer groups that are not only large in size, but also economically valuable.

The results support a more **customer-value-oriented approach to segmentation**, where customer count, purchasing frequency, revenue contribution, product preferences, and behavioral characteristics are considered together.

---

## Recommendations

Based on the Customer Profile analysis, several potential business and marketing actions can be considered.

### 1. Focus on Loyal Customers

Loyal customers generate the highest revenue contribution (**22.30%**) and demonstrate the strongest overall behavioral performance.

The company could focus on retaining these customers through personalized offers, relevant product recommendations, loyalty benefits, and customer retention campaigns.

### 2. Develop Targeted Strategies for High-Value Combinations

The highest-value Demographic & Behavioral combinations are **D5 + Loyal, D7 + Loyal, and D6 + Loyal**.

These groups could be analyzed further to understand their common characteristics and used as specific targets for personalized marketing campaigns.

### 3. Use Behavioral Profiles for Customer Targeting

Different Behavioral Profiles demonstrate different purchasing and engagement patterns.

Instead of applying the same marketing strategy to all customers, campaigns could be adapted to behavioral characteristics such as purchasing frequency, engagement level, discount usage, and purchase quantity.

### 4. Personalize Product Recommendations

Differences in product category preferences across Behavioral Profiles suggest that product recommendations can be adapted to specific customer groups.

For example, customers showing stronger preferences for **Books, Fashion, or Sports** could receive more relevant product recommendations and category-specific campaigns.

### 5. Encourage New Customers to Make Repeat Purchases

Profiles such as **No-Disc. New Customers** and **Disc.-Oriented New Customers** represent customers who have not yet developed strong returning behavior.

Targeted follow-up campaigns, personalized recommendations, and carefully designed incentives could be used to encourage a second purchase and support customer retention.

### 6. Evaluate Customers Beyond Customer Count

The analysis shows that the largest customer group is not necessarily the highest-value group.

Therefore, customer targeting and resource allocation should consider multiple indicators, including **customer value, purchasing frequency, and revenue contribution**, rather than relying only on customer count.

---

## Conclusion

This project used customer-level demographic and behavioral segmentation to develop a structured understanding of the e-commerce customer base.

The analysis showed that **customer volume, purchasing frequency, and customer value do not always follow the same pattern**. While Standard customers represent the largest Behavioral Profile by customer count, Loyal customers demonstrate stronger overall performance and generate the highest share of total revenue.

The combination of Demographic and Behavioral Profiles provided an even more detailed view of customer value. In particular, the highest-value combinations were all associated with the **Loyal** Behavioral Profile, highlighting the importance of repeat purchasing behavior when evaluating valuable customer groups.

Overall, the project demonstrates how customer profiling can transform transaction-level data into meaningful customer segments and business insights. The resulting profiles can support more targeted approaches to **customer retention, marketing, product recommendations, and customer value management**.

---

## Tools & Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**
* **Git & GitHub**
