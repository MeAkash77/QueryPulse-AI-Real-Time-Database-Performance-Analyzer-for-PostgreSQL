# QueryPulse-AI-Real-Time-Database-Performance-Analyzer-for-PostgreSQL 🚀

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-14%2B-blue.svg)](https://www.postgresql.org/)
[![Version](https://img.shields.io/badge/version-0.1--beta-orange.svg)](https://github.com/yourusername/stonebraker/releases)

## ⚠️ Disclaimer

**This is a beta release (v0.1-beta) and NOT production-ready software. Use at your own risk.**
- This tool may suggest database changes that could impact performance
- Always test suggestions in a non-production environment first
- Back up your database before applying any changes

## Motivation 💭

Database performance optimization is a critical yet complex task that requires deep expertise in SQL, query planning, and system architecture. Many organizations struggle with:

- **Complex Query Analysis**: Identifying bottlenecks in large SQL queries
- **Schema Design Decisions**: Making optimal choices for indexes and constraints
- **Performance Testing**: Lack of automated tools for before/after comparisons
- **Risk Management**: Fear of making changes that might degrade performance
- **Knowledge Gap**: Limited access to database optimization experts

This project aims to democratize database optimization by combining the power of Large Language Models (LLMs) with automated testing and analysis tools, making expert-level optimization accessible to all developers.

## Project Description 📝

Stonebraker is an intelligent system that:

1. **Analyzes Database Schemas**: 
   - Automatically scans table structures
   - Identifies missing indexes
   - Suggests optimal data types
   - Recommends partitioning strategies

2. **Optimizes Queries**:
   - Rewrites complex queries for better performance
   - Suggests materialized views
   - Identifies common anti-patterns
   - Provides explain plan analysis

3. **Tests Performance**:
   - Runs automated benchmarks
   - Compares query execution times
   - Measures resource utilization
   - Generates detailed reports

4. **Ensures Safety**:
   - Provides rollback capabilities
   - Tests changes in isolation
   - Validates optimization impacts
   - Prevents destructive changes

The AI agent leverages state-of-the-art LLMs through Groq's high-performance API or local Ollama models, combining their analytical capabilities with practical database optimization techniques.

## 🎯 Introduction

Stonebraker is an intelligent system that combines LLM capabilities with database optimization techniques to help developers improve their PostgreSQL database performance. It analyzes schemas, suggests optimizations, and provides automated testing of changes.

### Key Features

- 🔍 Automated schema analysis and optimization suggestions
- 📊 Query performance testing and benchmarking
- 🛠️ LLM-powered query rewriting and improvement
- 📈 Before/After performance comparison
- 🔄 Safe rollback capabilities
- 🤖 AI-driven insights for better decision making

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/cloudraftio/stonebraker.git
cd stonebraker

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your credentials

# Start the application
streamlit run app.py
```

## 📋 Prerequisites

1. **Python Environment**
   - Python 3.8 or higher
   - pip package manager
   - virtualenv or venv

2. **PostgreSQL Setup**
   - PostgreSQL 14+ installed and running
   - Database user with appropriate permissions
   - Access to EXPLAIN ANALYZE privileges

3. **LLM Provider (choose one)**
   - Groq API account and API key
   - Ollama local setup with supported models

## 🔧 Installation Details

1. **Python Dependencies**
```bash
pip install -r requirements.txt
```

2. **Configuration**
   - Copy `.env.example` to `.env`
   - Configure database connection
   - Add LLM provider credentials

## 📖 Example Usage
![Web Interface](./docs/image/image.jpg)
*StonebrakerAI Dashboard*

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Check existing issues or create a new one
2. Fork the repository
3. Create a feature branch (`git checkout -b feature/amazing-feature`)
4. Commit your changes (`git commit -m 'Add amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

### Development Setup
```bash
# Install dev dependencies
pip install -r requirements.txt

# Run tests
python -m pytest
```

## 🗺️ Roadmap

### v0.1-beta (Current)
- [x] Basic schema analysis
- [x] Query optimization suggestions
- [x] Performance testing framework

## 🧹 Security & Maintenance

Before contributing or deploying:
1. Run `pre-commit run --all-files` to clean sensitive data
2. Check for credentials in git history
3. Verify no API tokens in code
4. Remove unnecessary files

## 📞 Contact & Support

- **Issues**: Use [GitHub Issue Tracker](https://github.com/cloudraftio/stonebraker/issues)

## 📄 License

The  is distributed under AGPL-3.0-only.







































QueryPulse-AI: Real-Time Database Performance Analyzer for PostgreSQL 🚀
https://img.shields.io/badge/License-AGPL%2520v3-blue.svg
https://img.shields.io/badge/python-3.8+-blue.svg
https://img.shields.io/badge/PostgreSQL-14%252B-blue.svg
https://img.shields.io/badge/Streamlit-1.28+-red.svg
https://img.shields.io/badge/version-1.0--beta-orange.svg

⚠️ Disclaimer
This is a beta release (v1.0-beta) and NOT production-ready software. Use at your own risk.

This tool may suggest database changes that could impact performance

Always test suggestions in a non-production environment first

Back up your database before applying any changes

The autonomous fix mode should be used with approval enabled initially

🌟 What's New in v1.0
Autonomous Fix Mode 🤖 - Auto-create indexes with approval workflow

Natural Language Debugging 💬 - Ask "Why is my DB slow?" in plain English

Predictive Alerting 🔔 - Detect performance degradation before outages

Multi-Database Support 🔄 - PostgreSQL, MySQL, MongoDB adapters

Beautiful Dashboard 📊 - Real-time performance visualizations

Index Usage Analytics 📈 - Track which indexes are actually being used

Smart Rollback ⏮️ - Automatic rollback if indexes hurt performance

Motivation 💭
Database performance optimization is a critical yet complex task that requires deep expertise in SQL, query planning, and system architecture. Many organizations struggle with:

Complex Query Analysis: Identifying bottlenecks in large SQL queries

Schema Design Decisions: Making optimal choices for indexes and constraints

Performance Testing: Lack of automated tools for before/after comparisons

Risk Management: Fear of making changes that might degrade performance

Knowledge Gap: Limited access to database optimization experts

Slow Detection: Finding issues only after they cause outages

This project aims to democratize database optimization by combining the power of Large Language Models (LLMs) with automated testing, predictive analytics, and intelligent alerting systems.

Project Description 📝
QueryPulse-AI is an intelligent, AI-powered database performance optimization system that:

1. 🔍 Analyzes Database Schemas
Automatically scans table structures and relationships

Identifies missing indexes using query statistics

Suggests optimal composite and partial indexes

Recommends partitioning strategies for large tables

Detects outdated statistics needing refresh

2. ⚡ Optimizes Queries
Rewrites complex queries for better performance

Suggests materialized views for expensive aggregations

Identifies common anti-patterns (SELECT *, N+1 queries)

Provides detailed EXPLAIN ANALYZE plan analysis

Compares before/after execution plans

3. 📊 Tests Performance
Runs automated benchmarks with timing measurements

Compares query execution times with statistical significance

Measures resource utilization (CPU, I/O, memory)

Generates detailed markdown reports

Validates improvements with rollback capability

4. 🤖 Autonomous Optimization
Auto-Fix Mode: Creates missing indexes with approval

Predictive Alerts: Detects growth trends and degradation

Natural Language Interface: Ask questions about performance

Smart Rollback: Reverts changes that don't improve performance

5. 🎯 Real-Time Monitoring
Live performance dashboards with Plotly visualizations

Active alert management with severity levels

Historical trend analysis

Index usage heatmaps

Slow query detection and ranking

6. 🔄 Multi-Database Support
PostgreSQL (primary)

MySQL (via adapter)

MongoDB (via adapter)

Extensible adapter pattern for new databases

🎯 Key Features
Core Features
🔍 Automated schema analysis and optimization suggestions

📊 Query performance testing and benchmarking

🛠️ LLM-powered query rewriting and improvement

📈 Before/After performance comparison

🔄 Safe rollback capabilities

🤖 AI-driven insights for better decision making

Advanced Features (v1.0)
🤖 Autonomous Fix Mode: Auto-create indexes with approval workflow

💬 Natural Language Debugging: "Why is my orders query slow?" - AI explains

🔔 Predictive Alerting: 24-hour advance warning of performance issues

📊 Beautiful Dashboard: Real-time charts, heatmaps, and metrics

🔄 Multi-DB Support: PostgreSQL, MySQL, MongoDB ready

📈 Index Analytics: Track usage, size, and effectiveness

⏮️ Smart Rollback: Automatic rollback if performance degrades

🚀 Quick Start
bash
# Clone the repository
git clone https://github.com/cloudraftio/stonebraker.git
cd stonebraker

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your credentials

# Start the application
streamlit run app.py
📋 Prerequisites
Python Environment

Python 3.8 or higher

pip package manager

virtualenv or venv

PostgreSQL Setup

PostgreSQL 14+ installed and running

Database user with ANALYZE and INDEX permissions

Access to pg_stat_statements extension

LLM Provider (choose one)

Groq API account and API key

Ollama local setup with supported models

Any OpenAI-compatible API

Optional for Advanced Features

MySQL: pip install pymysql

MongoDB: pip install pymongo

Plotly for dashboards: pip install plotly

🔧 Installation Details
Step 1: Clone and Setup
bash
git clone https://github.com/cloudraftio/stonebraker.git
cd stonebraker
python -m venv venv
Step 2: Install Dependencies
bash
pip install -r requirements.txt
Step 3: Configure Environment
bash
cp .env.example .env
Edit .env with your credentials:

env
# Database Configuration
DB_HOST=localhost
DB_PORT=5432
DB_USER=postgres
DB_PASSWORD=your_password
DB_NAME=your_database

# LLM Configuration (choose one)
LLM_PROVIDER=groq  # or ollama
GROQ_API_KEY=your_groq_api_key
OLLAMA_BASE_URL=http://localhost:11434
Step 4: Enable PostgreSQL Extensions
sql
CREATE EXTENSION IF NOT EXISTS pg_stat_statements;
CREATE EXTENSION IF NOT EXISTS pgstattuple;
📖 Usage Examples
1. Basic Optimization
python
# In the web interface
Request: "Analyze query performance for orders table and suggest indexes"
2. Natural Language Debugging
python
Request: "Why are my order reports getting slower every day?"
# AI analyzes trends and explains in plain English
3. Autonomous Fix Mode
python
# Enable in sidebar
- Toggle "Auto-Fix Mode"
- Set "Require Approval" for safety
- Click "Scan for Fixes"
4. Performance Dashboard
text
Navigate to "Performance" tab:
- View real-time query metrics
- See index usage heatmaps
- Track historical trends
- Get optimization recommendations
5. Predictive Alerts
text
Navigate to "Alerts" tab:
- Active alerts with severity levels
- Predictive warnings for:
  * Table growth trends
  * Query performance degradation
  * Index effectiveness decline
🏗️ Architecture
text
┌─────────────────────────────────────────────────────┐
│                   Streamlit UI                       │
│  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌──────────┐  │
│  │  Home   │ │Performance│ │ Alerts  │ │ Settings │  │
│  └─────────┘ └─────────┘ └─────────┘ └──────────┘  │
└─────────────────────────────────────────────────────┘
                           │
┌─────────────────────────────────────────────────────┐
│              Performer Graph (LangGraph)             │
│  ┌──────────────┐ ┌──────────────┐ ┌─────────────┐ │
│  │Analyze DB    │→│Human Loop    │→│SQL Executor │ │
│  └──────────────┘ └──────────────┘ └─────────────┘ │
└─────────────────────────────────────────────────────┘
                           │
┌─────────────────────────────────────────────────────┐
│                   Core Modules                       │
│  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌──────────┐ │
│  │SQL Agent│ │Auto Fixer│ │Alert Mgr│ │Dashboard │ │
│  └─────────┘ └─────────┘ └─────────┘ └──────────┘ │
└─────────────────────────────────────────────────────┘
                           │
┌─────────────────────────────────────────────────────┐
│              Database Adapters                       │
│  ┌──────────┐ ┌──────┐ ┌────────┐ ┌─────────┐     │
│  │PostgreSQL│ │MySQL │ │MongoDB │ │Custom   │     │
│  └──────────┘ └──────┘ └────────┘ └─────────┘     │
└─────────────────────────────────────────────────────┘
📊 Dashboard Features
Performance Metrics
Avg Query Time: Real-time query performance

Index Usage Percentage: How often indexes are used

Active Connections: Current database load

Cache Hit Ratio: Buffer cache effectiveness

Visualizations
Query Performance Trend: Line chart over time

Index Usage Heatmap: Color-coded index effectiveness

Slow Queries Table: Ranked by execution time

System Health: CPU, Memory, Disk metrics

Alert Types
🔴 Critical: Immediate action needed

🟡 Warning: Monitor and plan fixes

🔵 Info: Informational suggestions

🔮 Predictive: Future issue warnings

🤝 Contributing
We welcome contributions! Please follow these steps:

Check existing issues or create a new one

Fork the repository

Create a feature branch (git checkout -b feature/amazing-feature)

Commit your changes (git commit -m 'Add amazing feature')

Push to the branch (git push origin feature/amazing-feature)

Open a Pull Request

Development Setup
bash
# Install dev dependencies
pip install -r requirements-dev.txt

# Run tests
python -m pytest

# Run linting
flake8 .
black .

# Run pre-commit hooks
pre-commit run --all-files
🗺️ Roadmap
v1.0-beta (Current - Released)
Basic schema analysis

Query optimization suggestions

Performance testing framework

Autonomous fix mode

Natural language debugging

Predictive alerting

Multi-database support (PostgreSQL, MySQL, MongoDB)

Beautiful dashboard with visualizations

Index usage analytics

Smart rollback capability

v1.1 (Planned)
Automated query rewriting

Machine learning for trend prediction

Anomaly detection algorithms

Custom alert rules

Export reports (PDF, JSON)

Slack/Teams integration

v2.0 (Future)
Kubernetes operator for auto-scaling

Cross-database query optimization

Real-time replication monitoring

Cost-based optimization suggestions

Cloud provider integrations (AWS RDS, Azure, GCP)

🧪 Testing
bash
# Run all tests
pytest tests/

# Run specific test suite
pytest tests/test_performer.py

# Run with coverage
pytest --cov=. tests/

# Run performance benchmarks
python tests/benchmark.py
🔒 Security Best Practices
Before deploying:

Never commit .env file with real credentials

Use database users with minimal required privileges

Enable SSL for database connections

Run in approval mode initially, not autonomous

Regularly rotate API keys

Monitor audit logs for changes

📞 Contact & Support
Issues: GitHub Issue Tracker

Discussions: GitHub Discussions

Documentation: Wiki

🙏 Acknowledgments
PostgreSQL community for excellent documentation

LangChain for LangGraph framework

Groq for high-performance LLM inference

Streamlit for amazing UI framework

All open-source contributors

📄 License
This project is distributed under AGPL-3.0-only license.

See LICENSE file for more details.

⭐ Star History
If you find this useful, please star the repository! It helps others discover the project.

https://api.star-history.com/svg?repos=cloudraftio/stonebraker&type=Date

Built with ❤️ by the CloudRaft Team
