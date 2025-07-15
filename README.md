# 2024 US Presidential Election Social Media Analysis

This project analyzes three datasets related to the 2024 U.S. presidential election, covering Facebook Ads, Facebook Posts, and Twitter Posts. Each dataset is explored using **three different Python approaches**:
- Pure Python (no external libraries)
- Pandas
- Polars

---

## 📁 Files Structure

Each dataset (`fb_ads`, `fb_posts`, `tw_posts`) is analyzed using:

| Analysis Type | Files |
|---------------|-------|
| Pure Python | `*_pure_python.ipynb` |
| Pandas | `*_pandas.ipynb` |
| Polars | `*_polars.ipynb` |

---

## ▶️ How to Run

1. Open any `.ipynb` notebook using [Jupyter Notebook](https://jupyter.org/) or [Google Colab](https://colab.research.google.com/).
2. Ensure the corresponding CSV data file is present in the same directory (e.g., `2024_fb_ads_president_scored_anon.csv`).
3. Run all cells in the notebook to view:
   - Column summaries
   - Value counts for categorical fields
   - Grouped statistics (`page_id` / `page_id` + `ad_id`)

> ⚠️ **Note**: The pure Python versions may take longer to run due to lack of optimized libraries.

---

## 📊 Summary of Key Findings

### Facebook Ads
- **Estimated Spend** ranges significantly, with some ads spending upwards of thousands of dollars.
- Most ads target **specific regions** and **demographics**, with **Clear Call-To-Action (CTA)** trends.
- Grouped analysis shows **certain `page_id`s consistently spending higher**, often aligning with political advocacy.

### Facebook Posts
- Highly **repetitive bylines and publishers** across pages.
- Certain pages are hyperactive, with outliers in post counts.
- Common engagement types and advocacy/issue messages were categorized and their distribution studied.

### Twitter Posts
- Heavy usage of **hashtags and mentions**.
- Many tweets do not contain explicit political claims but still align with campaign strategy.
- Volume and engagement vary widely across `page_id`s, with spikes during significant political events.

---

## 💡 Interesting Insights

- **Cross-platform behavior**: Pages that advertise heavily on Facebook also post more often, suggesting strategic amplification.
- **Message types**: Ads with fundraising CTAs have **higher average spend and impressions**, revealing monetization goals.
- **Targeting**: Demographics and region data highlight **geo-targeted campaigning**, especially in battleground states.

---

## 🧠 Suggested Next Steps

- Integrate temporal analysis (e.g., daily/weekly post and ad trends).
- Perform sentiment analysis on `illuminating_scored_message` content.
- Build dashboards to allow researchers to filter by candidate, platform, or message type.
