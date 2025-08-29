# 🧮 RFM Customer Segmentation

This project uses RFM analysis to group customers based on how recently they purchased (Recency), how often they buy (Frequency), and how much they spend (Monetary). It helps businesses understand customer behavior and target the right people.

---

## What I Did

1. **Loaded and cleaned the data**   
   - Checked for missing values and removed nulls  
   - Dropped duplicate records to ensure accuracy

2. **Calculated RFM metrics**  
   - Recency: Days since last purchase (scored from 5 to 1, where 1 = most recent)  
   - Frequency: Total number of purchases (scored from 1 to 5)  
   - Monetary: Total amount spent (scored from 1 to 5)

3. **Scored each customer**  
   Assigned scores from 1 to 5 for each metric.  
   *Note: Recency was reversed—customers with more recent purchases received lower scores (1 = most recent).*

4. **Created RFM segments**  
   Combined scores to group customers into categories like "Champions", "Loyal", or "At Risk".

5. **Visualized the results**  
- ![barplot](https://github.com/Esraa-MOhamed7/Customer-Segmentation-with-RFM-Analysis/blob/main/Total%20Revenue%20by%20Segment.png)
- ![pieplot](https://github.com/Esraa-MOhamed7/Customer-Segmentation-with-RFM-Analysis/blob/main/Top%203%20Segments%20by%20Count%20and%20Revenue.png)
- ![barplot](https://github.com/Esraa-MOhamed7/Customer-Segmentation-with-RFM-Analysis/blob/main/Customer%20Segment%20Distribution.png)

---

🙏 Thank you for exploring this project. I hope it helps you understand RFM segmentation and inspires your own data journey.
