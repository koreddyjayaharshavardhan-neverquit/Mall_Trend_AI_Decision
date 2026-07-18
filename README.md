# MallTrend AI

MallTrend AI is an intelligent dashboard application built with Gradio that provides retail and mall trend analysis. It aggregates data from various sources (YouTube, News, RSS) and leverages the Google Gemini API to analyze trends, generate insights, and provide a conversational assistant for your retail trend queries.

## Features

- **Dashboard View**: Get an overall report of mall trends based on city and category.
- **Category Insights**: Deep dive into specific retail categories to understand market demand and predictions.
- **Comparative Trends**: Compare two different trend keywords side-by-side to analyze their relative performance.
- **MallTrend Assistant**: An AI assistant powered by Google Gemini to answer your specific questions about trends in any city or category.
- **Customer Feedback System**: Collect customer feedback via QR codes and analyze the data using AI to identify top products.

## Technologies Used

- **Gradio**: For the interactive web interface.
- **Google Gemini**: For intelligent analysis and assistant capabilities.
- **Firebase Firestore**: For storing customer feedback data.
- **APIs**: YouTube Data API, News API, and RSS feeds for trend data aggregation.
- **Other Python Libraries**: `pandas`, `fastapi`, `uvicorn`, `qrcode`, `pillow`, `feedparser`

## Setup & Installation

1. **Install dependencies**:
   Make sure you have Python installed. Run the following command to install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

2. **Environment Variables**:
   You will need to set up your API keys. Create a `.env` file in the root directory and add the following keys:
   ```env
   mall_trend_api=your_gemini_api_key_here
   youtube_api=your_youtube_api_key_here
   news_api=your_news_api_key_here
   ```

## Running the Application

To start the MallTrend AI dashboard, run:
```bash
python app.py
```

The application will launch on a local Gradio server, which you can access in your web browser (typically at `http://127.0.0.1:7860`).
