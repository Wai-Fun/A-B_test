# **A/B testing case study: Does the new landing page improve conversion rate?**

## **Objective**

Evaluate whether a new landing page improves conversion rates for an e-commerce platform and determine if it should replace the existing page.

---

## **Dataset**

* ~300,000 users
* Randomly assigned to:

  * **Old landing page (control)**
  * **New landing page (treatment)**
* Key metric: **Conversion (0 = no, 1 = yes)**

---

## **Approach**

1. **Data Cleaning**

   * Removed mismatched group-page assignments
   * Verified no missing or duplicate data
   * Ensured each user saw only one page variant

2. **Exploratory Analysis**

   * Compared traffic distribution across pages
   * Visualized conversion counts and rates
   * Analyzed time spent on page

3. **Statistical Testing**

   * Conducted **two-proportion Z-test**
   * Calculated **confidence intervals (95%)**
   * Measured **effect size (difference in conversion rates)**

4. **Additional Analysis**

   * Logistic regression to evaluate impact of time on conversion

---

## **Key Results**

### **Conversion Rates**

* **New Page:** 11.88%
* **Old Page:** 12.04%
* **Difference:** **-0.16 percentage points**

### **Statistical Test**

* Z = -1.31
* p-value = 0.1897

👉 No statistically significant difference (p > 0.05)

### **Confidence Intervals**

* New Page: 11.71% – 12.05%
* Old Page: 11.87% – 12.21%

👉 Overlapping intervals confirm no meaningful difference

### **Effect Size**

* Extremely small (~0.16%)
* ≈ **1–2 fewer conversions per 1,000 users**

### **Time on Page**

* Logistic regression shows **no significant relationship** between time spent and conversion

---

## **Business Insight**

The new landing page performs **slightly worse**, but the difference is negligible and not statistically significant.

From a business perspective:

* No measurable improvement in conversions
* No meaningful revenue impact
* No justification for immediate rollout

---

## **Recommendation**

Do **not** implement the new landing page in its current form.

Instead:

* Continue testing **incremental design changes**
* Explore **user segmentation** (e.g., device, new vs returning users)
* Run follow-up experiments targeting specific improvements

---

## **Key Takeaway**

> The new landing page does not improve conversion rates. Both statistical and practical analysis show that its impact is negligible, highlighting the importance of data-driven decision-making before implementing product changes.

---

## **Tools & Technologies**

Python (Pandas, NumPy), Matplotlib, Seaborn, SciPy, Statsmodels
