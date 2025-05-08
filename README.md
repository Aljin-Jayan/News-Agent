News-Agent: Malayalam News Summarizer
====================================

A lightweight AI agent that fetches and summarizes latest news in Malayalam using Google Search.

Features:
- Generates summaries in simple Malayalam (English only for names/places)
- Focuses on latest news (last 24-48 hours)
- Delivers 2-3 bullet points per story (<60 words)
- Provides source links
- Uses only Google Search API

Setup:
1. Install dependencies:
   pip install -r requirements.txt

2. Configure environment:
   - Copy .env.example to .env
   - Add your API keys:
     GOOGLE_API_KEY=your_api_key
     GOOGLE_CSE_ID=your_search_engine_id

3. Run the agent:
   python -m agent

Example Usage:
from agent import news_agent
response = news_agent.query("കേരളത്തിലെ ഇന്നത്തെ വാർത്തകൾ")
print(response)

Sample Output:
• മുഖ്യമന്ത്രി പുതിയ ആരോഗ്യ പദ്ധതി ആരംഭിച്ചു
• കോഴിക്കോട്ട് മെട്രോ റൂട്ട് പ്രഖ്യാപിച്ചു
🔗 https://example.com/news

Files:
agent.py - Main agent logic
instructions.txt - AI behavior rules
util.py - Helper functions

License: MIT
Note: Requires Google Custom Search API credentials
