# 📈 Automated EUR/INR Exchange Rate Email Notifier

This Python script automatically tracks the EUR/INR exchange rate in real-time and sends an email with the latest rate and a plotted graph of the currency trend. It's ideal for finance professionals, traders, or anyone needing regular updates on forex rates.

---

## 🚀 Features

- 📊 Fetches live **EUR/INR** exchange rate using the [Yahoo Finance API](https://pypi.org/project/yfinance/)
- 📈 Generates and sends a **line chart** of the exchange rate trend
- 📧 Sends **daily email updates** with the latest rate and visual graph
- 🕒 Automates the process to run every **24 hours**

---

## 🛠️ Technologies Used

- `yfinance` – for retrieving financial data  
- `matplotlib` – for plotting exchange rate trends  
- `smtplib` and `email` – for sending automated email with attachments  
- `time` – for scheduling the daily execution  

---

## 📦 Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/eur-inr-email-bot.git
   cd eur-inr-email-bot
Install dependencies:

bash
Copy
Edit
pip install yfinance matplotlib
Set up Gmail:

Enable 2FA on your Gmail account

Create an App Password and replace it in the script at server.login(sender_email, "<APP_PASSWORD>")

⚙️ Configuration
Update the following variables in the script:

python
Copy
Edit
sender_email = "your-email@gmail.com"
email_recipient = "recipient-email@gmail.com"
▶️ How It Works
The script performs the following actions:

Downloads the EUR/INR 1-minute interval exchange rate data for the past day.

Plots the data and saves it as an image (eur_inr_plot.png).

Sends an email with the latest exchange rate and the graph as an attachment.

Waits 24 hours and repeats the process.

💡 Example Output
Subject: EUR/INR - Today's Exchange Rate Update
Body:

rust
Copy
Edit
Here is the latest update for EUR/INR:

Latest Exchange Rate: 90.34 INR.

See the attached graph for details.
Attachment: A graph image showing the full-day exchange rate movement.

🛑 Warning
Do not commit your actual email credentials to GitHub.

Consider using environment variables or a .env file for secure credential management.

📌 Future Enhancements
Add support for multiple currency pairs

Use a scheduling library like APScheduler or cron

Deploy on a cloud VM for true automation

👨‍💻 Author
Meet Patel – LinkedIn
Feel free to reach out for feedback or collaboration!
