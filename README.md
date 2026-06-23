🚀 Key Features
Multi-Threaded & Asynchronous Speed: Built with asyncio and multi-threading support to process massive bulk lists of phone numbers simultaneously, achieving maximum validation velocity.

Intelligent Phone Number Formatting: Automatically parses country codes and standardizes varied phone number formats (e.g., converting local formats into international +E.164 standards) before sending requests.

High-Accuracy Endpoint Analysis: Directly communicates with Amazon's official authentication and password-reset endpoints, analyzing precise status codes and JSON responses to verify account existence.

Anti-Bot & CAPTCHA Bypass: Integrated with automated proxy rotation (HTTP/S, SOCKS5) and dynamic User-Agent switching to mimic human behavior, easily bypassing rate limits and IP bans.

Real-Time Structured Output: Automatically filters and sorts results instantly into organized text files:

valid_accounts.txt: Phone numbers/emails actively registered on Amazon.

invalid_accounts.txt: Numbers/emails with no Amazon account associated.

Robust Error Handling: Features an automated retry mechanism to gracefully handle proxy timeouts, dropped connections, or bad gateway responses without interrupting the progress.

🛠️ Tech Stack
Python 3.x

Aiohttp / Requests: For handling rapid, parallel HTTP request/response lifecycles.

Asyncio / Threading: For managing concurrent tasks efficiently without blocking performance.

Phonenumbers Library: For client-side phone number validation and normalization to save bandwidth.

Fake-UserAgent: For generating randomized browser fingerprints to prevent detection.

📋 Workflow
Load your target phone numbers (or emails) into the input.txt file.

Add your proxy list to proxies.txt to distribute the request load and protect your IP.

Launch the script; it cleans the syntax, applies the correct international formats, and checks them against the target Amazon endpoints.

The system parses the server's response payload, categorizes the account as Valid or Invalid, and instantly updates the live console stats.
