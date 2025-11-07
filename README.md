# UK Company Database 🏢

A comprehensive Streamlit application for searching and analyzing UK companies using the official Companies House API. Perfect for due diligence, business intelligence, and market research.

## ✨ Features

### 🔍 **Real-time Company Search**
- Search UK companies by name or registration number
- Official Companies House data integration
- Up to 50 search results with detailed filtering

### 📊 **Detailed Company Profiles**
- Official registration data and company status
- Business activities and SIC codes
- Registered office addresses
- Incorporation dates and company types

### 👥 **Directors & Officers Analysis**
- Complete leadership information
- Appointment and resignation dates
- Nationality and occupation details
- Officer role classifications

### 🎯 **Ultimate Beneficial Owners (PSCs)**
- Persons with Significant Control data
- Nature of control and ownership percentages
- Corporate and individual beneficial owners
- Notification dates and control structures

### 🕸️ **Network Graph Visualization**
- Interactive company relationship mapping
- Shared directors and ownership connections
- Visual network analysis with Plotly
- Company ecosystem understanding

### 🎨 **Professional UI**
- Accordion-style organization for clean data presentation
- Responsive design with professional styling
- Interactive visualizations and charts
- Mobile-friendly interface

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- Companies House API key (free registration required)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/kaljuvee/uk-company-db.git
   cd uk-company-db
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure API key**
   ```bash
   cp .env.sample .env
   # Edit .env and add your Companies House API key
   ```

4. **Run the application**
   ```bash
   streamlit run Home.py
   ```

5. **Open in browser**
   - Navigate to `http://localhost:8501`
   - Enter your API key in the sidebar
   - Start searching UK companies!

## 🔑 Getting a Companies House API Key

1. Visit [Companies House Developer Hub](https://developer.company-information.service.gov.uk/)
2. Register for a free account
3. Create a new application
4. Copy your API key to the `.env` file

## 📖 Usage Guide

### Basic Company Search
1. Enter your Companies House API key in the sidebar
2. Type a company name (e.g., "Tesco PLC") or company number
3. Click "🔍 Search Companies"
4. Browse results and click "📊 Get Detailed Info" for comprehensive analysis

### Network Analysis
1. Enter a company name in the search field
2. Click "🕸️ Build Network Graph"
3. Explore the interactive network visualization
4. Hover over nodes for detailed information

### Example Searches
- **Tesco PLC** - Major UK retailer
- **BP PLC** - Energy company  
- **Vodafone Group PLC** - Telecommunications
- **HSBC Holdings PLC** - Banking and financial services
- **00445790** - Direct company number search

## 🏗️ Technical Architecture

### Core Components
- **`app.py`** - Main Streamlit application
- **`companies_house_api.py`** - Companies House API client
- **`.env`** - Environment configuration
- **`requirements.txt`** - Python dependencies

### API Integration
- Official UK Companies House REST API
- Rate limiting and error handling
- Comprehensive data models for companies, officers, and PSCs
- Network graph generation algorithms

### Data Models
- **CompanyProfile** - Complete company information
- **Officer** - Director and officer details
- **PSC** - Persons with Significant Control
- **Network Graph** - Relationship mapping data

## 🎯 Business Applications

### Due Diligence
- Verify company registration and status
- Check director backgrounds and appointments
- Identify ultimate beneficial owners
- Assess regulatory compliance

### Market Research
- Analyze competitor structures
- Identify industry connections
- Research business networks
- Track corporate changes

### Risk Assessment
- Evaluate company stability
- Check for dormant or dissolved status
- Analyze ownership structures
- Identify potential conflicts of interest

### Investment Analysis
- Research target companies
- Understand ownership hierarchies
- Analyze management teams
- Map business relationships

## 🛠️ Development

### Project Structure
```
uk-company-db/
├── Home.py                   # Main Streamlit application
├── utils/
│   ├── __init__.py          # Python package init
│   └── companies_house_api.py # API client and data models
├── requirements.txt          # Python dependencies
├── .env.sample              # Environment template
├── .env                     # Environment configuration
├── README.md               # Documentation
└── .gitignore             # Git ignore rules
```

### Key Features Implementation
- **Search functionality** with real-time API calls
- **Detailed company profiles** with structured data display
- **Interactive network graphs** using Plotly
- **Professional UI** with custom CSS styling
- **Error handling** and user feedback
- **Session state management** for smooth user experience

## 📊 Data Sources

All data is sourced from the official UK Companies House API, providing:
- **Real-time accuracy** - Live government data
- **Comprehensive coverage** - All UK registered companies
- **Official status** - Legally authoritative information
- **Regular updates** - Automatically synchronized

## 🔒 Security & Privacy

- API keys stored securely in environment variables
- No data persistence - all searches are real-time
- Official government data source
- Rate limiting to respect API guidelines

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📞 Support

For issues or questions:
1. Check the [Companies House API documentation](https://developer.company-information.service.gov.uk/api/docs/)
2. Review the application logs for error details
3. Ensure your API key is valid and has sufficient quota

## 🎉 Acknowledgments

- **Companies House** for providing the official UK company data API
- **Streamlit** for the excellent web application framework
- **Plotly** for interactive data visualizations

---

**UK Company Database** - Professional UK company analysis made simple 🏢
