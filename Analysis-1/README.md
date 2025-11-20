## 📊 Descriptive Analytics

This section presents several descriptive analyses based primarily on the **renewable energy datasets**.  
The goal is to understand how electricity access and renewable capacity vary across African countries.

### 🔧 Excel Skills Used
- **Power Query** – for data cleaning, aggregation, and filtering  
- **FILTER Function** – to dynamically extract country-level indicators  
- **Charts** – bar charts, column charts, and interactive map visuals  

---

### **1. Countries With the Highest and Lowest Electricity Access**

A simple bar chart was used to display the **Top 10 countries with the highest** and **Top 10 with the lowest** electricity access rates.  
This helps highlight energy inequalities across the continent.

<img width="1015" height="300" alt="Screenshot 2025-11-20 135720" src="https://github.com/user-attachments/assets/d56eaa2e-2043-42d4-95da-88ec861b5a41" />  

---

### **2. Fastest Growth in Renewable Energy Since 2000**

For this analysis, I highlighted the **top 6 African countries** showing the most significant increase in renewable energy share (%) since 2000.  
A customized column chart was created to make the comparison clearer and visually appealing.

<img width="642" height="310" alt="Screenshot 2025-11-20 135816" src="https://github.com/user-attachments/assets/94efb185-cbe7-4f26-a371-30a63b5d32c8" />

**Indicator Used:**  
**RE-Share of Electricity Capacity**  
I selected this indicator because it directly measures infrastructure investment in renewable energy.  
It is also **less volatile** than generation data, which fluctuates due to weather variations and grid constraints.

---

### **3. Distribution of Renewable Energy Sources by Region (Solar, Hydro, Wind)**

This analysis examines how the major renewable sources are distributed across African countries.  
A regional map visualization was used to uncover patterns in solar, wind, and hydro capacity.

**Indicator Used:**  
**Electricity Installed Capacity (MW)**  
This was chosen for the same reason as earlier—it is stable and represents long-term investment.

![Africa-map-RE-visualisation](https://github.com/user-attachments/assets/51ed3c14-b4f0-47ec-b6ad-d0b08f6697dd)  

---

### 🛠️ Process Flow

1. Aggregated power values (MW) for all renewable technologies — **solar, wind, hydro, and others** — using Power Query.  
2. Created a filtered table that includes only *major renewable types* (solar, wind, hydro).  
3. Applied the **FILTER** function to dynamically return countries and values based on user-selected inputs from data validation.  
4. Built an interactive map visualization to display renewable capacity by country.

🎯 **Note:**  
The map displays only the **top 75% countries** in each renewable category.  
This helps focus the visualization on countries with meaningful data and improves readability.

---

