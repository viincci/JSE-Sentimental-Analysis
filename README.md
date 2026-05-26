# JSE Sentiment Analysis
## Project Overview
The JSE Sentiment Analysis project is designed to analyze news sentiment for the JSE Top 40 Index. It fetches news data, performs sentiment analysis using a machine learning model, and displays the results in a web application.
## Key Features
- Fetches JSE Top 40 Index data using yfinance
- Fetches news data using the GNews API
- Performs sentiment analysis using the ProsusAI/finbert model
- Displays sentiment analysis results in a web application
## Tech Stack
- Python 3.x
- Flask
- yfinance
- requests
- pandas
- seaborn
- matplotlib
- transformers
- GNews API
## Installation
1. Clone the repository: git clone https://github.com/your-username/JSE-Sentimental-Analysis.git
2. Install dependencies: pip install -r requirements.txt
## Usage
1. Set the NEWS_API_KEY environment variable
2. Run the application: gunicorn app:app
## Environment Variables
- NEWS_API_KEY: GNews API key
## Code

```
from flask import Flask, jsonify, render_template
import yfinance as yf
import requests
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
from transformers import pipeline
import os
from dotenv import load_dotenv
```
## Vercel Deployment
The project can be deployed to Vercel using the render.yaml file. The NEWS_API_KEY environment variable must be set manually in the Render dashboard.