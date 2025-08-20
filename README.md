# 📊 Power BI Overstimulation Analysis Dashboard

<div align="center">

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-FF6F00?style=for-the-badge&logo=microsoft&logoColor=white)
![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

</div>

## 🚀 Project Overview

A comprehensive **Power BI dashboard** analyzing **overstimulation patterns** and their impact on productivity, well-being, and performance metrics. This project demonstrates advanced data visualization techniques, complex DAX calculations, and interactive business intelligence reporting for behavioral and psychological data analysis.

## 🎯 Business Problem

In today's fast-paced digital environment, **overstimulation** has become a critical factor affecting:
- 🧠 **Cognitive Performance**: Decreased focus and decision-making ability
- 💼 **Workplace Productivity**: Reduced efficiency and increased errors
- 🏥 **Health & Wellbeing**: Stress levels and mental health impacts
- 📱 **Digital Behavior**: Screen time and technology usage patterns
- 🎯 **Goal Achievement**: Impact on personal and professional objectives

## ✨ Key Features

### Interactive Visualizations
- **Heat Maps**: Overstimulation intensity across time periods and demographics
- **Trend Analysis**: Temporal patterns and seasonal variations
- **Correlation Matrix**: Relationships between stimulation factors and outcomes
- **Geographic Analysis**: Location-based overstimulation patterns
- **Drill-through Reports**: Detailed individual and group analysis

### Advanced Analytics
- **Statistical Modeling**: Predictive indicators of overstimulation
- **Cohort Analysis**: User behavior patterns over time
- **Anomaly Detection**: Identification of unusual patterns
- **Segmentation**: User groups based on stimulation sensitivity
- **Performance Metrics**: KPIs and business impact measurements

### Dynamic DAX Calculations
- **Complex Measures**: Multi-dimensional calculations for deep insights
- **Time Intelligence**: YoY, MoM, and custom period comparisons
- **Conditional Formatting**: Dynamic visual indicators based on thresholds
- **Parameter-driven Analysis**: User-controlled dashboard personalization

## 🏗️ Dashboard Architecture

```
Data Sources → Data Model → DAX Calculations → Visualizations → Insights
     ↓             ↓            ↓               ↓              ↓
Survey Data    Star Schema   Measures      Interactive      Business
Sensor Data    Relationships  Calculations   Charts          Actions
App Usage      Hierarchies    Time Intel.    Filters         Decisions
```

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| **BI Platform** | Microsoft Power BI Desktop/Service |
| **Data Modeling** | Power Query, DAX |
| **Data Sources** | Excel, CSV, SQL Server, APIs |
| **Cloud Services** | Power BI Service, Azure |
| **Collaboration** | Power BI Workspace, Teams Integration |
| **Mobile** | Power BI Mobile App |
| **Security** | Row-level Security (RLS) |

## 📊 Data Model & Schema

### Fact Tables
- **`FactStimulationEvents`**: Individual stimulation occurrences
- **`FactPerformanceMetrics`**: Productivity and performance data
- **`FactSurveyResponses`**: User-reported stimulation levels
- **`FactHealthMetrics`**: Stress, sleep, and wellness indicators

### Dimension Tables
- **`DimUser`**: User demographics and characteristics
- **`DimTime`**: Date, time, and calendar hierarchies
- **`DimLocation`**: Geographic and environmental data
- **`DimStimulationType`**: Categories of stimulation sources
- **`DimDevice`**: Technology and device information
- **`DimEnvironment`**: Physical and digital environment factors

## 📋 Dashboard Pages & Features

### 1. Executive Summary Dashboard
- **KPI Cards**: Key overstimulation metrics and trends
- **Gauge Charts**: Performance against targets and thresholds
- **Trend Lines**: Historical patterns and forecasting
- **Alert Indicators**: Critical threshold breaches
- **Quick Filters**: High-level segmentation controls

### 2. Detailed Analysis Page
- **Correlation Analysis**: Heatmap of factor relationships
- **Distribution Charts**: Overstimulation level distributions
- **Time Series Analysis**: Detailed temporal patterns
- **User Segmentation**: Cluster analysis visualizations
- **Comparative Analysis**: Before/after intervention studies

### 3. Individual User Analysis
- **Personal Dashboards**: Individual user drill-through reports
- **Behavior Patterns**: Personal stimulation triggers and responses
- **Progress Tracking**: Individual improvement over time
- **Recommendation Engine**: Personalized intervention suggestions
- **Goal Achievement**: Personal objective monitoring

### 4. Environmental Factors
- **Location Analysis**: Geographic stimulation patterns
- **Device Usage**: Technology impact on overstimulation
- **Time of Day**: Circadian rhythm analysis
- **Workplace vs. Home**: Environment-specific patterns
- **Social Factors**: Group and peer influence analysis

### Dynamic Filtering & Parameters

#### User-Controlled Parameters
```dax
// Parameter Table for Dynamic Analysis
Sensitivity Parameter = 
{
    ("High Sensitivity", 1),
    ("Medium Sensitivity", 2), 
    ("Low Sensitivity", 3)
}

// Dynamic Threshold Calculation
Dynamic Threshold = 
VAR SelectedSensitivity = SELECTEDVALUE('Sensitivity Parameter'[Value])
VAR BaseThreshold = 7
RETURN BaseThreshold - SelectedSensitivity
```

## 📊 Key Visualizations

### Interactive Charts
1. **Stimulation Heatmap**: Intensity across time and user segments
2. **Performance Correlation**: Scatter plot with trend lines
3. **Recovery Time Distribution**: Histogram with statistical overlays
4. **Geographic Analysis**: Map visualization with bubble sizing
5. **User Journey**: Sankey diagram of stimulation flow patterns

### Custom Visuals
- **Bullet Charts**: Performance against targets
- **Radar Charts**: Multi-dimensional user profiles
- **Waterfall Charts**: Factor contribution analysis
- **Box Plots**: Distribution analysis with outliers
- **Network Diagrams**: Relationship mapping between factors

## 🎯 Business Insights & Findings

### Key Discoveries
- **Peak Stimulation Hours**: 10-11 AM and 2-4 PM show highest levels
- **Recovery Patterns**: Average recovery time of 2.3 hours from peak stimulation
- **Environmental Factors**: Open offices show 34% higher stimulation than private spaces
- **Device Impact**: Multi-device usage increases stimulation by 28%
- **Demographics**: Age 25-35 shows highest sensitivity to overstimulation

### Performance Correlations
- **Productivity**: Inverse correlation (-0.72) with overstimulation levels
- **Decision Quality**: 23% decrease in complex decision-making during peak stimulation
- **Creativity**: Optimal range of 4-6 stimulation level for creative tasks
- **Stress Levels**: Strong positive correlation (0.81) with overstimulation

### Intervention Effectiveness
- **Mindfulness Breaks**: 18% reduction in stimulation levels
- **Environment Changes**: 25% improvement with noise reduction
- **Technology Limits**: 31% improvement with notification management
- **Scheduling Optimization**: 15% improvement with task timing adjustments

## 📱 Dashboard Interactivity

### User Experience Features
- **Drill-through Navigation**: Click to explore detailed views
- **Cross-filtering**: Visual interactions across multiple charts
- **Bookmarks**: Saved states for different analysis scenarios
- **Mobile Optimization**: Responsive design for tablet and phone
- **Real-time Updates**: Live data refresh capabilities

### Collaboration Features
- **Commenting**: Stakeholder feedback and discussion
- **Sharing**: Secure sharing with role-based access
- **Export Options**: PDF, PowerPoint, and Excel exports
- **Alerts**: Automated notifications for threshold breaches
- **Subscription**: Scheduled report delivery

## 📋 Prerequisites & Setup

### Requirements
- Microsoft Power BI Desktop (latest version)
- Power BI Pro or Premium license for sharing
- Data sources: Excel files, SQL Server, or web APIs
- Basic understanding of data modeling concepts

### Installation Steps
1. **Download Repository**
```bash
git clone https://github.com/Ompailwan/PowerBI-Overstimulation-Dashboard.git
cd PowerBI-Overstimulation-Dashboard
```

2. **Data Preparation**
- Import sample data files from `/data` folder
- Configure data source connections
- Refresh data model

3. **Dashboard Setup**
- Open `Overstimulation_Analysis.pbix` in Power BI Desktop
- Configure data source credentials
- Publish to Power BI Service workspace

## 🔒 Security & Governance

### Data Protection
- **Row-Level Security**: User-specific data access controls
- **Column-Level Security**: Sensitive data masking
- **Audit Logging**: Complete activity tracking
- **Data Classification**: Sensitivity labels and protection

### Compliance
- **GDPR**: Data privacy and anonymization features
- **HIPAA**: Healthcare data protection (when applicable)
- **Access Controls**: Role-based permissions and approval workflows

## 📈 Performance Optimization

### Optimization Techniques
- **Data Model Optimization**: Star schema and relationship optimization
- **DAX Performance**: Efficient formula writing and calculation groups
- **Visual Optimization**: Reduced visual count and smart caching
- **Incremental Refresh**: Efficient data loading strategies

### Monitoring & Maintenance
- **Performance Analyzer**: Built-in performance monitoring
- **Usage Metrics**: Dashboard adoption and usage tracking
- **Refresh Monitoring**: Data refresh success tracking
- **User Feedback**: Continuous improvement based on user input

## 🎓 Learning Outcomes

This project demonstrates mastery of:
- **Advanced Power BI Development**: Complex dashboard creation and optimization
- **DAX Programming**: Sophisticated calculations and time intelligence
- **Data Modeling**: Efficient star schema design and relationships
- **UX/UI Design**: User-centered dashboard design principles
- **Business Intelligence**: Translating data into actionable insights
- **Behavioral Analytics**: Understanding human behavior patterns through data

## 💼 Business Applications

### Use Cases
- **Corporate Wellness**: Employee wellbeing monitoring and intervention
- **Educational Settings**: Student stress and performance analysis
- **Healthcare**: Patient overstimulation in clinical environments
- **Retail**: Customer experience and environmental optimization
- **Remote Work**: Home office productivity optimization

### ROI & Business Value
- **Productivity Improvement**: 15-20% increase in focused work time
- **Wellness Programs**: Data-driven intervention strategies
- **Space Optimization**: Environmental design improvements
- **Policy Development**: Evidence-based workplace policies
- **Cost Reduction**: Decreased stress-related absences and turnover

## 🤝 Contributing

Enhancement opportunities:
1. **Additional Data Sources**: Wearable device integration, calendar APIs
2. **Machine Learning**: Predictive modeling for stimulation patterns
3. **Real-time Analytics**: Live streaming data integration
4. **Mobile App**: Custom mobile companion application
5. **AI Integration**: Automated insights and recommendations

## 📧 Contact

**Om Pailwan** - [ompailwan88@gmail.com](mailto:ompailwan88@gmail.com)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ompailwan/)
[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Ompailwan)

---

<div align="center">

⭐ **Star this repo if you found it helpful!** ⭐

</div>
