# ⚡ EV Analytics & Automated Reporting System

An end-to-end EV market analytics and automated reporting pipeline built using n8n, Python, Google Sheets, QuickChart, Google Gemini and Gmail.

The project transforms raw electric vehicle data into meaningful KPIs, visualizations and AI-generated business insights, then automatically generates and delivers an HTML analytics report through Gmail.

---

## 📌 Project Overview

The objective of this project was to build an automated analytics workflow that reduces manual effort in data processing, analysis, visualization and reporting.

Instead of manually analyzing a spreadsheet and preparing a report, the workflow automates the complete process:

Google Sheets → Data Processing → KPI Analysis → Visualization → AI Analysis → HTML Report → Gmail

The project combines traditional data analytics with Generative AI and workflow automation.

---

## 🔄 Workflow Architecture

```text
                    ┌─────────────────────┐
                    │    Google Sheets    │
                    │      EV Dataset     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Python Processing │
                    │  Data Cleaning /    │
                    │   Transformation    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Python KPI        │
                    │      Analysis       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │      QuickChart     │
                    │   Data Visualization│
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Google Gemini    │
                    │ AI Executive        │
                    │ Summary Generation  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Python HTML       │
                    │   Report Generator  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       Gmail         │
                    │ Automated Delivery  │
                    └─────────────────────┘
