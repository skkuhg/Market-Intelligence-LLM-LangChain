# Market Intelligence LLM Application

A comprehensive market intelligence application that combines **Tavily AI** for real-time data retrieval and **OpenAI GPT-4o-mini** for intelligent analysis and insight generation.

## 🚀 Features

- **Real-time Data Retrieval**: Fetch data from social media, news, and reports using Tavily AI
- **Three Analysis Types**: Market trends, customer sentiment, and competitive analysis
- **Batch Processing**: Analyze multiple queries simultaneously
- **Interactive Interface**: User-friendly query system
- **Comprehensive Dashboards**: Visual representation of analysis results
- **Export Functionality**: Save results in multiple formats (TXT, CSV)
- **Error Handling**: Robust error management and logging

## 🛠️ Setup Instructions

### 1. Prerequisites

- Python 3.8 or higher
- Git
- API keys for Tavily AI and OpenAI

### 2. Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/skkuhg/Market-Intelligence-LLM-LangChain.git
   cd Market-Intelligence-LLM-LangChain
   ```

2. Install required packages:
   ```bash
   pip install langchain langchain-openai langchain-community tavily-python python-dotenv pandas matplotlib seaborn
   ```

3. Set up environment variables:
   - Copy `.env.example` to `.env`
   - Add your API keys to the `.env` file:
     ```
     TAVILY_API_KEY=your_tavily_api_key_here
     OPENAI_API_KEY=your_openai_api_key_here
     ```

### 3. Getting API Keys

#### Tavily AI API Key
1. Visit [Tavily AI](https://tavily.com/)
2. Sign up for an account
3. Navigate to your dashboard to get your API key

#### OpenAI API Key
1. Visit [OpenAI Platform](https://platform.openai.com/api-keys)
2. Sign up/log in to your account
3. Generate a new API key

## 📊 Usage

### Running the Notebook

1. Open the Jupyter notebook:
   ```bash
   jupyter notebook market_intelligence_llm.ipynb
   ```

2. Run the cells sequentially to:
   - Install dependencies
   - Load libraries
   - Configure API keys
   - Initialize the application

### Example Usage

```python
# Initialize the application
app = MarketIntelligenceApp()

# Analyze market trends
trends_result = app.analyze(
    industry="technology",
    query="What are the latest trends in AI adoption?",
    analysis_type="trends"
)

# Analyze customer sentiment
sentiment_result = app.analyze(
    industry="healthcare",
    query="Customer sentiment towards AI diagnostic tools",
    analysis_type="sentiment"
)

# Competitive analysis
competitive_result = app.analyze(
    industry="fintech",
    query="Major players in AI-driven financial services",
    analysis_type="competitive"
)
```

## 🔧 Analysis Types

### 1. Market Trends Analysis
- Identifies key market trends
- Highlights growth opportunities
- Reveals potential challenges
- Provides actionable recommendations

### 2. Customer Sentiment Analysis
- Overall sentiment distribution
- Key themes in customer feedback
- Major concerns and pain points
- Improvement opportunities

### 3. Competitive Analysis
- Key competitors and market positions
- Competitive advantages and strategies
- Market share insights
- Innovation trends

## 📈 Advanced Features

### Batch Analysis
Process multiple queries simultaneously:
```python
batch_queries = [
    {
        "industry": "automotive",
        "query": "Electric vehicle market trends",
        "analysis_type": "trends"
    },
    {
        "industry": "retail",
        "query": "AI shopping assistant sentiment",
        "analysis_type": "sentiment"
    }
]
batch_results = batch_analysis(batch_queries)
```

### Interactive Interface
Run the interactive analysis tool:
```python
interactive_analysis()
```

### Export Results
Export analysis results to files:
```python
export_insights(result, "my_analysis.txt")
export_history_to_csv(app, "analysis_history.csv")
```

## 🔒 Security Notes

- **Never commit API keys** to version control
- Use environment variables or `.env` files for API keys
- The `.env` file is ignored by Git for security
- API keys are loaded from environment variables only

## 📊 Visualizations

The application includes:
- Sentiment distribution pie charts
- Analysis timeline plots
- Industry distribution bar charts
- Data source histograms
- Comprehensive dashboards

## 🚀 Applications

- **Market Research**: Understand industry trends and opportunities
- **Competitive Intelligence**: Analyze competitor strategies
- **Customer Insights**: Understand customer sentiment and preferences
- **Strategic Planning**: Make data-driven business decisions
- **Risk Assessment**: Identify potential market risks

## 🔧 Technical Stack

- **Data Retrieval**: Tavily AI
- **LLM Processing**: OpenAI GPT-4o-mini
- **Orchestration**: LangChain
- **Visualization**: Matplotlib, Seaborn
- **Data Processing**: Pandas
- **Environment**: Jupyter Notebook

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📞 Support

For questions or support, please open an issue on GitHub.

## 🔮 Future Enhancements

- [ ] Web interface using Streamlit
- [ ] Database integration for historical data
- [ ] Real-time monitoring and alerts
- [ ] Additional data sources
- [ ] Custom model fine-tuning
- [ ] API endpoint creation
- [ ] Cloud deployment options

---

**Ready to analyze market trends with AI!** 🚀
