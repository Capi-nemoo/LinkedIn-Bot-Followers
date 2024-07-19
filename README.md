# <img src="https://github.com/user-attachments/assets/9115aa71-ea52-4fb3-b629-b1a1b5833515" width="20" height="20"> LinkedIn Follower Bot <img src="https://github.com/user-attachments/assets/9115aa71-ea52-4fb3-b629-b1a1b5833515" width="20" height="20"> 

![GitHub stars](https://img.shields.io/github/stars/Connor9994/LinkedIn-Follower-Bot?style=social) ![GitHub forks](https://img.shields.io/github/forks/Connor9994/LinkedIn-Follower-Bot?style=social) ![GitHub issues](https://img.shields.io/github/issues/Connor9994/LinkedIn-Follower-Bot) 

## 🚀 Overview

Welcome to the **LinkedIn Follower Bot**! This Python script automates the process of following accounts on LinkedIn, designed to enhance your networking capabilities while ensuring the safety of your account. Build professional connections effortlessly and manage your LinkedIn presence with ease!

[LinkedIn Follower Bot](https://github.com/Connor9994/LinkedIn-Follower-Bot)

### Key Features

- **Automated Account Following**: Automatically follow potential connections based on your LinkedIn network growth.
- **Weekly Limits**: Prevents exceeding a threshold (100 accounts) to avoid flags or restrictions from LinkedIn.
- **Daily Execution Check**: Ensures the bot runs only once a day.
- **Log Management**: Maintains a log of the dates of each 25-account interval for easy tracking.

### **NoDriver Instead of Selenium**
Official successor of the Undetected-Chromedriver python package that does NOT use WebDriver 
https://github.com/ultrafunkamsterdam/nodriver

## ⚙️ Requirements

Make sure you have Python installed, then install the required library by running:

```bash
pip install -r requirements.txt
```

## 🛠 Getting Started

### Prerequisites

- Python 3.6 or higher
- Chrome Browser
- LinkedIn Account
- Proper setup of paths in the script

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Connor9994/LinkedIn-Follower-Bot.git
   cd LinkedIn-Follower-Bot
   ```

2. Modify the paths in the script as necessary for your system.
   ```
   browserPath = Your Chrome Directory
   (Windows: C:\Program Files\Google\Chrome\Application\chrome.exe)
   
   profilePath = Where you want to save your LinkedIn User Data
   (Eg. C:\Users\Administrator\Desktop\LinkedIn Follower Bot\Users\LinkedIn)

   LoggedIn = (1 - Logged In / 0 - Logged Out)
   Run Script w/ 0, log in to LinkedIn, press enter to save the Cookies/Etc to profilePath
   Change LoggedIn to 1
   ```

4. Run the script:

   ```bash
   python LinkedInFollower.py
   ```

## 📜 Usage

The script will read from `AccountLog.txt` to check prior follow activity and will execute the follow actions accordingly. The following sequence occurs:

1. Checks if the bot has run today or if the weekly following limit has been reached.
2. Launches Chrome.
3. Scrolls through the LinkedIn network page to find accounts to follow.
4. Follows accounts dynamically until the limit is reached.
5. Logs the activity/date in `AccountLog.txt`.

## 🚧 Disclaimer

Use this bot responsibly. Automation goes against the Terms of Service of LinkedIn, and excessive use will result in account restrictions. Always ensure to adhere to LinkedIn guidelines. This is for educational purposes only!

## 📧 Contributing

Contributions are welcome! Feel free to open issues or pull requests to improve the script, enhance features, or fix bugs.
