📧 Automated Email Sender (Python)

This project is a Python-based automation script that sends personalized emails to multiple recipients using data from a CSV file. It is designed to simplify bulk email sending with features like attachments, retry handling, and logging.

🚀 Features
Send emails to multiple users from a CSV file
Personalized email content using recipient names
File attachment support (e.g., PDF reports)
Retry mechanism for failed email attempts
Logging system to track success and errors
📂 How It Works
The script reads recipient details (name and email) from a CSV file.
For each recipient, it creates a personalized email message.
It attaches a file (if available).
It connects to the SMTP server (Gmail) and sends the email.
If sending fails, it retries up to a defined limit.
All activities (success/failure) are recorded in a log file.
⚙️ Configuration

Before running the script, update the following:

SENDER_EMAIL → Your Gmail address
APP_PASSWORD → Gmail App Password (not your normal password)
CSV_FILE → Path to recipients file
ATTACHMENT_PATH → File you want to send
📄 CSV Format

Your recipients.csv file should look like this:

name,email
Ali,ali@example.com
Sara,sara@example.com
📝 Output
Emails are sent to all valid recipients
Logs are saved in email_log.txt
Console shows success or retry messages
⚠️ Notes
Make sure to enable App Passwords in your Gmail account
Ensure the attachment file exists before running
Internet connection is required
