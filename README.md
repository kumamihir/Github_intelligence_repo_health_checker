LIVE_URL : https://kumamihir.github.io/Github_intelligence_repo_health_checker/

[README.md](https://github.com/user-attachments/files/24588429/README.md)
# 🤖 GitHub Intelligence Repository Health Checker

An AI-powered automated system that analyzes GitHub repositories to provide comprehensive health scores, risk assessments, and actionable insights using n8n workflow automation.

## 📋 Overview

This project combines **n8n workflow automation** with a modern web interface to deliver real-time intelligence on GitHub repositories. It evaluates repository health based on multiple metrics including contribution activity, code quality indicators, maintenance status, and community engagement.

## ✨ Features

- **🔄 Automated Data Collection**: n8n workflow automatically fetches and processes repository data
- **📊 Health Score Calculation**: Comprehensive scoring system based on multiple repository metrics
- **👥 Contributor Analysis**: Deep insights into contributor activity and patterns
- **📈 Risk Assessment**: Identifies potential risks in repository maintenance and activity
- **📝 Markdown Reports**: Auto-generated detailed reports for easy sharing
- **🌐 Interactive Dashboard**: Clean, responsive web interface for visualizing results

## 🤖 AI Automation with n8n

The core of this project is an intelligent n8n workflow that orchestrates the entire analysis process:

### Workflow Architecture

The n8n automation consists of the following nodes:

1. **Webhook Trigger** - Initiates the workflow when a repository URL is submitted
2. **Parse Repository URL** - Extracts owner and repo name from GitHub URLs
3. **HTTP Request (Repo Data)** - Fetches repository metadata from GitHub API
4. **Normalize Repository Data** - Standardizes data structure for processing
5. **Parallel Data Fetching**: 
   - **Fetch Code Metrics** - Analyzes code structure and composition
   - **Fetch Contributors** - Retrieves contributor statistics and activity
6. **Merge Data Streams** - Combines all collected data into unified dataset
7. **Calculate Health Score** - Applies scoring algorithm based on multiple factors
8. **Generate Markdown Report** - Creates formatted analysis report

### Key Automation Benefits

- ⚡ **Real-time Analysis**: Instant results upon repository submission
- 🔁 **Scalable Processing**: Handles multiple requests efficiently through workflow parallelization
- 🎯 **Consistent Evaluation**: Standardized scoring methodology across all repositories
- 📦 **Modular Design**: Easy to extend with additional analysis nodes

## 🚀 Getting Started

### Prerequisites

- n8n installed (self-hosted or cloud)
- GitHub Personal Access Token (for API access)
- Web server (for hosting the frontend)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/kumamihir/Github_intelligence_repo_health_checker.git
   cd Github_intelligence_repo_health_checker
   ```

2. **Set up n8n workflow**
   - Import the n8n workflow (workflow file to be added)
   - Configure GitHub API credentials in n8n
   - Set up webhook URL in n8n settings

3. **Configure the frontend**
   - Update the webhook URL in `index.html` to point to your n8n webhook
   - Deploy `index.html` to your web server

4. **Start analyzing! **
   - Open the web interface
   - Enter a GitHub repository URL
   - View the comprehensive health report

## 📊 Health Metrics

The system evaluates repositories based on:

- **Activity Level**: Commit frequency, recent updates, issue resolution
- **Community Engagement**: Stars, forks, watchers, contributors
- **Maintenance Status**: Issue response time, PR merge rate, stale content
- **Code Quality**: Documentation, test coverage indicators, code structure
- **Risk Factors**: Bus factor, dependency freshness, security alerts

## 🛠️ Technology Stack

- **Automation**: n8n (workflow automation platform)
- **Frontend**: HTML, CSS, JavaScript
- **APIs**: GitHub REST API
- **Data Processing**: Custom scoring algorithms
- **Reporting**: Markdown generation

## 📸 Screenshots

### n8n Workflow
The complete automation workflow showing all processing nodes and data flow paths.

## 🎯 Use Cases

- **Project Selection**: Evaluate repositories before adopting dependencies
- **Health Monitoring**: Regular checkups on your own repositories
- **Due Diligence**: Assess open-source projects for enterprise use
- **Community Analysis**: Understand contributor patterns and project vitality

## 🤝 Contributing

Contributions are welcome! Feel free to:

- Report bugs or issues
- Suggest new metrics or features
- Improve the scoring algorithm
- Enhance the UI/UX
- Add more n8n workflow nodes for deeper analysis

## 📝 License

This project is open source and available under the MIT License.

## 👤 Author

**Mihir Kumar**
- GitHub: [@kumamihir](https://github.com/kumamihir)

## 🙏 Acknowledgments

- Built with [n8n](https://n8n.io/) - Fair-code workflow automation
- Powered by [GitHub API](https://docs.github.com/en/rest)
- Inspired by the need for better repository intelligence tools

---

⭐ If you find this project useful, please consider giving it a star! 
