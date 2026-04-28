# melodybox-retention-analysis
 Analysis of declining new-user retention in a subscription music service."


> **TL;DR** : Retention dropped from ~77% to ~52% in February 2024. The cause wasn't a worse product- existing plans were retained at the same rate as before. The drop was entirely a composition shift: a new $0.99 / 7-day trial plan, primarily acquired through paid social, retains at just 10%. Critically, this 10% is uniform across channels, engagement, and auto-renew settings — meaning the trial offer itself is selecting for users who won't convert. Recommendation: Question the trial's economics before optimising it.

📄 **Full case study writeup:** [(https://www.notion.so/MelodyBox-Subscription-Retention-Analysis-350658b8997e81bf9e58e8a165bd6829?source=copy_link)]

---

## The problem

A subscription music service flagged that new-user retention had been declining for several months. Three questions to answer:

1. Is the trend real?
2. What's causing it?
3. What should the product team do?

---

## The approach

Cohort decomposition. Find the trend, validate it's real, then progressively segment to isolate the cause.

1. Define retention 
2. Build a cohort retention view
3. Validate for right-censoring and seasonality
4. Segment by plan, channel, engagement, auto-renew
5. Distinguish product quality issues from composition shifts
6. Recommend, prioritise, size

---

## Key findings

- Retention dropped from **~77% to ~52%** in February 2024 and stayed there.
- **Existing plans (monthly_standard, monthly_premium) stayed flat at ~77% throughout 2024.** The product didn't get worse.
- A new **trial_7day plan** launched February 2024 and retains at just **10.4%** roughly one-seventh the rate of paid plans.
- **70% of trial signups came through paid_social**, which roughly doubled in volume share at the same time.
- Trial retention is **uniform across channels (~9-13%), engagement levels (~7-12%), and auto-renew settings (10-13%)** -none of the typical optimisation levers move it.

---

## Recommendations

1. **Question the trial's unit economics** before optimising anything else. If trial CPA exceeds 10.4% × monthly_standard LTV, the trial is unprofitable.
2. If keeping the trial, **restructure the offer** (auto-renew default, longer window, or first-month discount)  not the experience. Engagement isn't the lever.
3. **Reframe what the trial is for.** It's currently judged on retention and failing but may be quietly succeeding on volume / CPA / brand awareness. Pick the right metric.

See full case study:  https://www.notion.so/MelodyBox-Subscription-Retention-Analysis-350658b8997e81bf9e58e8a165bd6829?source=copy_link

---
---
## Repo structure
## How to reproduce

```bash
git clone https://github.com/[your-username]/melodybox-retention-analysis.git
cd melodybox-retention-analysis
pip install pandas matplotlib jupyter
jupyter notebook notebooks/melodybox_retention.ipynb
```

---

## Tools used

Python (pandas, matplotlib) · Jupyter

---

## A note on the data

This is a **synthetic dataset** I generated to mirror realistic subscription patterns. It is not real data, and the company name "MelodyBox" is fictional. The analytical patterns and pitfalls are designed to reflect what a real product analyst would encounter.


---




