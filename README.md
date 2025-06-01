# IPL-Data-Engineering-and-Analytics-Dashboard 📊🏏

An interactive Tableau dashboard offering in-depth analysis of Indian Premier League (IPL) team and player statistics across all seasons, powered by a full-stack data engineering pipeline built on AWS.

## 🔗 Live Dashboard
[View Interactive Dashboard on Tableau Public](https://public.tableau.com/app/profile/vivek.sai.chinna.burada/viz/indivivdual/Story1?publish=yes)

## 📋 Project Overview

This dashboard presents a comprehensive analysis of IPL data through two main analytical stories:

### Story 1: Team Analytics 🏟️
- **Interactive Stadium Map**: Visualizes all IPL venues across India
- **Home Team Performance**: Analyzes runs scored by home teams against opponents
- **Toss Analysis**: Examines toss win frequency and batting/bowling preferences
- **Overall Team Wins**: Displays team performance across all IPL seasons

### Story 2: Player Analytics 👤
- **Individual Performance**: Tracks player statistics across seasons
- **Seasonal Trends**: Shows performance evolution over time
- **Boundary Analysis**: Analyzes hitting patterns and boundary frequency
- **Strike Rate Metrics**: Displays batting efficiency and balls faced

## ✨ Key Features

### Interactive Filters
- **Team Selection**: Multi-select checkbox for filtering specific teams
- **Stadium Selection**: Interactive map highlighting for venue-specific analysis
- **Player Selection**: Individual player filtering for detailed analysis
- **Season Selection**: Temporal filtering for specific IPL seasons

### Dynamic Visualizations
- Real-time updates based on filter selections
- Contextual statistics for selected teams/players/venues
- Comparative analysis across different parameters

## 🛠️ Data Engineering Story

### **From Raw Data to Insights: My Data Pipeline**

When I started this project, I faced the challenge of working with a massive, messy IPL dataset spanning all seasons and multiple sources. Here’s how I engineered a scalable, cloud-based pipeline to power the dashboard:

#### **1. Data Collection & Storage**
- Gathered raw IPL match and player data from various sources in different formats (CSV, JSON).
- Stored all raw files securely on **Amazon S3**, making them easy to manage and scale.

#### **2. Data Cleaning with PySpark**
- Used **PySpark** to clean and preprocess the data:
  - Standardized team and player names.
  - Filled missing values and removed duplicates.
  - Created new columns (e.g., match type, decade) for richer analysis.

#### **3. Data Transformation with AWS Glue**
- Automated the ETL (Extract, Transform, Load) process using **AWS Glue**.
- Partitioned data by season and venue for faster queries.
- Normalized and structured the data for analytics.

#### **4. Data Quality Assurance**
- Implemented checks for missing values, schema consistency, and outlier detection.
- Ensured the data was always up-to-date and accurate.

#### **5. Dashboard Connection**
- Connected **Tableau** directly to the processed data in S3 using **Amazon Athena**.
- Enabled real-time, interactive analytics with minimal operational overhead.

**Result:**  
This pipeline transformed a huge, unstructured dataset into a clean, query-optimized analytics layer. It not only powers deep insights in the dashboard but also demonstrates my hands-on skills in cloud data engineering and big data processing.

---

## 💡 Why This Pipeline? (Athena/Glue vs. Redshift)

- **Athena + Glue** is ideal for flexible, serverless, and cost-effective analytics on S3 data. It requires no infrastructure management and is perfect for dashboards and ad-hoc queries.
- **Redshift** is better for ultra-fast, complex analytics on massive, structured datasets and for production-grade BI at scale. It requires more setup and is best for consistent, high-volume workloads.

**For this project, Athena + Glue offers the perfect balance of scalability, flexibility, and cost-efficiency.** If the data or user base grows significantly, or if advanced analytics are needed, migrating to Redshift or EMR is a future option.

---

## 🖼️ Dashboard Screenshots

### Team Analytics (Story 1)
![Team Overview](screenshots/story1/overview.png)

**Venue Distribution**
![Venue Map](screenshots/story1/venue_map.png)

**Performance Metrics**
![Home Runs Analysis](screenshots/story1/home_runs_chart.png)
![Toss Decisions](screenshots/story1/toss_decisions.png)

### Player Analytics (Story 2)
![Player Overview](screenshots/story2/player_overview.png)

**Performance Trends**
![Seasonal Performance](screenshots/story2/seasonal_performance.png)
![Boundaries Analysis](screenshots/story2/boundaries_chart.png)

## 🎯 Use Cases

### Team Management
- Evaluate home advantage statistics
- Analyze toss decision strategies
- Compare team performance across venues

### Player Scouting
- Track individual player progression
- Identify consistent performers
- Analyze batting patterns and strike rates

### Cricket Analytics
- Venue-specific performance insights
- Historical trend analysis
- Performance prediction modeling

## 🛠️ Technical Specifications

- **Platform**: Tableau Desktop/Public
- **Data Sources**: IPL historical data (2008-2023)
- **Visualizations**: Interactive maps, bar charts, pie charts, heatmaps
- **Interactivity**: Multi-level filtering and cross-filtering

## 📊 Data Insights

### Key Metrics Analyzed
- **Team Performance**: Runs scored, wins/losses, home advantage
- **Player Statistics**: Runs, innings, boundaries, strike rate
- **Venue Analysis**: Stadium-specific performance patterns
- **Toss Impact**: Decision trends and success rates

## 🔧 How to Use

1. **Access Dashboard**: Click the Tableau Public link above
2. **Navigate Stories**: Use story navigation tabs to switch between team and player analytics
3. **Apply Filters**: Select teams, players, or venues using interactive controls
4. **Explore Data**: Hover over visualizations for detailed tooltips
5. **Compare Metrics**: Use multi-select options for comparative analysis

## 📁 Repository Contents

- `/dashboard/`: Contains the Tableau workbook file (.twbx)
- `/screenshots/`: Dashboard screenshots organized by story
- `/data/`: Data source documentation
- `/docs/`: Additional documentation and user guides

## 🚀 Future Enhancements

- [ ] Real-time data integration
- [ ] Predictive analytics models
- [ ] Mobile-responsive design
- [ ] Advanced statistical metrics
- [ ] Player comparison tools

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues, feature requests, or pull requests.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

**Vivek Sai Chinna Burada**
- Tableau Public: [Profile Link](https://public.tableau.com/app/profile/vivek.sai.chinna.burada)
- GitHub: [Your GitHub Profile]

## 🏷️ Tags

`tableau` `ipl` `cricket-analytics` `data-visualization` `sports-analytics` `dashboard` `business-intelligence`

---
⭐ Star this repository if you found it helpful!
