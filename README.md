# 🤖 AI Scraping Agent (Natural Language to Data)

## 📌 Overview
Project ini adalah AI-powered scraping system yang memungkinkan user melakukan scraping hanya dengan input bahasa natural.

Contoh:
"Tolong scrape plumber di New York"

Sistem akan memahami intent, memilih workflow yang sesuai, dan mengumpulkan data secara otomatis.

## 🚨 Problem
- Scraping biasanya butuh setup manual
- Tidak fleksibel untuk berbagai sumber data
- Membutuhkan skill teknis

## 💡 Solution
Membangun AI agent berbasis n8n yang mampu:
- Memahami perintah bahasa natural
- Memilih workflow scraping yang sesuai
- Mengambil data dari Google Maps
- Menyimpan hasil ke Google Sheets / Excel
  
## ⚙️ Tech Stack
- n8n
- AI Agent (LLM-based intent detection)
- Apify (Google Maps API)
- Google Sheets

## 🔍 Key Features
- Natural language input
- Dynamic workflow selection
- Automated data extraction
- Structured output

## 📊 Impact
- Mempercepat riset data secara signifikan
- Menghilangkan kebutuhan setup manual
- Bisa scraping ratusan data dalam sekali input

## ⚠️ Limitations
- Bergantung pada API pihak ketiga
- Biaya usage (Apify & AI)
- Source masih terbatas
- 
## 📄 Documentation
See full documentation in AI_Scraping_Agent.pdf

## 🧠 Workflow Architecture

```mermaid
flowchart TD
    A[User Input] --> B[AI Agent]
    B --> C{Intent Detection}

    C -->|Google Maps| D[Scraping Workflow]
    D --> E[API Request]
    E --> F[Data Extraction]

    F --> G[Format Data]
    G --> H[Store to Google Sheets]
