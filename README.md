📊 Nginx Log Analyzer

This is a simple shell script to analyze Nginx access logs from the command line.
It extracts useful insights such as:

Top 5 IP addresses with the most requests

Top 5 most requested paths

Top 5 response status codes

Top 5 user agents

🚀 How It Works

The script uses common Linux tools like awk, sort, uniq, and head to process the log file.
It expects a standard Nginx access log format.

🛠️ Usage

Clone this repository:

git clone https://github.com/<your-username>/log-analysis.git
cd log-analysis


Make the script executable:

chmod +x nginx_log_analyzer.sh


Run the script with your access log file:

./nginx_log_analyzer.sh access.log

📄 Example Output
Analyzing log file: access.log

Top 5 IP addresses with the most requests:
45.76.135.253 - 1000 requests
142.93.143.8 - 600 requests
178.128.94.113 - 50 requests
43.224.43.187 - 30 requests
10.0.0.1 - 20 requests

Top 5 most requested paths:
/api/v1/users - 1000 requests
/api/v1/products - 600 requests
/api/v1/orders - 50 requests
/api/v1/payments - 30 requests
/api/v1/reviews - 20 requests

Top 5 response status codes:
200 - 1000 requests
404 - 600 requests
500 - 50 requests
401 - 30 requests
304 - 20 requests

Top 5 user agents:
Mozilla/5.0 ... - 700 requests
curl/7.68.0 - 400 requests
Googlebot/2.1 ... - 300 requests
PostmanRuntime/7.26.8 - 200 requests
python-requests/2.25.1 - 100 requests

📦 Requirements

Linux / macOS

Standard shell utilities (awk, sort, uniq, head)

🌟 Features

Simple and lightweight

No dependencies outside core Linux utilities

Works on any standard Nginx access log

🔮 Future Improvements

Filter logs by date range

Export results into JSON/CSV

Support Apache log format
