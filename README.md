# 🌍 World Population & GDP Analysis — Interactive Power BI Dashboard

An end-to-end Data Analytics and Business Intelligence solution that explores global macroeconomic trends, population dynamics, healthcare metrics, trade activity, and economic stability across world nations.

---

## 📌 Executive Summary

This interactive multi-page dashboard translates complex socio-economic datasets into clear, actionable insights[cite: 2, 3, 4, 5]. Designed with an executive dark-themed interface, the report empowers policymakers, economists, and global business analysts to assess market potential, analyze trade imbalances, measure health outcome disparities, and evaluate national debt vulnerabilities.

---

## 📂 Dashboard Architecture & Pages

The dashboard is structured across 4 dedicated pages, offering both high-level macro overviews and granular thematic analysis:

### 1. 🏠 Landing & Navigation Page
* **Purpose:** Serves as the interactive portal for report navigation[cite: 2].
* **Key Visuals:** High-resolution dynamic header, structured navigation buttons leading to all major report sections, and thematic category icons.

### 2. 📊 Executive Overview
* **Purpose:** High-level comparative analysis of global wealth, population density, and trade.
* **KPI Cards:** Average GDP ($370.84bn), Average Life Expectancy (66.93 years), Total Population (6bn), Highest GDP Country (United States), and Lowest Inflation Country (Hong Kong).
* **Visual Highlights:**
  * **GDP vs. Per Capita Dual-Axis Chart:** Contrasts overall economic size against individual wealth standards across major economies.
  * **Geographic Population Map:** Interactive Azure map visualizing spatial demographic distributions.
  * **Ranked Global Summary Table:** Full dynamic breakdown of GDP, Imports, Exports, Life Expectancy, Real Growth Rates, and Country Ranks.

### 3. 🏥 Health & Education Metrics
* **Purpose:** Investigates the direct correlation between economic prosperity and public health outcomes.
* **Visual Highlights:**
  * **Birth Rate vs. Death Rate Comparison:** Stacked bar chart highlighting demographic natural growth and aging trends.
  * **Infant Mortality Rate:** Highlighting public health bottlenecks in developing and sub-Saharan African nations.
  * **GDP Per Capita vs. Life Expectancy Scatter Plot:** Demonstrates the non-linear relationship between wealth accumulation and longevity.
  * **Adult HIV/AIDS Prevalence Trends:** Detailed risk mapping across vulnerable regions.
  * **Analytical Insights Panel:** Embedded textual synthesis summarizing key disparities in public health and development levels.

### 4. 📈 Economic Performance & Trade Dynamics
* **Purpose:** In-depth evaluation of international trade balance, fiscal health, labor forces, and monetary stability.
* **Visual Highlights:**
  * **Exports, Imports & Industrial Growth Combo Chart:** Measures trade volume alongside industrial output velocity.
  * **External Debt Analysis:** Horizontal bar chart highlighting total external debt burdens across major economies (e.g., UK, USA, Italy).
  * **Inflation vs. Unemployment Scatter Plot:** Explores macro economic stability across development classifications (Developed, Middle Income, Low Income).
  * **Labor Force Distribution:** Donut chart breaking down global workforce participation, dominated by China and India.
  * **Strategic Recommendations:** Actionable guidance on FDI in emerging markets, public health aid, and fiscal stabilization.

---

## 📐 Data Architecture & DAX Measures

The project utilizes an explicitly defined **`Table Measure`** repository to manage dynamic calculations efficiently:

| Measure Name | Description / Business Purpose |
| :--- | :--- |
| **Average Birth Rate** | Calculates the arithmetic mean of birth rates per 1,000 population. |
| **Average Death Rate** | Computes baseline mortality rates across filtered countries. |
| **Average GDP** | Evaluates overall regional economic scale. |
| **Average Life Expectancy** | Tracks global longevity standards. |
| **Country GDP Rank** | Dynamic ranking measure prioritizing countries by total economic output. |
| **GDP Growth Index** | Evaluates real economic growth rate percentages. |
| **Highest GDP Country** | Identifies the top-performing economy dynamically. |
| **Lowest Inflation Country**| Isolates the country with the most stable price environment. |
| **Population Density** | Evaluates demographic concentration relative to geographic area. |
| **Total GDP** | Aggregates gross domestic product globally or by selected filters. |
| **Total Population** | Sums overall population figures. |
| **Trade Balance Index** | Evaluates net export vs. import margins across trading partners. |

---

## 🛠️ Data Pipeline & Transformation Workflow

1. **Extraction:** Imported global macroeconomic datasets covering over 30 socio-economic parameters.
2. **Data Cleansing & Transformation (Power Query):**
   * Handled missing and zero-value entries across health indicators.
   * Standardized currency formats, growth rate percentages, and demographic units.
   * Categorized countries into structural bins: *Development Level* (High Income / Developed, Middle Income, Low Income) and *GDP Category*.
3. **Data Modeling:** Applied a clean Star Schema data model separating dimensional metadata (Geographic, Economic Bins) from core numerical fact tables.
4. **UI/UX Design:** Implemented an executive dark-palette theme with high-contrast visual cues, custom tooltips, slice-and-dice interaction rules, and intuitive navigation bookmarks.

---

## 💡 Key Business Insights

* **Wealth Disparity:** While total GDP is concentrated in major powers (US, China), Per Capita GDP reveals a stark contrast, highlighting severe internal wealth distribution gaps in large emerging nations.
* **Healthcare Impact:** Life expectancy scales dramatically with GDP per capita up to ~$20k, after which gains plateau above 80 years.
* **Trade & Debt Exposure:** High external debt levels are predominant among developed nations with heavy global trade volume, whereas high inflation and high birth rates heavily cluster in low-income economies.

---

## 💻 How to Run This Project

1. Clone or download this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/world-population-gdp-powerbi-dashboard.git](https://github.com/YOUR_USERNAME/world-population-gdp-powerbi-dashboard.git)
