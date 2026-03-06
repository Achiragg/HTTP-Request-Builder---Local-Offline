🛠️ HTTP Request Builder — 100% Local & Offline
A lightweight, fully offline browser-based tool to convert JSON API request configs into formatted Raw HTTP requests and cURL commands — running entirely on your local machine with zero network activity.

🔒 No internet required. No server. No data leaves your machine. Ever.


Why?
When debugging or analyzing API requests, it's common to paste raw JSON payloads into AI tools to get them converted into HTTP format. However, these payloads often contain sensitive information — auth tokens, user IDs, internal API keys, and more — which poses a data leakage risk when sent to external platforms.
This tool solves that by doing everything 100% locally in your browser. It is a single HTML file with no dependencies, no backend, and no network calls of any kind. You can even disconnect from the internet and it will work perfectly.

⚡ Fully Offline — How It Works
WhatDetail🖥️ Runs onYour local machine, inside your browser🌐 Network callsNone☁️ Data sent to serversNone📦 Installation neededNone🔌 Internet requiredNo
Just download the HTML file, open it in your browser, and use it. That's it.

Features

✅ Converts JSON API request config to Raw HTTP format
✅ Generates a ready-to-use cURL command
✅ Handles query parameters, request headers, and request body
✅ Auto-recalculates Content-Length from the actual body
✅ Sanitizes header values (handles embedded JSON, special characters, quoted strings)
✅ Syntax-highlighted output for easy reading
✅ One-click copy to clipboard
✅ 100% offline — no network, no backend, no tracking


Usage
1. Download
Download http-request-builder.html and open it in any modern browser (Chrome, Firefox, Edge, Safari). No internet connection needed.
2. Paste your JSON config
The tool accepts a JSON object in the following format:
json{
  "host": "api.example.com",
  "path": "/v1/endpoint",
  "method": "POST",
  "query": {
    "param1": "value1"
  },
  "requestHeaders": {
    "content-type": "application/json",
    "authorization": "Bearer <token>"
  },
  "requestBody": {
    "key": "value"
  }
}
3. Click Convert
Hit the ▶ CONVERT button and instantly get:

RAW HTTP tab — a properly formatted HTTP request with all headers and body
cURL tab — a copy-paste ready cURL command

4. Copy
Use the ⎘ COPY button to copy the output to your clipboard.

Supported Fields
FieldDescriptionhostThe target host (e.g. api.example.com)pathThe request path (e.g. /v1/users)methodHTTP method — GET, POST, PUT, DELETE, etc.queryKey-value pairs appended as query stringrequestHeadersAll request headers as key-value pairsrequestBodyRequest body (serialized as JSON)

host and content-length from requestHeaders are handled automatically — host is placed correctly in the request line, and content-length is recalculated from the actual body.


Screenshot

Open the HTML file in your browser to see the tool in action.


🔒 Security & Privacy
This tool was built with data privacy as the #1 priority.

Runs entirely in your browser as a single HTML file
No backend, no server, no cloud
No analytics, no tracking, no cookies
No external API calls or network requests of any kind
Works fully offline — you can use it on an air-gapped machine

Your API payloads, tokens, and sensitive headers never leave your machine.

License
MIT — free to use, modify, and distribute.
