<div align="center">

# 🤖 Instagram Followers Data Bot

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)](https://python.org)
[![Selenium](https://img.shields.io/badge/Selenium-4.15%2B-green?logo=selenium&logoColor=white)](https://selenium.dev)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

*A powerful automation tool for extracting and analyzing Instagram follower data*

[Features](#-features) • [Quick Start](#-quick-start) • [Installation](#-installation) • [Usage](#-usage) • [Output](#-output)

</div>

---

## 📖 Overview

The **Instagram Followers Data Bot** is a Jupyter Notebook-based automation tool that leverages Selenium WebDriver to extract comprehensive follower data from any public Instagram account. Whether you're conducting market research, analyzing competitor audiences, or building influencer databases, this bot streamlines the data collection process.

### 🎯 What It Does

1. **🔐 Secure Login** - Authenticates with your Instagram account (with 2FA support)
2. **📊 Profile Analysis** - Extracts stats from any target account (posts, followers, following)
3. **👥 Follower Extraction** - Scrapes the complete followers list
4. **📈 Deep Dive Analytics** - Collects detailed profile data for each follower
5. **💾 Data Export** - Saves everything to CSV format for further analysis

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🔒 **Secure Credentials** | Environment variable-based authentication (no hardcoded passwords!) |
| 🛡️ **2FA Support** | Handles two-factor authentication prompts |
| 📱 **Private/Public Detection** | Identifies private vs public profiles |
| ⏳ **Progress Tracking** | Real-time progress updates during scraping |
| 🚫 **Error Handling** | Robust exception handling for uninterrupted operation |
| 📁 **CSV Export** | Clean, structured output files |

---

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/matef88/Instgram_Followes_Data_Bot.git

# Navigate to the project
cd Instgram_Followes_Data_Bot

# Install dependencies
pip install -r requirements.txt

# Set up your credentials
cp .env.example .env
# Edit .env with your Instagram credentials

# Launch Jupyter Notebook
jupyter notebook Instgram_Followers_Data.ipynb
```

---

## 📦 Installation

### Prerequisites

- **Python 3.10+** - [Download Python](https://python.org/downloads/)
- **Google Chrome** - [Download Chrome](https://chrome.google.com)
- **ChromeDriver** - Automatically managed by Selenium 4.x

### Step-by-Step Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/matef88/Instgram_Followes_Data_Bot.git
   cd Instgram_Followes_Data_Bot
   ```

2. **Create Virtual Environment** (recommended)
   ```bash
   python -m venv venv
   
   # Windows
   venv\Scripts\activate
   
   # macOS/Linux
   source venv/bin/activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure Credentials**
   ```bash
   cp .env.example .env
   ```
   
   Edit the `.env` file with your details:
   ```env
   INSTAGRAM_USERNAME=your_username_here
   INSTAGRAM_PASSWORD=your_password_here
   TARGET_ACCOUNT=target_account_to_analyze
   ```

---

## 🎮 Usage

### Running the Bot

1. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook Instgram_Followers_Data.ipynb
   ```

2. **Execute Cells Sequentially**
   - Run each cell in order from top to bottom
   - When prompted, enter your 2FA code if you have two-factor authentication enabled

3. **Wait for Completion**
   - The bot will display progress updates
   - Large follower counts may take significant time

### Notebook Structure

| Section | Description |
|---------|-------------|
| **1. Import Dependencies** | Load all required libraries |
| **2. Configuration** | Load credentials from `.env` |
| **3. Helper Functions** | Utility functions for scraping |
| **4. Login** | Authenticate with Instagram |
| **5. Navigate to Target** | Open target profile |
| **6. Extract Followers** | Scroll and collect follower list |
| **7. Verify Data** | Preview extracted followers |
| **8. Save Followers** | Export to CSV |
| **9. Detailed Analysis** | Visit each follower's profile |
| **10. Save Final Data** | Export detailed CSV |
| **11. Cleanup** | Close browser |

---

## 📊 Output

The bot generates two CSV files:

### 1. `{target}_followers_list.csv`
Basic follower list with usernames.

| Username |
|----------|
| user1 |
| user2 |
| user3 |

### 2. `{target}_followers_detailed.csv`
Comprehensive profile data for each follower.

| Username | Posts | Followers | Following | Profile_Type |
|----------|-------|-----------|-----------|--------------|
| user1 | 150 | 2.5K | 300 | Public |
| user2 | 45 | 890 | 120 | Private |
| user3 | 0 | 100 | 500 | Public |

---

## ⚠️ Important Notes

### Legal & Ethical Usage

> **Disclaimer:** This tool is for educational and research purposes only. Always comply with Instagram's Terms of Service and applicable data protection laws (GDPR, CCPA, etc.).

### Best Practices

- ✅ Use for your own account analysis
- ✅ Obtain consent before scraping others' data
- ✅ Respect rate limits and add delays
- ❌ Don't use for spam or harassment
- ❌ Don't sell scraped data
- ❌ Don't overwhelm Instagram's servers

### Rate Limiting

Instagram may temporarily block accounts that make too many requests. The bot includes delays to mitigate this, but use responsibly.

---

## 🔧 Troubleshooting

| Issue | Solution |
|-------|----------|
| **ChromeDriver errors** | Ensure Chrome is updated; Selenium 4.x auto-manages drivers |
| **Login failed** | Check credentials in `.env`; verify 2FA code |
| **Empty follower list** | Target account may be private; check your access |
| **Timeout errors** | Increase wait times in the code; check internet connection |
| **Element not found** | Instagram may have updated their UI; XPath selectors may need updating |

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👤 About the Author / Origin

This project was originally created by **[matef88](https://github.com/matef88)**.

The repository provides a foundation for Instagram data extraction using Python and Selenium. This revitalized version includes:

- 🔐 Secure credential management
- 🐛 Bug fixes (indentation issues, error handling)
- 📚 Comprehensive documentation
- 🎨 Improved code structure and readability
- ⚡ Modern Python practices

*Show some love by starring the original repository! ⭐*

---

<div align="center">

**Made with ❤️ by the open-source community**

[⬆ Back to Top](#-instagram-followers-data-bot)

</div>
