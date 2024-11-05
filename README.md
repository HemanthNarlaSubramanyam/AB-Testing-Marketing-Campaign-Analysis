# AB-Testing-Marketing-Campaign-Analysis 
![image](https://github.com/user-attachments/assets/cdfd393f-c035-48c9-95f8-e4b5fb7d4e83)

## **Overview**
This project performs **A/B Testing** to evaluate the effectiveness of a marketing campaign. A/B testing is a powerful method used in marketing to compare two variants of a campaign to determine which one performs better. In this project, we analyze two test groups: users exposed to **advertisements (Ad group)** and those shown **public service announcements (PSA group)**, measuring their **conversion rates**.

## **Dataset**
The dataset consists of **588,101 entries** with the following columns:
- **User ID**: A unique identifier for each user.
- **Test Group**: Specifies whether the user was in the **Ad** group (saw advertisements) or the **PSA** group (saw public service announcements).
- **Converted**: A boolean field indicating whether the user purchased a product (**True** for purchase, **False** otherwise).
- **Total Ads**: The number of ads the user saw.
- **Most Ads Day**: The day the user saw the highest number of ads.
- **Most Ads Hour**: The hour of the day the user saw the most ads.

## **Steps Involved**
- **Data Loading**: The dataset is loaded and inspected to ensure there are no missing or duplicated entries.
- **Data Cleaning**: Unnecessary columns, such as `Unnamed: 0`, are dropped for cleaner analysis.
- **Exploratory Data Analysis (EDA)**:
  - The distribution of users across test groups is analyzed.
  - Conversion rates for the **Ad** and **PSA** groups are calculated.
- **Group-Level Performance**:
  - Purchase rates for both the **Ad** and **PSA** groups are determined.
- **Statistical Testing**:
  - A **Z-test** is performed to check if the difference in conversion rates between the two groups is statistically significant.

## **Results**
- **Conversion Rates**:
  - **Ad Group**: *2.55%* conversion rate.
  - **PSA Group**: *1.79%* conversion rate.
  
- The **Z-test** results indicate that the Ad group has a **significantly higher conversion rate** compared to the PSA group with:
  - **Z-Score**: *7.37*
  - **P-Value**: *8.53e-14*

Since the P-value is much lower than the significance level (*0.05*), we **reject the null hypothesis**, confirming that the Ad group outperforms the PSA group.

## **Conclusion**
The analysis demonstrates that the **Ad group** achieves a significantly higher conversion rate than the **PSA group**, validating the effectiveness of the advertising campaign. This suggests that **investing in advertisements** can drive higher conversions and, ultimately, business success.

### **Key Insights**:
- Ads result in **higher conversions** than PSAs.
- Statistical evidence supports the **significant difference** in conversion rates.
