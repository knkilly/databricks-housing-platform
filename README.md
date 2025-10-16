# Housing Analytics Platform

> A comprehensive data analytics platform for the housing market, built with Trino and Databricks Unity Catalog using medallion architecture (Bronze → Silver → Gold).

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![Trino](https://img.shields.io/badge/Trino-435-purple.svg)](https://trino.io/)

## 🏘️ Overview

This project provides end-to-end analytics for housing market, including:
- **200,000+** property transactions from Land Registry (2020-2025)
- Real-time property listings integration
- Market trend analysis by postcode sector
- Price index calculations
- Investment scoring system

## 🏗️ Architecture

```
Bronze Layer (Raw Data)
    ↓
Silver Layer (Cleaned & Standardized)'
    ↓
Gold Layer (Analytics & Aggregates)
```

**Technology Stack:**
- **Query Engine**: Trino 435
- **Data Catalog**: Databricks Unity Catalog
- **Storage Format**: Delta Lake
- **Programming**: Python 3.9+, SQL
- **Orchestration**: Docker Compose

## 📊 Data Sources

- **HM Land Registry** - Price Paid Data (public)
- **ONS Postcode Directory** - Geographic reference data
- **Property Listings** - Rightmove/Zoopla (via API/scraping)

## 🚀 Quick Start

### Prerequisites

- Docker Desktop (with WSL2 on Windows)
- Python 3.9+
- Databricks workspace with Unity Catalog
- 16GB RAM recommended

### Installation

1. **Clone the repository**
```bash
   git clone https://github.com/knkilly/databricks-housing-platform.git
   cd databricks-housing-platform
```

## 📁 Proposed Project Structure

```
databricks-housing-platform/
├── README.md                   # This file
├── LICENSE                     # MIT License
└── .gitignore                  # Git ignore rules
```

## 🎯 Current Status

- [ ] Infrastructure setup (Trino + Databricks)
- [ ] Bronze layer implementation
- [ ] Land Registry data ingestion (2020-2025)
- [ ] Silver layer transformations
- [ ] Gold layer schema design
- [ ] Property listings integration
- [ ] Gold layer analytics implementation
- [ ] Dashboard/API development
- [ ] Automated pipeline orchestration

## 🗓️ Planned Roadmap

### Phase 1: Foundation (Weeks 1-4) ✅

- Set up Trino and Databricks
- Implement Bronze → Silver → Gold layers
- Load historical transaction data

### Phase 2: Enrichment (Weeks 5-6)

- Add property listings data
- Integrate geographic data
- Build valuation models

### Phase 3: Analytics (Weeks 7-8)

- Create price indices
- Develop investment scoring
- Build interactive dashboards

### Phase 4: Automation (Future)

- Scheduled data updates
- Real-time alerts
- API development

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

- **Author**: Keerthi Killy
- **GitHub**: [@knkilly](https://github.com/knkilly)
- **LinkedIn**: [Keerthi Killy ](https://uk.linkedin.com/in/keerthi-killy)

---

**⭐ If you find this project useful, please give it a star!**