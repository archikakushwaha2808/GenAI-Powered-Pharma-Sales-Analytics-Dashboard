# GenAI-Powered Pharma Sales Analytics Dashboard



# 1. Executive Overview

The **GenAI-Powered Pharma Sales Analytics Dashboard** is an end-to-end business intelligence project that combines traditional data analytics with Generative AI to transform pharmaceutical sales data into actionable business insights.

The project analyzes historical pharmaceutical sales records to identify revenue drivers, evaluate product performance, detect seasonal demand patterns, and forecast future sales using time series forecasting techniques. In addition to conventional analytics, it integrates **Google Gemini AI** to generate executive summaries, answer business questions in natural language, and provide strategic recommendations based on the analyzed data.

This solution enables users to move beyond static dashboards by interacting with the analysis through an AI-powered business assistant capable of explaining trends, identifying risks, and suggesting data-driven decisions.

The project demonstrates a complete analytics workflow using **Python, SQL, Excel, Power BI, Prophet, and Google Gemini AI**, providing an intelligent decision-support system for pharmaceutical sales management.

### Business Objectives

- Analyze historical pharmaceutical sales performance.
- Identify top-performing and underperforming medicines.
- Discover seasonal and monthly sales patterns.
- Forecast future sales using Prophet.
- Generate AI-powered executive summaries and business insights.
- Enable natural language interaction through Google Gemini AI.
- Support inventory planning, marketing strategy, and business decision-making using data-driven recommendations.


# 2. Business Context

Pharmaceutical companies operate in highly regulated and demand-sensitive markets, where accurate sales analysis and demand forecasting are essential for efficient business operations. Even small forecasting errors can lead to:

- Overstocking, resulting in increased inventory holding costs.
- Stock-outs, leading to lost sales and reduced customer satisfaction.
- Expired inventory, causing direct financial losses.
- Inefficient resource allocation and reduced profitability.

To address these challenges, businesses require not only historical sales analysis but also intelligent decision-support systems that can explain trends and recommend actionable strategies.

This project combines traditional data analytics with **Generative AI** to provide a more interactive and business-friendly solution. Along with identifying revenue concentration, seasonal demand patterns, and product-level performance, the integrated **Google Gemini AI** helps generate executive summaries, answer business questions in natural language, and recommend data-driven strategies.

The insights generated through this project support:

- Revenue optimization
- Demand forecasting
- Inventory planning
- Marketing strategy
- Product performance evaluation
- Strategic resource allocation
- AI-assisted business decision-making


# 3. Dataset Overview

The project utilizes a pharmaceutical sales dataset containing historical transaction records across multiple medicine categories. The dataset serves as the foundation for exploratory data analysis, sales forecasting, and AI-driven business intelligence.

### Dataset Includes

- Drug Category (M01AB, M01AE, N02BA, N02BE)
- Sales Date
- Daily Sales Records
- Revenue Information
- Time-based Sales Trends

Each record represents the sales performance of a specific pharmaceutical product over a given time period, enabling detailed trend analysis and forecasting.



##  Analytical Capabilities

The dataset supports multiple levels of business analysis, including:

- Time Series Analysis
- Exploratory Data Analysis (EDA)
- Product Performance Comparison
- Sales Trend Identification
- Revenue Contribution Analysis
- Statistical Analysis
- Future Sales Forecasting using Prophet



## Generative AI Utilization

After completing the analytical workflow, the processed insights are provided to **Google Gemini AI**, enabling users to interact with the analysis using natural language.

Instead of manually interpreting dashboards and charts, users can ask business-oriented questions such as:

- Which medicine generates the highest revenue?
- Which product requires additional marketing?
- What are the major business risks?
- What inventory strategy should the company follow?
- Summarize the overall sales performance.

The AI generates executive summaries, business insights, strategic recommendations, and decision-support reports based on the analyzed pharmaceutical sales data.


#  4. Data Preparation & Feature Engineering

High-quality data preparation is a crucial step in any analytics project. Before performing exploratory analysis, forecasting, and AI-driven insight generation, the pharmaceutical sales dataset was carefully cleaned, transformed, and engineered to ensure accuracy and consistency.



##  Data Cleaning

The following preprocessing steps were performed:

- Handled missing values and inconsistent records.
- Checked for duplicate entries.
- Standardized date formats for time-series analysis.
- Converted data into appropriate numerical and datetime formats.
- Verified data consistency across all medicine categories.

These preprocessing steps improved the quality and reliability of subsequent analyses.



##  Feature Engineering

To enhance analytical capabilities, several new features were derived from the original dataset:

- Extracted **Year** from transaction dates.
- Extracted **Month** for monthly trend analysis.
- Aggregated sales at:
  - Daily level
  - Monthly level
  - Yearly level
  - Medicine category level

These engineered features enabled deeper temporal analysis and more meaningful business insights.



## Analytical Preparation

The transformed dataset was prepared for multiple analytical tasks, including:

- Exploratory Data Analysis (EDA)
- Sales Trend Analysis
- Statistical Analysis
- Product Performance Evaluation
- Time Series Forecasting using Prophet
- AI-powered Business Insight Generation



## Preparing Data for Generative AI

The processed analytical results were summarized into structured business context before being passed to **Google Gemini AI**.

Instead of sending raw transactional records, the AI receives key analytical insights such as:

- Total sales by medicine
- Average sales performance
- Best-performing products
- Underperforming products
- Sales trends
- Forecast summaries
- Business observations

This approach enables the AI to generate:

- Executive summaries
- Business recommendations
- Strategic insights
- Natural language answers to business questions

Using structured analytical outputs instead of raw data improves the quality, relevance, and reliability of AI-generated responses.



#  5. Revenue & Trend Analysis



##  5.1 Overall Revenue Growth Trend

![Yearly Sales Trend](yearly_drug_sales_trend.png)

### Analysis:

The yearly revenue trend demonstrates a consistent upward trajectory across time periods.

Key observations:

- Revenue exhibits sustained long-term growth.
- No structural revenue collapse or stagnation detected.
- Growth stability suggests expanding market demand.

### Business Interpretation:

This pattern indicates healthy market positioning and stable product portfolio performance. The company appears to be scaling effectively.

From a strategic perspective:
- Investment expansion may be justified.
- Production planning can be scaled gradually.
- Growth momentum supports market confidence.



## 5.2 Revenue Concentration by Drug Category

![Top Categories](sales_contribution_by_drug_category.png)

### Analysis:

A small subset of drug categories contributes disproportionately to total revenue.

This distribution follows a Pareto-like pattern:
- ~20% of categories generate the majority of revenue.
- Remaining categories contribute marginally.

### Business Implication:

This insight enables:

- Focused marketing investment on high-performing categories
- Priority-based inventory management
- Strategic product positioning

High-contribution categories should be protected from stock-outs and prioritized in promotional planning.



##  5.3 Seasonal Demand Pattern

![Monthly Heatmap](monthwise_avg_sales_heatmap.png)

### Analysis:

The heatmap highlights recurring seasonal peaks and troughs.

- Certain months consistently outperform others.
- Demand patterns appear cyclical.
- Seasonal spikes may correlate with disease patterns or prescription cycles.

### Business Impact:

Seasonality enables proactive planning:

- Increase production before peak months.
- Optimize logistics scheduling.
- Avoid overproduction during low-demand periods.

Accurate seasonal awareness reduces inventory risk and improves operational efficiency.



## 5.4 Category Performance Over Time

![Category Performance Over Time](monthly_drug_sales_trend.png)

### Analysis:

Tracking individual drug categories over time reveals:

- Some categories demonstrate stable growth.
- Others show volatility.
- Certain categories may show plateau or decline.

### Strategic Insight:

This supports:

- Product lifecycle management
- Identifying emerging vs mature products
- Rationalizing underperforming SKUs
- Diversification strategy decisions

Categories with sustained upward trends may warrant further R&D or marketing focus.



# 6. Sales Forecast Projection

![Forecast](drug_sales_forecast.png)

### Forecast Model Overview:

A time-series forecasting model was developed based on historical sales trends.

The projection indicates:

- Continued revenue growth trajectory
- No abrupt structural decline predicted
- Stable seasonal components

### Business Application:

Forecasting supports:

- Quarterly revenue planning
- Procurement scheduling
- Working capital optimization
- Inventory planning alignment

Data-driven forecasting reduces uncertainty and improves strategic preparedness.



#  7. SQL-Based KPI Analysis

SQL was used to perform business-oriented KPI analysis by querying and aggregating pharmaceutical sales data efficiently.

The following key performance indicators (KPIs) were calculated:

- Total Revenue
- Product-wise Revenue
- Monthly Revenue
- Yearly Revenue
- Category-wise Sales Contribution
- Revenue Growth Rate
- Running Revenue Totals
- Top & Bottom Performing Medicines

These SQL queries enabled efficient business reporting and demonstrated the ability to perform scalable analytics directly at the database level, supporting enterprise-ready reporting and decision-making.


#  8. Power BI Dashboard Development

An interactive Power BI dashboard was developed to transform analytical findings into intuitive business visualizations.

The dashboard includes:

- Revenue Trend Analysis
- Product-wise Sales Performance
- Monthly Sales Analysis
- Category Contribution
- Seasonal Trends
- Forecast Visualization
- KPI Cards

Users can interactively:

- Filter data by medicine category
- Analyze monthly and yearly trends
- Compare product performance
- Monitor sales growth
- Explore forecasted business performance

Beyond visualization, the project integrates **Google Gemini AI**, allowing users to ask business questions in natural language and receive AI-generated summaries, strategic recommendations, and decision-support insights based on the analytical results.

This combination bridges the gap between traditional dashboards and AI-assisted business intelligence.



#  9. Generative AI Business Assistant

One of the key innovations of this project is the integration of **Google Gemini AI**, transforming a traditional analytics dashboard into an intelligent business assistant.

Instead of manually interpreting charts and reports, users can ask business questions in natural language.

Examples include:

- Which medicine should receive more marketing?
- Which product has the highest sales?
- Which medicine is underperforming?
- What inventory strategy would you recommend?
- Summarize the overall business performance.

The AI uses the analytical insights generated during the project to produce:

- Executive Summaries
- Business Insights
- Strategic Recommendations
- Risk Analysis
- Growth Opportunities
- Inventory Suggestions
- Decision Support Reports

This demonstrates the practical application of Generative AI in business analytics and decision support.


#  10. Strategic Business Insights

Based on exploratory analysis, forecasting, SQL queries, dashboard visualizations, and AI-generated insights, several important business observations were identified.

### Key Findings

- High-performing medicines contribute significantly to overall revenue.
- Sales exhibit seasonal demand patterns that can improve inventory planning.
- Forecasting indicates future demand trends that support proactive business planning.
- Product-level performance highlights opportunities for targeted marketing strategies.
- AI-generated recommendations assist business users in making faster, data-driven decisions.

These insights support:

- Revenue Optimization
- Inventory Planning
- Marketing Strategy
- Product Portfolio Management
- Business Decision-Making




#  11. Conclusion

The **GenAI-Powered Pharma Sales Analytics Dashboard** demonstrates the complete lifecycle of a modern data analytics project by combining data engineering, business analytics, forecasting, visualization, and Generative AI.

The project showcases practical skills in:

- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Statistical Analysis
- SQL-Based KPI Analysis
- Power BI Dashboard Development
- Time Series Forecasting (Prophet)
- Business Intelligence
- Google Gemini AI Integration
- Prompt Engineering
- AI-Powered Decision Support

By integrating Generative AI with traditional analytics, the project enables users to interact with business insights using natural language, making data-driven decision-making more accessible and efficient.

This project demonstrates the ability to bridge the gap between technical analytics and business strategy while leveraging modern AI technologies to enhance decision support.

