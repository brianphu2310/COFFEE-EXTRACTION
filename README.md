<img width="856" height="688" alt="image" src="https://github.com/user-attachments/assets/30262200-4397-4a9c-8353-005b268d3675" />
<img width="3191" height="2373" alt="image" src="https://github.com/user-attachments/assets/5ce288c0-a1cb-4548-a335-2cf69bed0973" />


# COFFEE-EXTRACTION
Analysis of 13 coffee brewing methods + Recommender Engine
# ☕ Coffee Brewing Methods Analysis + Recommender Engine

## 📌 Project Overview

This project analyzes **13 coffee brewing methods** based on scientific data and builds an **interactive recommender engine** to help users find their perfect brewing method.

### 🎯 Key Questions Answered

- Which brewing method has the highest caffeine?
- What is the relationship between brewing time and caffeine?
- Which method is healthiest (highest antioxidants)?
- How do acidity, bitterness, and body differ across methods?
- **Which brewing method is best for YOU based on your preferences?**

---

## 📊 Dataset

| Method | Time (min) | Caffeine (mg) | Antioxidant Rank | Acidity | Bitterness | Body |
|---|---|---|---|---|---|---|
| Ristretto | 0.37 | 127 | 4 | 5 | 8 | 9 |
| Espresso | 0.47 | 124 | 3 | 6 | 7 | 9 |
| AeroPress | 1.50 | 60 | 1 | 5 | 4 | 5 |
| Moka Pot | 4.00 | 548 | 3 | 4 | 6 | 8 |
| Pour Over | 4.50 | 173 | 2 | 8 | 3 | 4 |
| French Press | 4.50 | 186 | 3 | 4 | 6 | 8 |
| Cold Brew | 1080 | 560 | 2 | 2 | 2 | 6 |
| ... | ... | ... | ... | ... | ... | ... |

*13 brewing methods analyzed in total*

---

## 🔬 Key Insights

| Insight | Finding |
|---|---|
| **Highest Caffeine** | Cold Brew (560mg), Moka Pot (548mg) |
| **Fastest** | Ristretto (0.37 min), Espresso (0.47 min) |
| **Healthiest** | AeroPress (Antioxidant Rank #1) |
| **Most Acidic** | Pour Over (8/10) |
| **Most Bitter** | Ristretto, Lungo, Turkish (8/10) |
| **Fullest Body** | Ristretto, Espresso (9/10) |

### 💡 Surprising Discovery

> **Brewing time does NOT correlate with caffeine content!**
> - Espresso (28 seconds): 124mg caffeine
> - Cold Brew (18 hours): 560mg caffeine (only 4.5x more)

---

## 📈 Visualizations

### Caffeine Ranking
![Caffeine Ranking](caffeine_ranking.png)

### Time vs Caffeine (Log Scale)
![Time vs Caffeine](time_vs_caffeine.png)

### Correlation Heatmap
![Correlation Heatmap](correlation_heatmap.png)

### Taste Profile Comparison
![Taste Comparison](taste_comparison.png)

---

## 🎯 Coffee Recommender Engine

The **Recommender Engine** asks you 5 questions and recommends the top 3 brewing methods based on your preferences.

### How it works:

| Question | Options |
|---|---|
| ⏱️ Time available | Instant, Fast, Medium, Slow, Very Slow |
| 🎨 Taste preference | Very Bright, Bright, Balanced, Bold, Very Bold |
| 🎯 Goal | Max energy, Quick boost, All-day sipping, Healthy, Light |
| 💪 Body | Light, Medium, Full, Very Full |
| ⚡ Caffeine sensitivity | Very sensitive, Moderate, High tolerance |

### Scoring System

Each brewing method gets **1 point** for matching your preference in each category.
- **Maximum score = 5 points**
- Top 3 methods with highest scores are recommended

### Interactive Tableau Dashboard

👉 **[View Live Dashboard on Tableau Public](YOUR_TABLEAU_LINK_HERE)**

*Replace with your actual Tableau Public link*

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **Excel** | Data cleaning & storage |
| **Python (Google Colab)** | Data analysis & visualization (Matplotlib, Seaborn, Pandas) |
| **Tableau Public** | Interactive dashboard & recommender engine |

---

## 📁 Repository Structure
