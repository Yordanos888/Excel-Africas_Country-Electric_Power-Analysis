## 📈 Trend & Time-Series Analysis

This section explores long-term patterns and answers key trend-based analytical questions using renewable energy and electricity access datasets.

---

### **1. Which Countries Made the Largest Improvement in Renewable Energy Between 2010–2024?**

For this analysis, I focused on **renewable energy installed capacity**, because it reflects: Infrastructure investment, Built assets  and Long-term commitment to clean energy. This makes it good indicator of **“improvement.”**  
The table can be found on the file workbook.

#### **Methodology**
- **Base Year:** 2010  
- **End Year:** 2024 (latest available year)  
- Calculated:
  - Absolute improvement (difference)  
  - **CAGR** (Compound Annual Growth Rate)  
  - Classification/status based on performance  
- Applied **conditional formatting icons** to highlight increases vs decreases

#### **Formulas Used**
- **Improvement:**  
=(end_year - base_year)

- **CAGR:**  
=(((end_year)/(base_year))^1/n)-1  ,     n = total years between the start and end of the whole year  
  *CAGR must be interpreted cautiously since it smooths volatility.*

- **Country Status Classification (Excel formula):**

```excel
=IF(AND(D5>=0.05,C5>=0.38),"Significant Transformers",
IF(AND(D5>=0.02,C5>=0.38),"Mature & Growing",
IF(C5>=0.38,"Mature High-RE",
IF(AND(D5>=0.05,C5<0.38),"Rapid Emerging",
IF(C5<0.15,"Early Stage","Moderate Progress")))))
```
# Analysis Summary: Renewable Energy Classification & Electricity Access Trends in Africa

## 1. Country Classification Framework

This classification system helps identify distinct patterns in renewable energy development:

### 🏆 **Strong Long-Term Performers**
Countries demonstrating consistent, sustained renewable energy growth and infrastructure development.

### 🌱 **High-RE Mature Systems**
Nations with established renewable energy infrastructure maintaining significant renewable shares in their energy mix.

### 🚀 **Rapidly Emerging Nations**
Countries showing accelerated renewable energy adoption and rapid growth trajectories.

### 📈 **Early Stage Developers**
Nations in the initial phases of renewable energy development with significant growth potential.

**Overall**, this classification clearly displays which countries improved, by how much, and their developmental category based on improvements, CAGR, and historical performance.

---

## 2. Electricity Access Improvement in Africa (2000-2023)

This analysis visualizes the progress of electricity access across five major African regions from 2000 to 2023.

### 📊 Methodology
- Classified all African countries into regional groups using external metadata
- Calculated average electricity access for each region per year
- Plotted the combined values on a single trend line chart

![Electricity Access Trend](https://github.com/user-attachments/assets/6bfc4499-9f88-4c98-80d1-8feb99bd8b38)

### 🔑 Key Findings

#### ⭐ **A "Two-Speed" Continent**

**High-Access Regions:**
- Northern and Southern Africa show consistently high levels of electricity access

**Fast Improvers:**
- Eastern Africa emerges as one of the most dynamic and rapidly improving regions

**Lagging Behind:**
- Central Africa remains significantly behind—forming an "electrification hotspot" requiring urgent policy attention

#### ⭐ **Convergence and Divergence Patterns**

**Eastern Africa → Converging**
- Slowly catching up with the continental average, signaling strong progress

**Central Africa → Diverging**
- The access gap is widening, indicating unequal development across the continent

---

## 🧾 Overall Conclusion

When combined with the renewable energy improvement analysis, this time-series analysis provides crucial context:

### 🌍 **Dual Progress Champions**
Many Eastern African countries (Kenya, Uganda, Ethiopia) are:
- Rapidly improving electricity access
- Maintaining high renewable energy shares
- Earning classifications like "Mature & Growing" or "Significant Transformers"

→ These countries are simultaneously expanding access while building a clean energy future.

### ⚠️ **Structural Challenges**
Central African countries with slow electrification progress often fall into categories such as:
- "Early Stage" development
- "Mature High-RE but Declining" performance

→ Indicating broader structural challenges in their energy systems.

### 📈 **Dual-Dimension Assessment**
These findings reveal how different African regions are evolving across two critical fronts:

1. **Electricity Access** (social progress)
2. **Renewable Energy Investment** (sustainability progress)

**The Reality:** Some regions are achieving both objectives, while others struggle with one or both dimensions—highlighting where targeted support and investment are most urgently needed.
