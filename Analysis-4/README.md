# Policy-Focused Analysis: Real-World Electricity Challenges in Africa

This section focuses on policy and development-oriented questions related to Africa's electricity sector. For these analyses, the primary indicator used is renewable electricity generation (RE-generation), as it reflects the actual usable electricity produced—directly linked to electricity access.

## 1. Which African Countries Are on Track to Achieve UN SDG 7.1 (Universal Access to Electricity by 2030)?

A final table was created in the workbook showing:

- Each country's SDG assessment status
- A predicted 2030 electricity access percentage
- Categorization based on historical trends and future projections

### 🔢 What Method Was Used for Prediction?

At first, Excel's built-in Forecast Sheet was considered, but it was found to be too limited and more focused on visualization than flexible computation.

Instead, a manual linear regression model was built using:

- Slope
- Intercept
- Dynamic ranges for each country's 2000–2023 electricity access data

This approach ensures that each country's prediction is accurately based on its own historical trend.

### 📐 Formulas Used

#### 1. Dynamic Slope Calculation  
``=SLOPE(
OFFSET($E$1, MATCH($A25, $A:$A, 0)-1, 0, 24, 1),
OFFSET($D$1, MATCH($A25, $A:$A, 0)-1, 0, 24, 1)
)
``  
#### 2. Dynamic Intercept Calculation  
``=INTERCEPT(
OFFSET($E$1, MATCH($A2, $A:$A, 0)-1, 0, 24, 1),
OFFSET($D$1, MATCH($A2, $A:$A, 0)-1, 0, 24, 1)
)  
``  

**Explanation:**
OFFSET creates a dynamic range that automatically extracts the 24 rows (2000–2023) belonging to each country.
This allows SLOPE and INTERCEPT to be calculated automatically for every unique country without manually selecting ranges.

#### 3. Final Prediction Formula (2030 Access %)  
``=MIN(
INDEX($E:$E, MATCH($A2, $A:$A, 0) + 23) +
(F2 * (2030 - 2023)),
100
)
``  

This formula takes the country's most recent electricity access value (2023) and extends it forward using the calculated slope (annual improvement rate).
It projects the value to 2030 using:

- Years forward: (2030 − 2023)
- Slope: F2
- Cap at 100%: Because electricity access cannot exceed 100%

It is a simple linear trend projection representing where each country is heading if current progress continues unchanged.

### 📌 Conclusion

While many African countries appear on track to reach universal access by 2030, the continent overall is not. A substantial number of countries—representing hundreds of millions of people—remain far behind.

Achieving SDG 7.1 will require:

- Dramatically increased investment
- Stronger political commitment
- Focused support in Central, Eastern, and Western Africa, where progress remains the slowest

## 2. Which Countries Have High Renewable Potential but Low Electricity Access?

This analysis identifies countries with a large gap between:

- Renewable energy share (RE-share)
- Electricity access

### 📊 How Discrepancy Was Calculated

A country is labeled as High Discrepancy = 1 if: **RE-share − Electricity Access ≥ 40 percentage points**

Otherwise, it is assigned 0.

Countries with a high discrepancy were classified as "CRITICAL" in their status.

<img width="455" height="151" alt="Screenshot 2025-11-21 085215" src="https://github.com/user-attachments/assets/7d1d4a6a-2e97-448f-88a3-f256006211d4" />  


### 🧩 Conclusion: The Core Problem — The "Grid Gap"

The main issue uniting these countries is the Grid Gap:

- They generate large amounts of renewable electricity (often from hydropower).
- But their transmission and distribution networks are weak, old, or incomplete.
- As a result, the electricity does not reach most of the population, especially rural areas.

This creates a paradox:
A country may export renewable electricity while millions of its citizens remain unconnected.

### 🛠️ Solution Pathway

To solve this, countries must invest in a dual strategy:

1. **Expand and modernize the national grid**
   - To connect households to centralized renewable power.

2. **Accelerate off-grid renewable deployment**
   - Such as:
     - Solar home systems
     - Mini-grids
     - Community solar hybrid systems

These alternatives bypass costly grid infrastructure and bring electricity to remote communities much faster.
