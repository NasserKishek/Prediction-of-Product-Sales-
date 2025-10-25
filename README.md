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

<img width="589" height="390" alt="OT vs OS" src="https://github.com/user-attachments/assets/28f60670-7880-4ced-be3b-2434bade3689" />

**Key Insights:**
- Supermarket Type 3 has the highest sales, this means larger or more modern supermarkets generate stronger sales, so investing in these outlets or replicating their model could be more profitable.
- Grocery Stores perform the worst, which shows smaller outlets struggle to generate significant sales. Retailers may need to improve grocery with better product mix or promotions.


<img width="558" height="393" alt="MRP vs OS" src="https://github.com/user-attachments/assets/5f6eab7e-d1f4-4400-9924-a818680ef4dd" />

**Key Insights:**
- Higher MRP products generally generate higher sales, this means expensive items often bring in more revenue per product, likely because their higher price directly increases sales value.
- There is still wide variation at each price level, this shows that not all expensive products sell well. Pricing alone doesn’t guarantee strong sales — demand and product type also matter.
- The moderate correlation (0.57) suggests price is important, but not the only driver, This means while pricing has a big influence, other factors like product category, outlet type, and consumer preferences also shape sales.


  <img width="590" height="390" alt="CDF" src="https://github.com/user-attachments/assets/3ff64cc3-ed23-40b4-b579-081e69beae75" />

**Key Insights:**
- Most products sell in small amounts (80%) – the majority of items generate relatively low sales.
- A small group of products sells much more (20%) – only a few items contribute to the highest sales.
- Sales are not evenly spread – revenue is concentrated in top-performing products, which should get more focus.

### Model:

#### Linear Regression Coefficent

<img width="828" height="547" alt="Lin-Reg Coefficent" src="https://github.com/user-attachments/assets/1c699db5-e026-4132-87e0-24c229cbc8ab" />

Top 3 most impactful features:

1. Item_MRP:
It is the most influential feature in predicting product sales.
A higher Maximum Retail Price (MRP) strongly increases predicted sales, meaning expensive products tend to generate more revenues.
In simple terms: when the MRP increases, sales revenues are expected to rise.

2. x4_Supermarket Type3:
This indicates outlets categorized as Supermarket Type 3 (likely large or modern stores).
The strong positive coefficient suggests that sales are higher in these outlet types, possibly due to better visibility, larger customer bases, or wider product availability.

3. x2_OUT027:
This feature represents a specific outlet (OUT027).
Its high positive coefficient means that this outlet consistently performs better than others, likely due to location advantages, loyal customers, or better management practices.

#### Tree-Based Model Feature Importance

<img width="854" height="547" alt="RF - Importance" src="https://github.com/user-attachments/assets/0094cbc0-be7a-4346-a1e7-0a2a5b74e490" />

The 5 most important feature:

1. Item_MRP:
The price of the item (Maximum Retail Price) is the most critical factor influencing sales.
Higher-priced items are associated with higher predicted sales — the model gives this feature the greatest weight.
This means price remains the strongest predictor of demand.

2. x4_Grocery Store:
This feature shows whether the outlet is a grocery store.
Its strong importance suggests that outlet type significantly affects sales, grocery stores tend to have distinct sales patterns compared to supermarkets, possibly due to smaller size or product mix.

3. x2_OUT027:
This represents a specific outlet that consistently performs better than others.
Its importance indicates that store-level characteristics (like location or customer loyalty) strongly impact sales results.

4. x4_Supermarket Type3:
This represents larger or more modern supermarkets.
A positive contribution here suggests that Supermarket Type 3 stores achieve higher sales, likely due to better visibility, higher foot traffic, and broader product selection.

5. Outlet_Establishment_Year: 
This shows how long an outlet has been operating.
Its lower but still noticeable importance implies that older or more established outlets may have stable customer bases, slightly influencing sales performance.

### Recommendations:

### Limitations & Next Steps:

