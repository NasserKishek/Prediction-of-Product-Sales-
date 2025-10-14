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

### Model

### Recommendations:

### Limitations & Next Steps:

