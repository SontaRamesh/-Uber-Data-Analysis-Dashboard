# 🚖 Uber Data Analysis Dashboard
---

## 📌 Project Overview
The **Uber Data Analysis Dashboard** is built in **Power BI** to uncover deep insights from ride data — including **bookings, revenue, rider behavior, vehicle performance, and location trends**.  
It helps identify business patterns and improve operational efficiency through **interactive filters and dynamic KPIs**.

---

## 🎯 Objectives
- Analyze **completed vs lost bookings**  
- Track **monthly & quarterly revenue growth**  
- Compare **vehicle-wise performance** (distance, bookings, and revenue)  
- Identify **top customers**, **popular routes**, and **cancellation reasons**  
- Explore **rider behavior** and **busy time slots**  
- Assess **filter impact** on performance metrics (vehicle, time, area)

---

## 📊 Dashboard Pages

### 🟢 1️⃣ Overview Page

![Overview Page](Dashboard%20Files/overview-page.png)

---
- **KPIs:** Completed Bookings, Lost Bookings, Revenue, Total Distance, Avg Distance  
- **Monthly & Quarterly Analysis:** Bookings & Revenue trends  
- **Top Locations:** Pickup & Drop based on booking count  
- **Ratings:** Average Rider vs Driver Ratings  
- 🔍 *Filter added for Vehicle Type*

---

### 🚗 2️⃣ Vehicle Page

![vehicle-page](Dashboard%20Files/vehicle-page.png)

---
- Detailed metrics by vehicle type  
- **KPIs:** Booking Count, Revenue, Contribution (%)  
- 💡 *Auto* leads with highest distance, bookings, and earnings  

---

### 💰 3️⃣ Revenue Page

![revenue-page](Dashboard%20Files/revenue-page.png)

---
- Revenue by **Customer**, **Vehicle**, and **Payment Method**  
- Monthly and Quarterly revenue variations  
- **Top 10 high-value customers** identified  
- **UPI** emerged as the most preferred payment method  

---

### 🧍 4️⃣ Rider Page

![rider-page](Dashboard%20Files/rider-page.png)

---
- **Cancellation reasons** by type (Customer, Driver, Incomplete)  
- **Payment method impact** on ride cancellations  
- **Rider Segmentation:** First-time, Returning, Regular Riders  
- Monthly and Quarterly Rider Trends  

---

### 📍 5️⃣ Location Page

![location-page](Dashboard%20Files/location-page.png)

---
- **Monthly total distance** and **vehicle distribution**  
- **Busy time slots:** 3 PM – 6 PM and 6 PM – 9 PM  
- **Top areas:** Raj Nagar Extension, Munirka, Vaishali  
- Interactive filters for **Vehicle, Time, and Area**  

---

## 🧠 Key Insights
- 🚘 **Auto** dominates with **highest bookings (37K+)** and **revenue ₹1.28 Cr**  
- 💸 **Total Revenue:** ₹5.18 Cr across all rides  
- 📆 **Highest Revenue Month:** March (₹45.6L)  
- 💳 **Top Payment Mode:** UPI (₹2.33 Cr)  
- 📍 **Top Pickup:** Khandsa | **Top Drop:** Ashram  
- ⏰ **Peak Hours:** 6 PM – 9 PM  
- 🌍 **Total Distance:** 25,12,975.19 km  

---

## 📈 DAX Measures Used
```DAX
-- Total Revenue
Total Revenue = SUM('Uber Data'[Revenue])

-- Revenue %
Revenue % =
DIVIDE(
    SUM('Uber Data'[Revenue]),
    CALCULATE(SUM('Uber Data'[Revenue]), ALL('Uber Data'))
)

-- Average Distance
Avg Distance = AVERAGE('Uber Data'[Distance])

-- Completed Bookings
Completed Bookings =
CALCULATE(
    COUNTROWS('Uber Data'),
    'Uber Data'[Status] = "Completed"
)
```

---

## 🧰 Tools & Technologies

| 🧩 **Tool** | ⚙️ **Purpose** |
|--------------|----------------|
| **Power BI** | Data Cleaning, Modeling & Dashboard Creation |
| **DAX** | KPIs, Calculations, and Dynamic Measures |
| **Excel / CSV** | Data Source Preparation |

---

## 💼 Business Impact

This dashboard enables **Uber** to:

- 🚗 Identify **top-performing vehicles and regions**
- 💰 Optimize **resource allocation and pricing strategies**
- 🙋‍♂️ Understand **rider behavior and cancellation causes**
- 🌟 Enhance **customer satisfaction** through insights-driven decisions

---

## 👨‍💻 Author

**Sonta Ramesh**  
🎓 **B.Tech Graduate** | 📊 **Data Analyst** | 💡 **Power BI Developer**  
🏫 **IARE College**  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/sonta-ramesh/)

---

⭐ *If you found this dashboard insightful, please give it a ⭐ on GitHub!*
