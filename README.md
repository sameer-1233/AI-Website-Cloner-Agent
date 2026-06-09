# AI Website Cloner Agent

## Overview

AI Website Cloner Agent is an AI-powered web application that takes a website URL as input, analyzes the website structure using Large Language Models (LLMs), and generates a responsive website clone automatically.

The project demonstrates how AI can be used to understand website layouts and generate similar web pages with minimal human intervention.

---

## Features

* Website URL Input
* Automated Website Scraping
* AI-Powered Layout Analysis
* Website Structure Extraction
* Responsive HTML Generation
* FastAPI Backend
* Public Access via ngrok
* Groq + Llama 3.3 Integration

---

## System Architecture

```text
User URL
    │
    ▼
Website Scraper Agent
    │
    ▼
Layout Analysis Agent
(Groq + Llama 3.3 70B)
    │
    ▼
Clone Generation Agent
    │
    ▼
HTML Renderer
    │
    ▼
Generated Website Clone
```

---

## AI Agents

### Agent 1 – Website Scraper

Extracts:

* Website Title
* Headings
* Paragraphs
* Navigation Links
* Buttons

Technology Used:

* Requests
* BeautifulSoup

---

### Agent 2 – Layout Analysis Agent

Analyzes website structure using:

* Groq API
* Llama 3.3 70B Versatile

Extracts:

* Navbar Structure
* Hero Section
* CTA Buttons
* Website Sections
* Footer Structure

---

### Agent 3 – Clone Generation Agent

Generates a responsive website based on the extracted layout.

Features:

* Responsive Design
* Tailwind CSS
* Modern SaaS UI
* Professional Layout

---

### Agent 4 – Preview Renderer

Displays the generated website directly in the browser.

---

## Tech Stack

### Backend

* Python
* FastAPI

### AI

* Groq API
* Llama 3.3 70B Versatile

### Web Scraping

* BeautifulSoup
* Requests

### Deployment

* ngrok

### Development Environment

* Google Colab

---

## Installation

### Clone Repository

```bash
git clone https://github.com/your-username/ai-website-cloner.git

cd ai-website-cloner
```

### Install Dependencies

```bash
pip install requests beautifulsoup4 groq fastapi uvicorn pyngrok nest_asyncio lxml
```

---

## Configuration

Set your Groq API Key:

```python
from groq import Groq

client = Groq(
    api_key="YOUR_GROQ_API_KEY"
)
```

Set your ngrok Auth Token:

```python
from pyngrok import ngrok

ngrok.set_auth_token(
    "YOUR_NGROK_AUTH_TOKEN"
)
```

---

## Usage

Run the application.

Enter a website URL:

```text
https://stripe.com
```

The system will:

1. Scrape website content.
2. Analyze website structure.
3. Generate layout information.
4. Create a responsive HTML clone.
5. Display the generated website.

---

## Example Workflow

```text
Input:
https://stripe.com

↓

Scraping Website...

↓

Creating Layout...

↓

Generating Clone...

↓

Displaying Generated Website
```

---

## Project Structure

```text
AI-Website-Cloner/

│
├── app.py
├── scraper.py
├── analyzer.py
├── generator.py
├── generated_clone.html
├── README.md
│
└── requirements.txt
```

---

## Future Improvements

* Screenshot-Based Visual Analysis
* Better CSS Extraction
* Multi-Page Website Cloning
* Improved Layout Similarity
* Cloud Deployment
* User Authentication
* Database Integration

---

## Challenges Faced

* Extracting meaningful website structure
* Generating layouts from limited website data
* Building a complete AI-driven workflow
* Integrating multiple AI agents into one pipeline

---

## Results

The project successfully demonstrates:

* Automated website understanding
* AI-powered layout extraction
* Responsive website generation
* End-to-end AI agent workflow

---

## Author

Sameer Pathania

AI Website Cloner Agent
Internship Project
