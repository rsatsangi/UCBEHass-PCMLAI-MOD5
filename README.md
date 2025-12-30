# Will the Customer Accept the Coupon?

## Project Overview
This project analyzes a real-world behavioral dataset from the **UCI Machine Learning Repository** to identify factors that influence whether a driver accepts a mobile coupon delivered while driving. The data was collected via an **Amazon Mechanical Turk** survey in which participants evaluated simulated driving scenarios and indicated whether they would accept various coupon offers.

**Primary Research Question:**  
What demographic, behavioral, and contextual factors distinguish drivers who accept coupons from those who reject them?

---

## Dataset Summary
- **Source:** UCI Machine Learning Repository  
- **Collection Method:** Amazon Mechanical Turk survey  
- **Observations:** 12,684  
- **Features:** 26  
- **Target Variable:**  
  - `Y = 1` → Coupon accepted  
  - `Y = 0` → Coupon rejected  
- **Coupon Categories:**  
  - Coffee House  
  - Restaurant (<$20)  
  - Carry Out & Take Away  
  - Bar  
  - Restaurant ($20–$50)

---

## Key Findings

### Overall Coupon Acceptance
- **56.93%** of coupons were accepted across all scenarios
- Acceptance rates vary substantially by coupon category, indicating that coupon type is a strong driver of behavior

---

### Acceptance Rate by Coupon Type

| Coupon Type | Acceptance Rate |
|------------|-----------------|
| Carry Out & Take Away | 73.8% |
| Restaurant (<$20) | 70.9% |
| Coffee House | 49.6% |
| Restaurant ($20–$50) | 44.6% |
| Bar | 41.2% |

---

## Bar Coupon Analysis

Bar coupons exhibit the **lowest overall acceptance rate (41.19%)**, making them the least effective category. Further segmentation reveals clear behavioral patterns.

### Visit Frequency as a Primary Driver
- Drivers visiting bars **more than 3 times per month**: **76.17% acceptance**
- Drivers visiting bars **3 times per month or fewer**: **37.27% acceptance**

### Interaction Between Age and Frequency
- Drivers **over age 25** who visit bars **more than once per month**: **68.98% acceptance**
- All other groups: **33.77% acceptance**

### Impact of Passenger Type for a Specific Criterias
- Visit Bar **more than once a month** & **travelling without Kids as Passenger** & **Not a Farming Fishing & Forestry occupation**: **71.43% acceptance**
- Visit Bar **more than once a month** & **Age is < 30**: **70% acceptance**
- Visit Bar **more than once a month** & **travelling without Kids as Passenger** & **Not Widowed**: **64% acceptance**
- Visit **Cheap restaurants more than 4 times a month** and **income is less than 50K**:  **46% acceptance**

### Hypothesis
Based on the observations, drivers who accept bar coupons are likely to be:

- Driver who visits Bar frequently
- Driver who is not driving alone and not having kids as passenegrs. 
   As Bars aren't kid-friendly place.
- Driver who is between 21-30 years of age 
- Drivers who has Friends/Partner as passengers, it is expected for requent 
   Bar visitors as it is social place to go with friends/partner   
- Driver who is not in occupation of Farming/Fishing/Forestry
- Drive who is widowed (Not having Life Partner) is less likely to accept

The data shows that drivers with established bar-going habits are 2–3× more 
likely to accept, indicating that the coupon amplifies existing behavior 
rather than creating new behavior.
Therefore, bar coupons should be sent more frequently to drivers who:
- Visit bars regularly (at least more than once per month),
- Fall within the 21–30 age demographic,
- Are traveling with friends or a partner, and
- Do not have children as passengers.


---

## Coffee House Coupon Analysis

Coffee House coupons show a **moderate acceptance rate (49.63%)**, with acceptance influenced by habitual behavior, time of day, and social context.


### Age-Based Trends
- **Ages Below 21**: **68% acceptance**
- **Ages 21**: **52% acceptance**
- **Ages 26**: **51% acceptance**
- **Ages 50 Plus**: **42% acceptance**


### Time-of-Day Patterns
- **7 AM**: **44% acceptance**
- **10 AM**: **63% acceptance**
- **2 PM**: **55% acceptance**
**The dominant age in the above Time-of-Day is 21**

### Hypothesis
Coffee House coupon acceptance is driven by **routine behavior and social context**, particularly among younger drivers who frequent coffee shops during morning/afternoon hours.

---

## Recommendations for sending Coupons

### Bar Coupons - Target Segments 🍺
- Drivers with bar visit frequency >1/month
- Ages 21–30
- Traveling with friends or a partner but No Kids

---

### Coffee House Coupons - Target Segments ☕
- Frequent coffee house visitors (>1/month)
- Ages 21 or close
- Traveling with friends
- Morning and Afternoon (Post Lunch) - time window (10 AM - 2 PM optimal)


---

## Methodology

The analysis follows a structured exploratory workflow:

- Data inspection and preprocessing
- Univariate statistical summaries
- Group-wise comparisons by acceptance outcome
- Visualization of distributions and conditional relationships
- Interpretation of observed trends
- Visualizations and descriptive statistics are used to identify patterns associated with coupon acceptance behavior.

---

## Technical Details

### Tools & Technologies

- Python
- Jupyter Notebook
- Pandas – data manipulation and aggregation
- NumPy – numerical computation
- Matplotlib / Seaborn – statistical visualization

---

### Repository Structure
```
├── README.md                     # Project documentation
├── data/
│   └── coupons.csv               # Raw dataset
└── Coupons-Data-Analysis.ipynb   # Jupyter Notebook with full analysis
```

---

## Author
**Rupanshu Satsangi**  
UC Berkeley – ML/AI Professional Certificate Program
