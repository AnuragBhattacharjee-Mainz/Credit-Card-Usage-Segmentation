# 💳 Credit Card Usage Segmentation Project

_Clustering customers based on their credit card usage patterns to identify distinct customer segments and provide insights for targeted marketing and business strategies._

---

## 📌 Table of Contents
- <a href="#Overview">Overview</a>
- <a href="#Business-Problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#Tools-&-technologies">Tools & Technologies</a>
- <a href="#Project-Structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Cleaning and Preparation</a>
- <a href="#Exploratory-Data-Analysis-eda">Exploratory Data Analysis (EDA)</a>
- <a href="#Modeling & Segmentation">Modeling--segmentation </a>  
- <a href="#Key Insights">key-insights </a>  
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#further-recommendations">Further Recommendations</a>
- <a href="#author--contact">Author & Contact</a>

---


---
<h2><a class="anchor" id="Overview"></a>Overview</h2>

This project applies **unsupervised machine learning techniques** to segment credit card customers into meaningful clusters or groups.  
By analyzing their card usage behavior, the model helps financial institutions design targeted strategies for:  
- Personalized offers  
- Customer retention   
- Inactive customers
- Risk management 

---

---

<h2><a class="anchor" id="Business-Problem"></a>Business Problem</h2>

Banks and financial institutions need to better understand their customers’ **credit card usage patterns**.  
- The project aims to:  
  - Identify **distinct customer groups** based on spending and repayment behavior  
  - Help in **improving customer satisfaction** with tailored services  
  - Support **marketing campaigns** for specific customer segments  
  - Reward loyal customers, identify and predict **high risk customer**   

---

---

<h2><a class="anchor" id="dataset"></a>Dataset</h2>

- Dataset used: **Customer Data**  
- Contains customer-level details such as:  
  - Balance, Purchases, Cash Advances  
  - Credit Limit, Payments, Tenure  
  - Purchase frequency & types
  - There are 18 columns in total

---

📂 File Location: `[Customer Data.csv] (./data/Customer Data.csv)`  

---


<h2><a class="anchor" id="Tools-&-technologies"></a>Tools & Technologies</h2>

---

- **Python**: Pandas, NumPy, Matplotlib, Seaborn  
- **Scikit-learn**: StandardScaler, PCA, KMeans, AgglomerativeClustering, silhouette_score, TSNE
- **Git and GitHub** 
- **Jupyter Notebook**  

---

---
<h2><a class="anchor" id="Project-Structure"></a>Project Structure</h2>

```
credit-card-usage-segmentation/
│
├── README.md
├── requirements.txt
├── Credit_card_Usage_Segmentation_Project.pdf
├── Credit_card_Usage_Segmentation_Project.ipynb
├── data/ # [Customer Data.csv]
├── Images/
├── Output_files/
```
---

---
<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning and Preparation</h2>

- Handled missing values  
- Treated outliers and filled missing values based on median 
- Standardized numerical features using **StandardScaler**  
- Applied **Principal Component Analysis (PCA)** for dimensionality reduction
- Applied t-SNE method on dataset in 2 Dimension 

---

<h2><a class="anchor" id="Exploratory-Data-Analysis-eda"></a>Exploratory Data Analysis (EDA)</h2>

- Distribution analysis of customer spending, balance, and credit usage
- Visualization of dataset for representing the null values using a SNS heatmap  
- Detection of high vs. low spenders, frequent vs. occasional users
- Correlation heatmap of key financial metrics  

**Correlation Analysis:**
- Strong correlation between purchases and OneOff Purchases
- Negative correlation between balance and prc full payment

---

<h2><a class="anchor" id="Modeling & Segmentation"></a>Modeling and Segmentation </h2>

---
- **Clustering Algorithm Used**: KMeans  
- **Optimal Number of Clusters** chosen using:  
  - Elbow Method  
  - Silhouette Score  
  
- **Clustering algorithm used**: Agglomerative
- **Optimal number of clusters** chosen using:
- Silhouette Score

- Other clusturing method used for visulizing datasets: 
  - Principal Component Analysis (PCA)
  - t-distributed Stochastic Neighbor Embedding (t-SNE)
---

Final Model:  
- Segmented customers into **[4] clusters**  
- Cluster profiles created based on usage patterns and financial behavior  
---

<h2><a class="anchor" id="Key Insights"></a>Key Insights </h2>

-  segment 1 characteristics: High Earners, high spenders, low credit risk customers
-  segment 2 characteristics: Low Balance, high spenders, Percent full payments are low, High risk customers 
-  segment 3 characteristics: Low Balance, low average purchases, low credit utilisation, Inactive customers
-  segment 4 characteristics: Good Balance, good credit ratio, low average purchase amount, potential for more spending  

---

<h2><a class="anchor" id="how-to-run-this-project"></a>How to Run This Project</h2>

1. Clone the repository:
```bash
git clone https://github.com/AnuragBhattacharjee-Mainz/Credit-Card-Usage-Segmentation.git
```
---
---
2. Install dependencies:
```bash
pip install -r requirements.txt
```
---
3. Load the CSV file:
```bash
python data/Customer Data.csv
```
---
4. Run the Jupyter Notebook:
```bash
- jupyter notebook Credit_card_Usage_Segmentation_Project.ipynb
```
---
<h2><a class="anchor" id="further-recommendations"></a>Further Recommendations</h2>

---
- The output file "cluster_groupby_values" can be further used to visualise insights of customer segments using BI software
- The output files "Cluster_0" to "Cluster_3" can be used to extract further business insights for each customer group  

---

<h2><a class="anchor" id="author--contact"></a>Author & Contact</h2>

- **Anurag Bhattacharjee**
- Aspiring Data Scientist
- 🔗 [LinkedIn](https://www.linkedin.com/in/anurag-process-analyst) 
- 🔗 [Xing](https://www.xing.com/profile/ANURAG_BHATTACHARJEE/web_profiles)
---

