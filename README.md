# 🎯 RFM Customer Segmentation — Automated AI Pipeline

> Can a single workflow analyze customers, send reports, fire alerts, and answer questions about the data — automatically?

This project takes RFM Analysis beyond a notebook. It connects **Data Analysis**, **AI Agents**, and **Automation** in one n8n workflow that serves real business decisions.

---

## ⚙️ How It Works — 2 Triggers

### 📁 File Trigger (Automated Analysis)

Activated when a CSV file is uploaded to **Google Drive**:

1. Validates the file type
2. Downloads and processes the data
3. Sends it to an AI model via API
4. Runs **RFM Analysis** and scores each customer
5. Stores results in **Google Sheets**
6. Sends an automatic **report to the Manager**
7. Fires a **Telegram Alert** if at-risk customers are detected

### 💬 Chat Trigger (Interactive Q&A)

A conversational AI agent that lets users ask questions about customer data in natural language — pulling answers directly from Google Sheets.

> *"How many at-risk customers do we have?"* → answered instantly from live data.

---

## RFM Scoring

| Metric | Description | Score Direction |
|---|---|---|
| **Recency** | Days since last purchase | 1 = most recent |
| **Frequency** | Total number of purchases | 5 = most frequent |
| **Monetary** | Total amount spent | 5 = highest spend |

Combined scores map each customer to a segment:

| Segment | Profile |
|---|---|
|  Champions | Recent, frequent, high spenders |
|  Loyal | Consistent buyers with solid value |
|  At Risk | Were active — going quiet |
|  Lost | Low across all three metrics |

---

## Tech Stack

| Layer | Tool |
|---|---|
| Workflow Automation | n8n |
| AI Model | Claude (Anthropic) via API |
| File Storage | Google Drive |
| Data Storage | Google Sheets |
| Alerts | Telegram |
| Analysis | Python / RFM Logic |

---

## Visualizations

- Bar chart — customer distribution per segment
  ![Alt text](https://github.com/Esraa-MOhamed7/Customer-Segmentation-with-RFM-Analysis/blob/main/Customer%20Segment%20Distribution.png)

- Pie chart — Top 3 segments share of total base
  ![Alt text](https://github.com/Esraa-MOhamed7/Customer-Segmentation-with-RFM-Analysis/blob/main/Top%203%20Segments%20by%20Count%20and%20Revenue.png)
- Bar chart — average monetary value per segment
  ![Alt text](https://github.com/Esraa-MOhamed7/Customer-Segmentation-with-RFM-Analysis/blob/main/Total%20Revenue%20by%20Segment.png)

---

## Links

- 💻 [Code & Workflow](https://github.com/Esraa-MOhamed7/Customer-Segmentation-with-RFM-Analysis)
- 📓 [Kaggle Notebook](https://www.kaggle.com/code/esraamoh7med/customer-segmentation-with-rfm-analysis)

---

## Note

This project was a hands-on experiment in combining Data Analysis, Machine Learning, Automation, and AI Agents in a single workflow — built to support real business decisions, not just demo outputs.

Feedback and suggestions are always welcome!
