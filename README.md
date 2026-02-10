# Stock Performance Overview — Power BI Project

## Project Description

This Power BI project analyzes stock performance, daily returns, and risk–liquidity characteristics of selected publicly traded companies over the period **2016–2026**.  
The goal is to present key financial indicators in a clear, interactive, and visually consistent dashboard, enabling easy comparison between companies from both performance and risk perspectives.

The report focuses on **exploratory analysis and visualization**, not prediction or forecasting.

---

## Dataset

The project is based on historical stock market data, including:

- Open, high, low, close prices  
- Trading volume  
- Company metadata  

Multiple tables are connected using Power BI relationships and transformed where necessary.

---

## Report Structure

The report consists of **three pages**, each focused on a different analytical angle.

---

### 📄 Page 1 — Price Over Time

**Purpose**  
To analyze long-term price development and overall performance trends.

**KPIs**
- Average Close Price  
- Price Change (%)  
- Average Daily Volume  
- Volatility (%)  

**Visuals**
- Line chart: *Average Closing Price Over Time by company*

**Interactivity**
- Company slicer  
- Year range slicer  
- Page navigation buttons  

**Key Question**
> Which stocks grew the most over time and how stable was their price behavior?

<img width="1052" height="692" alt="Snímek obrazovky 2026-02-10 050905" src="https://github.com/user-attachments/assets/732fdf12-1011-4ff3-bd8d-06edcfdbf9c8" />

---

### 📄 Page 2 — Daily Return Distribution

**Purpose**  
To evaluate short-term price movements and return consistency.

**KPIs**
- Average Daily Return (%)  
- Positive Days (%)  
- Best Day (%)  
- Worst Day (%)  

**Visuals**
- Daily return distribution chart using predefined return buckets  
  (e.g. −5% and below, −2% to 0%, 0% to +2%)

**Design Notes**
- Sorted return buckets for correct analytical order  
- Conditional coloring for best and worst outcomes  

**Key Question**
> How frequently do stocks generate positive returns and how extreme are daily movements?

<img width="1055" height="693" alt="Snímek obrazovky 2026-02-10 050849" src="https://github.com/user-attachments/assets/36203180-7bac-4b81-8881-ceb2dc587a07" />

---

### 📄 Page 3 — Risk & Liquidity

**Purpose**  
To compare companies based on risk exposure versus market liquidity.

**KPIs**
- Volatility (%)  
- Maximum Drawdown (%)  
- Average Daily Volume  
- Maximum Daily Loss (%)  

**Visuals**
- Bubble (scatter) chart:
  - X-axis: Average Daily Volume (liquidity)
  - Y-axis: Volatility (risk)
  - Bubble size: Relative trading activity
  - Color: Company

**Key Question**
> Which stocks are riskier, which are more liquid, and how do they compare at a glance?

<img width="1071" height="708" alt="Snímek obrazovky 2026-02-10 050923" src="https://github.com/user-attachments/assets/6e054e24-391a-4f6c-8a98-a1b2498dbc1a" />

---

## DAX Measures & Calculations

The report uses multiple custom DAX measures, including:

- Average Close Price  
- Price Change (%)  
- Average Daily Return (%)  
- Volatility (%)  
- Maximum Drawdown (%)  
- Maximum Daily Loss (%)  

Calculated columns are used for:

- Daily return computation  
- Return bucket categorization  
- Sorting logic for distributions  

---

## Design & UX Principles

- Consistent dark theme across all pages  
- Color-coded KPIs (green = positive, red = risk/loss)  
- Clear visual hierarchy and spacing  
- Interactive slicers and page navigation  
- Focus on readability and business interpretation  

## Summary

This Power BI report provides a structured overview of stock performance, volatility, and liquidity by combining long-term trends with short-term behavior and risk analysis.  
The project emphasizes clarity, interactivity, and analytical relevance, making it suitable for both business users and technical evaluation.
