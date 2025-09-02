# 📦 Inventory Optimization using ABC, Safety Stock & EOQ  

## 🔹 Project Overview  
This project focuses on optimizing inventory management for 50 SKUs using **Excel-based analysis**.  
The study applies **ABC Classification, Safety Stock, Reorder Point (ROP), and Economic Order Quantity (EOQ)** to balance service levels with cost efficiency.  

---

## 📂 Dataset  
The dataset contains 50 products with the following attributes:  

- Product ID & Name  
- Annual Demand  
- Unit Cost  
- Lead Time (days)  
- Std. Dev. of Daily Demand  

---

## ⚙️ Methodology  
1. **ABC Classification** – Based on Annual Value (Demand × Cost).  
   - A: Top 70% of value  
   - B: Next 20%  
   - C: Last 10%  
   
2. **Safety Stock (SS)**  
   - Formula: `SS = Z × σ × √LT`  
   - Z = 1.65 (95% service level)  

3. **Reorder Point (ROP)**  
   - Formula: `ROP = (Daily Demand × LT) + SS`  

4. **Economic Order Quantity (EOQ)**  
   - Formula: `EOQ = √((2 × Demand × Ordering Cost) ÷ (Unit Cost × Holding Rate))`  

5. **Annual Holding Cost**  
   - Formula: `(SS + EOQ/2) × (Unit Cost × Holding Rate)`  

---

## 📊 Key Insights  
- **Category A (18 SKUs)** contributed ~70% of annual value → tighter control needed.  
- **Safety Stock** ranged from **7 to 133 units** → varies by demand uncertainty and lead time.  
- **Top 10 SKUs** contributed **~44% of holding costs** → prioritizing these reduces cost significantly.  
- **EOQ optimization** indicated lower replenishment frequency → improved efficiency.  

---

## 🛠️ Tools Used  
- **Microsoft Excel**  
   - Formulas for ABC, SS, ROP, EOQ  
   - Sorting & filtering for ABC categories  
   - MIN/MAX functions for range analysis  
   - Charts for visualization  

---

## 📌 Applications  
- Prevents **stockouts** while minimizing **holding costs**.  
- Directly applicable in **e-commerce inventory planning** (e.g., Flipkart supply chain).  

