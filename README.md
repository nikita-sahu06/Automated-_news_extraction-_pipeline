# Automated-_news_extraction-_pipeline
Automated accident news parsing pipeline using n8n, Google Gemini LLM, and Microsoft Excel.
An end to end automated built with  automated data engineering pipeline built with **n8n**, **Google Gemini LLM**, **NewsAPI**, and **OneDrive Excel**.

## 📌 Project Overview
This pipeline automatically fetches real-time accident news every hour, passes unstructured news headlines to Gemini AI for entity extraction, cleans the JSON output using regex, and logs structured data into a cloud-hosted Microsoft Excel sheet for future data analysis.

## 🛠️ Tech Stack
* **Orchestration:** n8n
* **LLM Engine:** Google Gemini API
* **Data Source:** NewsAPI
* **Storage:** Microsoft Excel (OneDrive)

## 📊 Extracted Data Schema
The pipeline extracts and maps the following fields:
- `date`
- `headline`
- `url`
- `city_state`
- `vehicle_type`
- `dead_count`
- `injured_count`
- `incident_time`

## 🚀 How to Use / Import
1. Download the `workflow.json` file from this repository.
2. Open your **n8n instance** and click **Import from File**.
3. Re-configure your credentials:
 - NewsAPI Key
 - Google Gemini API Key
 - Microsoft OneDrive / Excel Account OAuth
4. Activate the schedule trigger!

