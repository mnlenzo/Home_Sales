# Home Sales Analysis with SparkSQL

### *How Home-Sales Trends Inform Product Demand for Consumer Home-Product Companies*

---

## **High-Level Overview**

Home sales are one of the strongest leading indicators of demand for **HVAC systems, appliances, renovation materials, home services, and smart-home products**. When someone buys a home, they enter a 6–12 month window of high purchase likelihood across multiple categories.

This project uses **PySpark + SparkSQL** to transform raw home-sales data into insights that help companies like **Trane Technologies, Home Depot, Lowe’s, Carrier, and PulteGroup** understand:

* Which types of homes drive the most downstream product demand
* How pricing shifts relate to customer spending power
* Which households are likely to upgrade HVAC systems or appliances
* When product demand will peak based on seasonal buying behavior

The analysis also demonstrates how distributed systems manage large datasets through **partitioning**, **temporary views**, and **caching**—patterns used daily by enterprise analytics teams.

---

##  **Key Insights with Outputs**

### **1. Four-bedroom homes sell around the $300K range — a prime segment for multi-system upgrades**

SparkSQL results show:

| Year     | Avg Price (4BR Homes) |
| -------- | --------------------- |
| **2019** | ~$300,264             |
| **2020** | ~$298,354             |
| **2021** | ~$301,819             |
| **2022** | ~$296,364             |

**Why it matters:**
These buyers typically invest early in:

* multi-zone HVAC installations
* premium appliance bundles
* higher-capacity water heaters
* attic/insulation upgrades

Stable price bands help forecasting teams size the opportunity.

---

### **2. Homes built between 2010–2017 have significantly higher values — and higher upgrade potential**

The Spark output shows that many homes built during this period average **$700K–$790K+**.

Examples:

* **2016 → ~$791K**
* **2015 → ~$775K**
* **2012–2014 → ~$740–$770K**

**Why it matters:**
Higher-value homes correlate with higher adoption of:

* premium HVAC systems
* smart thermostats and IAQ (indoor air quality) add-ons
* appliance packages
* whole-home upgrades

This is a high-margin audience perfect for targeted lifecycle marketing.

---

### **3. Caching significantly reduces compute time — essential for real-time dashboards**

Queries produced:

* **Uncached runtime:** ~0.69 seconds
* **Cached runtime:** ~0.55 seconds

Even on moderately sized datasets, caching improves responsiveness.
At enterprise scale, this means:

* Faster analytics dashboards
* Lower compute cost
* Better forecasting granularity

Companies with large SKU catalogs and seasonal volatility benefit heavily from this performance pattern.

---

## **Why This Matters to Consumer Home-Product Companies**

Home-product demand (HVAC, appliances, materials, smart home tech) is tightly linked to **home age**, **home size**, **sale price**, and **seasonality**.

This analysis gives teams the visibility to:

* Predict HVAC replacement cycles
* Time promotions to align with home-sales peaks
* Target high-value customers with bundled product offers
* Improve regional inventory planning
* Anticipate renovation budgets based on sale price segments

By leveraging SparkSQL, these insights can scale across millions of transactions, similar to enterprise customer datasets.

---

# **Recommendations for Further Exploration**

### **1. Build a predictive model linking home attributes → product demand**

Examples:

* Larger homes → dual-system HVAC demand
* Older homes → renovation and appliance replacement cycles
* Higher-priced homes → premium SKU preferences

Useful for: Product strategy, pricing, forecasting, and marketing.

---

### **2. Combine home-sale seasonality + SKU sales for promotion timing**

Identify which months produce:

* HVAC tune-ups and replacements
* Appliance bundle purchases
* DIY home-improvement surges
* Contractor bookings

Useful for: Merchandising, regional planning, and ad budgeting.

---

### **3. Create buyer segmentation models**

Segment customers by:

* Price tier
* Home size
* Construction year
* Regional market behavior

Useful for: CRM, loyalty, and personalized marketing.

---

### **4. Develop a real-time Spark pipeline for sales forecasting**

Continuously update predictions based on:

* Interest rate movements
* Inventory availability
* New construction activity

Useful for: Supply chain, workforce planning, and revenue management.
