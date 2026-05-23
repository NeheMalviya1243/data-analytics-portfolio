# Nehe Malviya — Data Analytics Portfolio

> Business Data Analytics | Rider University (Graduating May 2026) | Lawrence Township, NJ

Welcome to my project portfolio. I build end-to-end data solutions — from raw data pipelines to interactive dashboards and business intelligence tools — using Python, SQL, and modern analytics frameworks.

---

## About Me

- **Degree:** B.S. Business Data Analytics — Rider University (May 2026)
- **Skills:** Python, SQL, Pandas, Streamlit, Plotly, Excel (Power Query, Pivot Tables), Tableau, R
- **Interests:** Business intelligence, automation, data storytelling, AI analytics tools
- **Seeking:** Data Analyst / Business Analyst roles (OPT eligible)

---

## Projects

### 01. Olympic Games Analytics Dashboard

**Tech Stack:** Python | Streamlit | Pandas | Plotly | Seaborn | Matplotlib

> An interactive web application for exploring 120+ years of Summer Olympic Games history across 134,000+ athlete records.

**What it does:**
- Medal Tally filtered by year and country (Gold / Silver / Bronze)
- Participation trends — nations, events, and athletes over time (1896–2016)
- Country-wise analysis with sport heatmaps and top athlete rankings
- Athlete-wise analysis — age distributions by medal type, Height vs. Weight scatter plots
- Men vs. Women participation trends over the full Olympic history

**Highlights:**
- Built a full ETL pipeline (`preprocessor.py`) — filters Summer Games, merges NOC region mappings, one-hot encodes medals
- Separated business logic (`helper.py`) from UI (`app.py`) following software engineering best practices
- Analyzed 134,000+ records across 35+ Olympic Games

**Repo:** [olympic-games-analytics-dashboard](https://github.com/NeheMalviya1243/olympic-games-analytics-dashboard)

---

### 02. GenAI KPI Meeting Assistant

**Tech Stack:** Python | Streamlit | Pandas | Plotly | Seaborn | Google Gemini API | FPDF | smtplib

> An AI-powered sales KPI dashboard that automates the entire weekly reporting workflow — from raw data upload to AI-generated summaries and email delivery.

**What it does:**
- Smart column auto-detection — handles messy, inconsistently named real-world datasets
- Computes Executive KPIs: Total Sales, Profit, Quantity, Avg Discount, Week-over-Week change
- Auto-selects Daily / Weekly / Monthly / Yearly trend granularity based on date range
- Region & Category analysis with bar charts, pie charts, and Seaborn profit heatmap
- Top 10 Selling Products bar chart
- AI-generated natural language KPI narrative via Google Gemini (`gemini-pro`)
- Generates formatted PDF report and emails it with chart attachments via Gmail SMTP

**Highlights:**
- End-to-end automation: CSV upload → KPIs → AI summary → PDF → Email in one app
- Integrated two AI backends: Google Gemini API and HuggingFace BART (`facebook/bart-large-cnn`)
- Handles real-world messy data with flexible column name mapping
- Production patterns: temp file handling, SMTP authentication, exception management

**Repo:** [genai-kpi-meeting-assistant](https://github.com/NeheMalviya1243/genai-kpi-meeting-assistant)

---

### 03. Breast Cancer Prediction

**Tech Stack:** Python | Flask | Scikit-learn (SVM) | Pandas | NumPy | HTML/Jinja2

> A machine learning web application that predicts whether a breast cancer tumor is Malignant or Benign — built with Python, SVM, and Flask.

**What it does:**
- Trains a Support Vector Machine on the Wisconsin Breast Cancer Dataset (569 records, 30 features)
- Achieves **98.2% accuracy** in classifying tumors as Malignant or Benign
- Flask web app lets doctors input 30 tumor measurements and get an instant prediction
- Supports dual input modes: individual form fields or space-separated bulk paste
- Returns prediction result, model accuracy, and processing runtime

**Highlights:**
- ML applied to a real healthcare problem with direct clinical utility
- Clean architecture: ML pipeline (`svm_func.py`) fully separated from web layer (`app.py`)
- Full-stack: data preprocessing → model training → deployed Flask web application
- Reduces unnecessary surgeries by accurately identifying benign tumors

**Repo:** [Breast_cancer_prediction](https://github.com/NeheMalviya1243/Breast_cancer_prediction)

---

### 04. Rider Event Hub

**Tech Stack:** HTML5 | CSS3 | JavaScript | React (CDN) | Supabase (PostgreSQL) | Netlify

> A full-stack campus event discovery platform for Rider University students — featuring real-time RSVP tracking, QR code sharing, admin moderation, and a live Supabase backend.

**What it does:**
- Centralized hub for all Rider University campus events (Academic, Networking, Club, Food, and more)
- Students browse by list or calendar view, filter by category/location/keyword, and RSVP with one click
- RSVP capacity tracking with real-time progress bar and sold-out detection
- Built-in QR code generator for every event for easy sharing
- Event submission form restricted to `@rider.edu` emails with admin approval workflow
- Admin dashboard to approve/reject events, feature listings, and export data to CSV
- Comments section and browser notification reminders per event

**Highlights:**
- Full-stack: React frontend + Supabase PostgreSQL backend + deployed on Netlify
- Relational database schema with foreign keys, cascade deletes, and atomic SQL functions for concurrent RSVP/view updates
- Built for real university use with `@rider.edu` email validation and role-based access (student / organizer / admin)
- Production deployment configured with `netlify.toml`

**Repo:** [rider_event_hub](https://github.com/NeheMalviya1243/rider_event_hub)

---

## Contact

- **GitHub:** [github.com/NeheMalviya1243](https://github.com/NeheMalviya1243)
- **University:** Rider University — Business Data Analytics
- **Location:** Lawrence Township, NJ
