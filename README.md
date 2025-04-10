# Scalable Sales Data ETL Pipeline on AWS ☁️

This project demonstrates a production-ready ETL pipeline built on AWS for processing large-scale sales data. It features scalable data ingestion, transformation, and warehousing using modern cloud components.

## ⚙️ Architecture Components

- **Data Source:** Structured Sales Data (CSV)
- **Staging Layer:** Amazon S3
- **ETL Jobs:** AWS Glue (Triggered via AWS Step Functions)
- **Schema Management:** AWS Glue Data Catalog
- **Data Warehouse:** Amazon Redshift
- **Monitoring & Logging:** AWS CloudWatch (Logs + Metrics)

<p align="center">
  <img src="path-to-diagram" alt="Architecture Diagram" width="600"/>
</p>

---

## 📐 Data Model

### Dimension Tables:
- Customer
- Product
- Sales Territory
- Currency
- Date
- Employee

### Fact Tables:
- Internet Sales
- Reseller Sales

---

## 🔄 ETL Pipeline Flow

1. **Ingest:** Upload raw sales CSV data to Amazon S3
2. **Clean & Transform:** Use AWS Glue jobs for data cleansing, aggregation, and schema mapping
3. **Load:** Push transformed data into Amazon Redshift
4. **Orchestrate:** Schedule and manage with AWS Step Functions
5. **Monitor:** Track job health and performance via AWS CloudWatch

---

## 🏗️ 3-Tier Data Architecture

- **Staging Layer:** Raw data in S3
- **Integration Layer:** Transformed fact and dimension tables in Redshift
- **Reporting Layer:** Optimized Redshift views for analytics consumption

---

## 💡 Highlights

- Reduced manual ETL by 90% using serverless Glue jobs
- Improved data availability from 24 hours to near real-time processing
- Enabled centralized schema governance with Glue Catalog
