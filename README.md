# 🏠 Airbnb Global Performance Dashboard — Power BI

An end-to-end Power BI dashboard project analyzing global Airbnb listing and review data across 10 major cities. Built with a focus on **real analytical thinking** — covering data modeling, DAX, Pareto analysis, seasonality, pricing strategy, and host trust insights.

> 📺 This project is explained step by step on the **[Mansi G. YouTube channel](https://www.youtube.com/@MansiG)**. Each decision is taught with the *why*, not just the *how*.

---

## 📥 Dataset

**Source:** [Maven Analytics Data Playground](https://mavenanalytics.io/data-playground/airbnb-listings-reviews)

Download the dataset from the link above and place it in the project folder before opening the `.pbix` file.

---

## 📊 Dashboard Overview

The dashboard spans **3 pages**, each focused on a distinct analytical theme:

### Page 1 — Growth & Listings Overview
Tracks the lifecycle of Airbnb's global expansion from 2008 to post-COVID, broken down by listing type (Entire Place, Private Room, Hotel Room, Shared Room).

**Key lifecycle phases annotated on the chart:**
- **Introduction** (pre-2010) — Slow take-off
- **Growth** (2010–2012) — Rapid expansion
- **Maturity** (2012–2015) — Peak new listings in 2015
- **Decline** (2016–2017) — Regulatory tightening; first profitable year in 2017
- **Reinvention** (2018–2019) — New growth wave, rise of hotel rooms
- **COVID-19** (2020) — Sharp contraction

### Page 2 — Market Share & Ratings
Pareto-style city breakdown showing listing concentration, Superhost share, average pricing by room type, and detailed rating scores across 5 dimensions.

### Page 3 — Seasonality, Review Frequency & Trust
Monthly review distribution by city, customer review frequency (Pareto), and host trust profile segmented by identity verification and profile photo status.

---

## 🔑 Key Metrics at a Glance

| Metric | Value |
|---|---|
| Total Listings | 2,79,712 |
| Cities Covered | 10 |
| Total Hosts | 1,82,024 |
| Property Types | 144 |
| Total Reviews | 5,373K |

---

## 💡 Key Insights

**Growth**
- Airbnb peaked in new listings in **2015**, then declined due to local regulatory pressure.
- Became profitable in the **second half of 2016**; 2017 was the first full profitable year.
- Hotel rooms saw a notable increase from **2018** during the reinvention phase.
- COVID-19 (2020) caused a sharp drop across all listing types.

**Market Share**
- **Paris, New York, and Sydney** together account for nearly half of all listings and **59% of total reviews** — a classic Pareto concentration.
- Paris leads all cities in both listings and reviews, partly driven by hotel room prices being **twice** the Airbnb equivalent.

**Pricing by Room Type**
| Room Type | Avg Price |
|---|---|
| Hotel Room | $800 |
| Entire Place | $673 |
| Shared Room | $580 |
| Private Room | $462 |

**Ratings**
- **Mexico City** and **Rio de Janeiro** are the top-rated cities overall.
- **Hong Kong** and **Istanbul** score the lowest.
- **Cleanliness** and **Value for Money** are the two dimensions with the lowest scores across cities universally.

**Seasonality**
- **Paris and Rome** dominate review activity from **April to August** (European summer peak).
- **New York** sees a review spike in **November–December** (holiday season).

**Review Frequency**
- **86.5%** of reviewers wrote only one review — typical of one-time or infrequent travelers.
- **98.8%** of all reviewers wrote 3 reviews or fewer.

**Host Trust**
- **66.9%** of hosts are fully verified with a profile photo — the most trustworthy segment.
- Only **0.3%** of hosts are completely unverified (no photo, no identity verification).
- Over two-thirds of all hosts carry at least one trust signal.

---

## 🎨 Design System

The dashboard uses a custom color palette consistent with Airbnb's brand identity:

| Color | Hex | Usage |
|---|---|---|
| Airbnb Red | `#FE585D` | Primary KPI cards, highlights, Superhost markers |
| Dark Grey | `#666666` | Secondary text, chart lines |
| Black | `#000000` | Body text, axis labels |
| Green | `#9DC656` | Section labels, positive indicators |
| Medium Grey | `#B3B3B3` | Background bars, non-Superhost segments |
| Light Grey | `#E6E6E6` | Card backgrounds, neutral fills |

**Custom visual assets used:** Airbnb logo, dashed rectangle card borders, magnifying glass icon (detailed ratings toggle), shield icon (trust visualization), star icon (overall rating).

---

## 🛠️ Tools & Techniques

| Tool / Concept | Application |
|---|---|
| **Power BI Desktop** | Dashboard design and report publishing |
| **DAX** | Custom KPI measures, cumulative %, running totals |
| **Power Query** | Data cleaning, type casting, relationship prep |
| **Data Modeling** | Star schema: Listings and Reviews fact tables |
| **Pareto Analysis** | City market share, reviewer frequency distribution |
| **Seasonality Analysis** | Monthly review % breakdown by city |
| **Pricing Analysis** | Average price comparison across room types |
| **Trust Analysis** | Host segmentation by verification and profile status |

---

## 📁 Project Structure

```
AirBnb_Global_Performance_Dashboard/
├── Airbnb.pbix                   # Power BI report file
├── README.md
└── assets/
    ├── air_bnb_logo.png          # Airbnb logo (used in dashboard header)
    ├── Color_Palette.png         # Project color palette reference
    ├── Dotted_Line_rectangle.png # Card border design element
    ├── Magnifying_glass.png      # Detailed rating toggle icon
    ├── SHIELD.PNG                # Trust visualization background
    └── Star.webp                 # Overall rating icon
```

---

## 🚀 Getting Started

1. **Download the dataset** from [Maven Analytics](https://mavenanalytics.io/data-playground/airbnb-listings-reviews).
2. **Clone or download** this repository.
3. Open **Power BI Desktop** and load the `.pbix` file.
4. In **Power Query**, update the data source path to point to your downloaded dataset files.
5. Click **Refresh** to load all data into the model.
6. Use the page navigation and slicers to explore the three dashboard pages interactively.

---

## 📺 Learn Along

This entire project is walked through step by step on the **Mansi G. YouTube channel** — covering not just the build, but the analytical reasoning behind every design and DAX decision.

---

*#PowerBI #DataAnalytics #AirbnbAnalysis #DAX #BusinessIntelligence #DataVisualization #ParetoAnalysis*
