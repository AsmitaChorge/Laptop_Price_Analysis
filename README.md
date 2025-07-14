💻 Project Report: Laptop Price Analysis

1. Project Overview
   
🎯 Objective:
To analyze laptop specifications and their impact on pricing. 
The goal is to understand key features influencing laptop prices and help both customers and sellers make informed decisions through data-driven insights.

2. Dataset Description
Source: E-commerce laptop product listings.

Size: ~1300 rows, 12+ columns.


Features:
Company, TypeName, Inches, ScreenResolution, Cpu, Ram, Memory, Gpu, OpSys, Weight, Price

3. Tools & Libraries Used
Language: Python


Libraries:
Pandas, NumPy – data cleaning and manipulation

Matplotlib, Seaborn – data visualization

Scikit-learn – label encoding (if applicable)


Platform: Jupyter Notebook / Google Colab




4. Data Preprocessing
Null Values: Checked and confirmed no nulls.


Data Cleaning:
Removed 'GB' from RAM and Memory fields, converted to numeric


Extracted important subfields:
e.g., From ScreenResolution: identified touchscreen presence


From Cpu: extracted brand like Intel, AMD, etc.


Feature Engineering:


Created new columns like Touchscreen, IPS, X_res, Y_res, ppi (Pixels per Inch)


Converted RAM/Memory to integer for analysis



5. Exploratory Data Analysis (EDA)
a. Price Distribution
Most laptops are priced between ₹30,000 to ₹70,000


Very few laptops priced above ₹150,000


📌 Insight:
Market is dominated by mid-range laptops. Premium laptops are niche.

b. Company-wise Price Trends
Top Brands by Price (on average):


Apple and MSI are the most expensive


HP, Lenovo, Acer offer more budget-friendly laptops


📌 Business Insight:
Brand perception and OS significantly affect pricing. Apple commands a premium due to brand loyalty and macOS.

c. Type of Laptop vs Price
Gaming, Workstation, and Ultrabooks are more expensive.


Notebooks and Netbooks are cheaper.


📌 Suggestion:
Target marketing based on user intent: gaming laptops for youth, ultrabooks for professionals, notebooks for students.

d. Touchscreen Impact
Touchscreen laptops are more expensive on average.


Detected using binary flag in ScreenResolution column.


📌 Insight:
Touchscreen adds premium value. Highlight touchscreen functionality in promotions for higher conversions.

e. Screen Resolution and PPI
High resolution (4K) and higher ppi (pixels per inch) significantly increase price.


ppi was calculated using screen size and resolution.


📌 Insight:
Visual creators and designers are likely to buy high-ppi laptops. Market those models specifically on creative platforms (YouTube, Behance, etc.).

f. CPU Brand vs Price
Laptops with Intel Core i7, i9, and AMD Ryzen 7 are more expensive.


i3, AMD A9, Pentium come under budget models.


📌 Suggestion:
Use CPU brand as a strong price predictor in recommender systems.

g. RAM vs Price
Direct correlation: Higher RAM = Higher price


8GB and 16GB are the most common configurations


📌 Insight:
RAM is a major selling point; upsell RAM upgrades as a customization option.

h. Storage vs Price
SSD > HDD in terms of pricing


Laptops with SSD-only storage are more expensive and perform better


📌 Business Suggestion:
Promote SSD models as "fast-boot", "student-friendly", and "future-ready" systems.

i. GPU Impact
Laptops with dedicated GPUs (NVIDIA, AMD) are costlier


Integrated graphics (Intel UHD, etc.) are cheaper


📌 Insight:
Highlight GPU-based differentiation while promoting gaming or creative laptops.

j. Operating System vs Price
macOS and Windows laptops are more expensive than DOS or Linux-based ones.


Windows dominates the dataset.


📌 Insight:
macOS drives up pricing. Bundle Windows + Office in entry-level laptops to add perceived value.

6. Key Business Insights
Factor
Insight
Recommendation
Brand
Apple and MSI are premium
Use influencer marketing for Apple-like perception
Touchscreen
Adds ₹10k–₹20k premium
Upsell as a premium feature
Storage Type
SSD boosts performance & price
Phase out HDD-only models
RAM/CPU
Core i5/i7 + 8/16GB drives mid/high range
Offer EMI and exchange for upgrades
OS
macOS > Windows > DOS/Linux in pricing
Highlight Windows licensing in ads
Usage Type
Gaming/Workstation are expensive niches
Segment audiences and personalize ads
Screen Features
Higher ppi → higher price
Market as creative/visual tools


7. Business Recommendations
🧠 Product Strategy
Segment products based on user profile:


Students: Affordable notebooks (Intel i3, 4GB, HDD)


Professionals: Ultrabooks (Intel i5/i7, SSD, 8GB+ RAM)


Gamers/Designers: Dedicated GPU, high PPI, i7/i9


📢 Marketing Strategy
Promote SSD-based laptops as faster and more reliable.


Run comparative ads highlighting value-for-money in mid-range models.


Push gaming laptops with offers on Steam Wallet, Game Pass, etc.


📦 Inventory Planning
Stock up mid-range configurations (₹45k–₹70k, i5 + 8GB + SSD)


Reduce models with only HDD or 4GB RAM (low demand)



8. Conclusion
The analysis identifies key factors influencing laptop pricing — including brand, CPU, RAM, storage type, screen specs, and more. These findings empower e-commerce platforms and retailers to improve their product listings, promotional targeting, and inventory decisions.

9. Future Scope
Apply Machine Learning Regression Models (e.g., Linear Regression, XGBoost) to predict laptop prices based on specs.


Build a Laptop Recommendation System using similarity measures.


Incorporate customer reviews/ratings to evaluate perceived value vs price.

