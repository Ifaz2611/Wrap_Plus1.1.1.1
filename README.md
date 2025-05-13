# 🌐 WARP+ GB Farming Script (Educational Only)

Automate the generation of free WARP+ (1.1.1.1) data by sending randomized fake referral requests to Cloudflare’s API using Python.

> ⚠️ **Disclaimer**: This project is for **educational purposes only**. Abuse of this method may violate Cloudflare’s Terms of Service. Use at your own risk.

---

## 📌 Features

- 🔐 Generates randomized keys and install IDs
- 📡 Automates WARP+ referral requests
- 🔁 Infinite loop with cooldown between requests
- ✅ Tracks success and failure counts
- 🛡️ Basic error handling included

---

## 🚀 Getting Started

### 1. Clone the Repository


git clone https://github.com/yourusername/warp-plus-gb-farmer
cd warp-plus-gb-farmer
2. Install Dependencies
bash
Copy
Edit
pip install httpx
3. Set Your Referral ID
Open the script file and insert your WARP+ referral ID:

python
Copy
Edit
WARP_CLIENT_ID = "your-referral-id-here"
You can find your referral ID in your WARP+ invite link:
https://warp.plus/<your-referral-id>

4. Run the Script
bash
Copy
Edit
python warp_script.py
🛠️ How It Works
Generates a fake device identity

Sends a POST request to Cloudflare’s API using your referral ID

Adds +1GB per successful request

Example Output:

yaml
Copy
Edit
PASSED: +1GB (total: 3GB, failed: 0)
Sleep: 42 seconds.
💻 Tech Stack
Language: Python 3

HTTP Requests: httpx

Random ID Generation: Built-in libraries
```bash
🧪 Sample JSON Payload
json
Copy
Edit
{
  "key": "random_key=",
  "install_id": "random_install_id",
  "fcm_token": "random_install_id:APA91b[random_string]",
  "referrer": "your_referral_id",
  "warp_enabled": false,
  "tos": "2025-05-13T10:00:00.000+02:00",
  "type": "Android",
  "locale": "es_ES"
}
```
🧩 Optional Improvements
Proxy support for IP rotation

Retry logic with backoff

GUI interface or scheduling with cron

Real-time Telegram notifications

📜 License
This project is released under the MIT License.

👤 Author
Ifaz2611<br>
GitHub: Ifaz2611

🙏 Acknowledgments
Cloudflare WARP+ team (for an amazing product)

Open-source community contributors








