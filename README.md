# <img width="48" height="48" alt="image" src="https://github.com/user-attachments/assets/5a658a68-8cf0-4187-909a-8d1c2dbae9e9" />
 Twitter Support Ticket System (AI-Powered)

> A **Machine Learning–driven Support Ticket System** inspired by **Twitter’s customer service model**, built to analyse sentiment, prioritise issues, and assist support agents in real time.

---

## Overview

This project combines **social media integration**, **natural language processing (NLP)**, and **ticket management** to create an intelligent customer support solution.  

It automatically classifies and prioritises user complaints from Twitter, routes them to agents, and even provides AI-assisted responses — boosting efficiency and user satisfaction.

---

## Key Features

-  **Twitter Customer Support** – TWCS tabular data that captures tweets mentioning support issues and responses.  
- **ML-Powered Classification** – Uses NLP to detect issue type, urgency, and sentiment.  
- **AI-Assisted Replies** – Suggests responses for support agents using fine-tuned transformer models.  
- **Analytics Dashboard** – Visualises issue categories, response times, and sentiment trends.  
- **Real-time Notifications** – Alerts agents about new tickets or urgent complaints.  
-  **Auto-Prioritisation** – High-severity issues move to the top of the queue.  
-  **Role-Based Access** – Secure roles for users, agents, and admins.

---
## Data Data
TWC dataset (twcs.csv) usually has columns like:
- **tweet_id**

- **author_id**

- **inbound**

- **response_tweet_id**


| Column      | Type    | Description                                         | Example |
|--------------|---------|-----------------------------------------------------|----------|
| ticket_id    | string  | Unique ID automatically generated for each ticket.  | `a1b2c3d4` |
| username     | string  | Twitter handle or username of the person tweeting. | `@john` |
| text         | string  | The original tweet text.                           | `My internet keeps disconnecting. Please help!` |
| is_support   | int     | Flag indicating if the tweet is a support issue (1) or not (0). | `1` |
| issue_type   | string  | Detected category of the issue based on keywords.  | `Connectivity` |
| status       | string  | Current ticket status (e.g., Open, Closed, Resolved). | `Open` |



---

##  Machine Learning Components

| Task | Model / Method |
|------|----------------|
| **Sentiment Analysis** | BERT / RoBERTa fine-tuned on Twitter data |
| **Topic Classification** | Logistic Regression / SVM / Transformer-based classifier |
| **Response Suggestion** | GPT / fine-tuned seq2seq model |
| **Data Source** | Twitter API (via Tweepy) |
| **Preprocessing** | NLTK / SpaCy / HuggingFace Transformers |

---

## 🛠️ Tech Stack

| Layer | Technologies |
|-------|---------------|
| **Frontend** | React / Next.js, TailwindCSS |
| **Backend** | Python (FastAPI / Flask) |
| **Machine Learning** | PyTorch / Scikit-learn / Transformers |
| **Database** | PostgreSQL / MongoDB |
| **APIs** | Twitter API v2, OpenAI API (optional) |
| **Visualization** | Plotly / Chart.js / Recharts |
| **Deployment** | Docker, Render / Vercel / AWS |

---

## 📈 Dashboard Preview (Concept)

