## 🧩 Analytical & Comparative Analysis

This section focuses on answering deeper analytical and comparative questions by combining multiple datasets and using advanced Excel techniques such as Power Query, data validation, filtering, and custom visualizations.

---

### **1. Is There a Relationship Between Renewable Capacity and Electricity Access?**

To explore this question, I used Power Query extensively to:
- Clean and prepare the renewable energy and electricity access datasets  
- Merge them into one structured analytical table  
- Load the final dataset for visualization  

A **data validation input** was used to filter countries dynamically, allowing users to interact with the scatter plot.  
I initially attempted to use slicers but it was complex to implement it. Used data validation tool again, for validation input as it gave more control and simplicity.

![Africa-RE Electricity Access Scatter](https://github.com/user-attachments/assets/878da33f-3442-4807-8ea7-8bb73f39ee49)

#### 🔍 What Happened — Both Good and Bad

**The Bad:**  
The initial goal was to determine whether:  
> **“Countries with higher renewable capacity also have higher electricity access.”**

However, the results did **not** show a clear or consistent relationship across African countries.  
Instead, the scatter plot revealed **mixed behaviors**—meaning the relationship is complex and cannot be explained by a single trend.

**The Good:**  
While it didn’t confirm the expected relationship, the scatter plot uncovered several valuable insights:

- **Some Countries have high RE-share but low electricity access, RE-share being on top:**  
This tells that governments in these countries are prioritizing or succeding in building RE infrastructure even faster than it is solving the problem of universal electricity access.

- **Other countries shows high electricity access but very low RE-share:**  
  Especially in North Africa, countries rely heavily on **non-renewable** energy sources despite strong electricity access performance.

- **Some countries RE-share is decreasing while electricity access increases:**  
  This suggests a shift in energy mix—possibly prioritizing energy availability over green energy expansion.

🎉 **Why this is my favorite visualization:**  
It shows that data doesn’t always confirm expectations.  
Instead, it teaches that **real-world systems are complex**, and a single graph can reveal multiple stories depending on how you interpret it.

---

### **2. Does Income Group Classification Influence Electricity Access in Africa?**

Using metadata from the electricity access dataset, I assigned each African country to its official **World Bank income group**.  
Then, I visualized electricity access averages for each group.

<img width="1899" height="1014" alt="Income Group vs Electricity Access" src="https://github.com/user-attachments/assets/2f8185e4-d0ad-44ea-a848-28ad0ba4ec61" />

The chart clearly shows a **strong positive correlation** between national income level and electricity access.

### **Key Findings**

#### **1. High-Income Country — 95–100% Access**
- Near-universal electrification  
- Minimal gaps in infrastructure  

#### **2. Upper-Middle-Income Countries — 85–90% Access**
- Strong access but not fully universal  
- Rural and remote communities still lag  

#### **3. Lower-Middle-Income Countries — 65–75% Access**
- Large portions of the population remain unconnected  
- Infrastructure investments are improving but uneven  

#### **4. Low-Income Countries — 35–45% Access**
- Severe electricity poverty  
- Majority of the population lacks grid access  
- Major infrastructure and financial limitations  

👉 **Conclusion:**  
Income level is a major predictor of electricity access.  
Lower-income countries face systemic obstacles—financial, infrastructural, and logistical—that significantly slow down electrification.

---

### **3. Regional Analysis: Electricity Access by African Regions**

This table compares electricity access between two major African regions:
- **Middle East & North Africa (MENA)**
- **Sub-Saharan Africa (SSA)**

I computed the **average electricity access from 2000–2023** for each region and applied **conditional formatting** to highlight year-to-year patterns and differences.  

<img width="659" height="755" alt="Regional Electricity Access Table" src="https://github.com/user-attachments/assets/9abc909c-9451-4e6e-9b8d-4d1d2173ba57" />  

Middle East & North Africa (MENA) has maintained a high level of access, consistently above 82% and reaching nearly 88% by 2023.
Sub-Saharan Africa (SSA) started from a much lower base (28.2% in 2000) but has shown remarkable, steady growth.

While both regions have seen an improvement in electricity access over the past two decades, the situations are distinct. The Middle East & North Africa region is focused on maintaining and slightly improving its already high access rates. In contrast, Sub-Saharan Africa is in a phase of rapid catch-up, having made tremendous progress but still requiring substantial investment and development to achieve universal access.

---

## 🧾 Final Conclusion

These analytical visualizations highlight the key factors influencing electricity access in Africa:

- The **RE-share vs electricity access scatter plot** did not reveal a simple relationship, but instead uncovered deeper insights about national priorities, energy transitions, and infrastructure gaps.
- The **income group analysis** clearly demonstrated that higher-income countries achieve significantly better electricity access.
- The **regional comparison** confirmed that geographic and economic contexts strongly shape electrification outcomes.

Together, these analyses show that electricity access in Africa is shaped by **multiple interconnected factors**—economic strength, regional conditions, policy choices, and energy-source preferences. Real-world energy systems are complex, and understanding them requires looking beyond a single metric or trend.

---
