# Key Business Insights - Customer Churn Analysis

## 📊 Project Summary
- **Dataset**: 36,992 customer records from Hugging Face
- **Model Used**: Random Forest Classifier
- **Accuracy**: **92.69%**
- **Recall**: **94.43%** (Excellent at catching customers likely to churn)

---

## 🔍 Major Churn Drivers (Top Insights)

### 1. Membership Category
- Customers with **No Membership** or **Basic Membership** have the **highest churn risk**.
- Platinum and Gold members are significantly more loyal.
- **Recommendation**: Create special upgrade offers and loyalty benefits for low-tier members.

### 2. Points in Wallet
- Lower `points_in_wallet` strongly correlates with higher churn.
- Customers with fewer points feel less valued and tend to leave.
- **Recommendation**: Run targeted campaigns to boost points for low-point customers.

### 3. Customer Feedback
- Negative feedback categories such as:
  - Poor Customer Service
  - Poor Website
  - Too many ads
- These are **strong predictors** of churn.
- **Recommendation**: Prioritize improvements in customer service and user experience.

### 4. Engagement Level
- Higher `days_since_last_login` → Higher churn probability.
- Inactive customers are at much greater risk.
- **Recommendation**: Send re-engagement offers, discounts, or personalized emails to inactive users.

### 5. Other Important Factors
- `avg_transaction_value`
- `complaint_status`
- `past_complaint`

---

## 📈 Model Performance Highlights

| Metric       | Value     | Interpretation                     |
|--------------|-----------|------------------------------------|
| Accuracy     | 92.69%    | Overall correct predictions        |
| Precision    | 92.30%    | When model predicts churn, it's reliable |
| **Recall**   | **94.43%**| Very good at identifying actual churners |
| F1 Score     | 93.35%    | Strong balance between precision & recall |

**Confusion Matrix**:
[[3060  317]   ← 3060 Low-risk correctly predicted
[ 224 3798]]  ← 3798 High-risk correctly predicted


---

## 💡 Actionable Business Recommendations

1. **Retention Campaigns**: Focus on Basic/No Membership customers with personalized offers.
2. **Loyalty Program**: Improve rewards system to increase points in wallet.
3. **Service Improvement**: Address top complaints (Customer Service & Website).
4. **Early Warning System**: Use the model to flag high-risk customers for proactive intervention.
5. **Re-engagement Strategy**: Target customers inactive for more than 30 days.

---

## 🚀 Business Impact
Implementing these insights can help the company:
- Reduce customer churn significantly
- Increase customer lifetime value
- Improve overall revenue through better retention

---

**Prepared by**: Venkata Geetha lakshmi Gunda  
**Date**: June 2026