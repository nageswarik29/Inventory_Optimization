# 📦 Inventory Optimization using ABC, Safety Stock & EOQ  

## 🔹 Project Overview  
This project analyzes inventory data (50 SKUs) to optimize supply chain decisions using **ABC Analysis, Safety Stock, Reorder Point (ROP), and Economic Order Quantity (EOQ)**.  

The goal is to identify high-value SKUs, reduce holding costs, and balance service level with cost efficiency — relevant for large-scale e-commerce operations like **Flipkart**.  

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
- **Safety Stock** ranged from **7 to 133 units** → varied by demand volatility & lead time.  
- **Top 10 SKUs** contributed **~44% of holding costs** → focus here maximizes savings.  
- **EOQ optimization** reduced replenishment frequency and lowered total cost.  

---

## 🛠️ Tools Used  
- **Excel** – Calculations, sorting, pivot tables  
- **Python (Pandas, NumPy, Matplotlib)** – Automation & visualizations  
- **Power BI / Tableau** (optional) – Dashboarding  

---

## 📌 Applications  
- Helps reduce **stockouts** while minimizing **holding costs**.  
- Useful for **e-commerce supply chains** where fast-moving SKUs require special attention.  

 

