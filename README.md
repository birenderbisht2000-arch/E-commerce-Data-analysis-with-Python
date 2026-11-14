# E-commerce-Data-analysis-with-Python
An exploratory data analysis (EDA) of 100,000 quick-commerce grocery orders across three Indian platforms — Blinkit ,
JioMart SwiggyInstamart — built with Python, pandas, NumPy and Matplotlib in a JupyterNotebook

The project looks at revenue, order counts, product-category performance, delivery speed and delays, customer satisfaction (service ratings) and high-value customers.

###  Project Overview--

Quick-commerce platforms compete on speed, reliability and customer experience. This project analyses a transactional dataset of 100,000 orders to understand:

How the three platforms compare on revenue and order volume
Which product categories drive the most sales
How delivery time and delays behave across platform and category
How satisfied customers are, using service ratings
Which customers spend the most

The entire analysis lives in a single notebook (E-commerce.ipynb) and is also exported as HTML (E-commerce.html) for quick viewing without running any code.

###  Business Questions & Insights

### 1. Which platform is winning?
**Insight:** None clearly. Revenue is ₹19.8M (SwiggyInstamart), ₹19.7M (Blinkit) and ₹19.6M (JioMart), each about a third of the ₹59.1M total. Order counts (33,449 / 33,424 / 33,127) and average order value (~₹590) are also nearly identical.

**Implication:** The ~1% gaps are too small to call a winner without statistical testing. Since basket size doesn't differ, platforms must compete on speed, reliability and experience.

### 2. What drives revenue?
**Insight:** Product category. Personal Care (29.4%) and Grocery (24.0%) together bring in over half of revenue, while Snacks contribute only 7.7%. Average order value is about ₹1,050 for Personal Care, ₹847 for Grocery and ₹273 for Snacks, and these averages are almost the same on every platform, so basket size depends on *what* is bought, not *where*.

**Implication:** Push high-ticket categories through promotions, bundles and homepage placement. Use low-ticket categories (Snacks, Fruits & Vegetables) as frequency drivers, with add-on or minimum-order offers.

### 3. How satisfied are customers?
**Insight:** Satisfaction is polarised. Only 46.5% of orders get a rating of 4 or more, the mean is 3.24 / 5, and the standard deviation is high (1.58). Sample feedback points to operational causes such as missing items, freshness and packaging, and several low-rated orders also requested refunds.

**Implication:** Rating gains are likely to come from fixing order accuracy, freshness and packaging, not from speed alone.

### 4. How reliable is delivery?
**Insight:** Average delivery time is ~29.5 minutes (range 5 to 76), and 13.7% of orders (13,672) were delayed. Delivery time is near-identical across platform and category pairs, so no platform has a clear speed edge.

**Implication:** About 1 in 7 delayed orders is a real service gap. The next step is to link delays to ratings and refunds to measure what each delay costs.

### 5. Who are the most valuable customers?
**Insight:** There are 9,000 unique customers; the most frequent placed 26 orders. Top spenders by category are all in Personal Care, at roughly ₹9,200 to ₹9,800 each.

**Implication:** A small group of repeat, high-spend customers can be targeted with loyalty rewards, early access or retention offers.

## Recommendations

| Priority | Action | Based on |
|----------|--------|----------|
| High | Reduce missing-item, freshness and packaging complaints | Polarised ratings and negative feedback |
| High | Investigate causes of the 13.7% delay rate | Delay count, 29.5 min average |
| Medium | Promote Personal Care and Grocery bundles | 53% of revenue, highest basket sizes |
| Medium | Add upsell triggers to Snacks and Fruits & Vegetables | Lowest basket values |
| Medium | Launch a loyalty program for repeat high spenders | Top customers by spend |
