# Prediction of Product Sales

## A data-driven analysis to predict total sales for food items at different outlets.
Author: Nasser Kishek

### Business problem:
The problem is that retailers often lack clarity on which products sell best and how outlet features such as size, type, or location influence sales, and without these insights, they risk poor inventory planning, ineffective pricing, and missed opportunities.

### Data:
- **Source:** 
  The dataset was obtained from the (https://www.analyticsvidhya.com/datahack/contest/practice-problem-big-mart-sales-iii/) Which can be downloaded from this link(https://drive.google.com/file/d/1syH81TVrbBsdymLT_jl2JIf6IjPXtSQw/view).  
  It contains retail sales data collected from multiple stores across different locations.

- **Description:**  
  Each record represents the sales performance of a particular product at a specific outlet, along with its attributes such as weight, visibility, category, and store type.

- **Structure:**  
  The dataset consists of **8,523 observations** and **12 features**.  
  The target variable is **`Item_Outlet_Sales`**, which represents the total sales value of each product.

- **Key Features:**  
  - `Item_Weight` – Weight of the product  
  - `Item_Fat_Content` – Indicates whether the product is low fat or regular  
  - `Item_Visibility` – Percentage visibility of the product in the store  
  - `Item_Type` – Category of the product  
  - `Outlet_Size`, `Outlet_Location_Type`, `Outlet_Type` – Store-level attributes  
  - `Item_Outlet_Sales` – (Target) Sales value of each item

### Methods:

### Results:

<img width="723" height="528" alt="HeatMap" src="https://github.com/user-attachments/assets/d03d2955-79c4-44a9-85b2-b3e44ee06674" />
The image above (Heatmap) shows us that Item_MRP and Item_Outlet_Sales has the strongest correlation (0.54) and it is moderately positive and this relationship, indicates that when the MRP increases the sales tend to increase. This could be because higher MRP items are more appealing, of higher quality, or because MRP reflects bundled or premium products.

<img width="1014" height="562" alt="Cat-cols" src="https://github.com/user-attachments/assets/0cb045a0-9eaf-4123-83ec-64030ef8d5ef" />
The chart above clearly shows that Supermarket Type1 is by far the most common outlet type in the dataset, with over 5,500 record.
Also The majority of products are categorized as Low Fat, indicating a trend toward health-conscious labeling or consumer preferences.

### Model

### Recommendations:

### Limitations & Next Steps:

