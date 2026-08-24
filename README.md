# Google Play Store Apps Analysis

An interactive **Tableau** dashboard analyzing the Google Play Store app catalogue to understand what drives engagement, how apps are priced, how the catalogue breaks down by category and content rating, and which apps lead on reviews, ratings, and installs. Data was prepared and queried using **SQL**, with the final analysis delivered as a multi-view Tableau dashboard.

**🔗 Live dashboard:** [View on Tableau Public](https://public.tableau.com/app/profile/asfee.alam/viz/BA_16068210413190/Dashboardmain)

---

## Objective

To assess the composition, pricing, and engagement of apps on the Google Play Store — and to identify where user attention actually concentrates versus where app supply is highest. The goal was to turn a large, raw app dataset into a decision-ready view for anyone thinking about where to build, publish, or compete.

---

## Tools & Techniques

- **Tableau** - dashboard development, calculated fields, context filters, top-N filters, dual-axis charts
- **SQL** - data preparation, cleaning, and validation
- **Chart types used:** bubble chart, waterfall chart, pie chart, treemap, scatter plot, dual-axis line chart, context-filtered ranked tables
- **Excel** - source dataset (`googleplaystore.xlsx`)

---

## Key Insights

### 1. The market is overwhelmingly general-audience
Apps rated **"Everyone" account for 58.2% of all reviews**, followed by Teen (23.5%) and Everyone 10+ (14.2%). Mature 17+ apps draw just 4.1%, and Adults-only 18+ is effectively negligible. For a publisher, the reach is in broad, general-audience apps — niche age-restricted content sees a fraction of the engagement.

### 2. App supply and user engagement don't line up
By sheer **count**, the catalogue is dominated by **Family (1,972 apps)** and **Game (1,144 apps)** — together far ahead of every other category. But the highest *engagement* (reviews) comes from **Communication and Social** apps. This supply-vs-demand gap is the sharpest strategic signal in the data: the most crowded categories aren't the ones capturing the most attention.

### 3. Engagement is concentrated in a handful of giants
Filtering the top apps by review volume shows how top-heavy the market is:
- **Instagram** - 266.2M reviews (Social)
- **WhatsApp Messenger** - 207.3M reviews (Communication)
- **Messenger** - 169.9M reviews (Communication)
- **Subway Surfers** - 166.3M reviews (Game)
- **Facebook** - 156.3M reviews (Social)

A small set of communication and social platforms captures a hugely disproportionate share of total reviews.

### 4. Installs are dominated by Google's own apps
Among the **top free apps by installs**, the leaderboard is almost entirely Google-owned - **Google Photos, Google News, and Google Drive each at ~4 billion installs**, with Gmail, Google Play Games, and Chrome close behind. Pre-installed and first-party distribution is a decisive advantage at the very top of the install curve.

### 5. Top-rated apps skew toward games and learning
The highest-rated apps are led by **ROBLOX**, **CBS Sports**, and **Duolingo**, followed by 8 Ball Pool and Candy Crush Saga — a mix of gaming and habit-forming/learning apps that sustain strong ratings.

### 6. Pricing is cheap by default, with a novelty-driven tail
Most categories cluster at very low price points. The high-price tail is driven largely by **novelty "I am Rich"-style apps**, which command high average prices but attract **near-zero reviews** — high price, no real engagement. Genuine paid demand sits in categories like Finance, Family, and Medical rather than in the priciest listings.

---

## Dashboard Views

| View | What it shows |
|------|---------------|
| **Category of Apps based on Price** (bubble) | Relative pricing weight across categories, sized and shaded by review volume |
| **Average Reviews by Category** (waterfall) | How review volume accumulates across categories, Communication and Social leading |
| **Content Rating by Reviews** (pie) | Share of reviews by content-rating band |
| **Category Installed by Content Rating** (matrix) | Which categories are installed heavily within each content-rating band |
| **Top 10 Apps by Reviews** (context filter) | Highest-reviewed apps, ranked within category |
| **Top 10 Apps by Rating** (bar) | Highest-rated apps overall |
| **Top 50 Apps by Price and Reviews** (dual-axis line) | Price vs. review relationship across the priciest apps |
| **Number of Apps per Category** (ranked table) | Catalogue composition by app count |
| **Top Free Apps by Installs** (ranked table) | Highest-install free apps |

---

## Conclusion

The Play Store rewards **broad, general-audience apps**, and user attention is heavily concentrated in **Communication and Social** categories and a small number of dominant platforms — even though **Family and Game** apps flood the catalogue by count. Installs at the very top are shaped by first-party (Google) distribution, and pricing offers little engagement advantage. For a new entrant, the data argues for competing on engagement in high-attention categories rather than on volume in the most crowded ones.

---

## Repository Contents

- `googleplaystore.xlsx` — source dataset
- `Google Play Store report.pdf` — exported report
- `README.md` — this file

## Author

**Asfee Alam** — [GitHub](https://github.com/asfeealam) · [Tableau Public](https://public.tableau.com/app/profile/asfee.alam)
