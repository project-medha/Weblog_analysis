# Apache Log Analyzer

**Overview**
This project is a Python-based Apache log analyzer that processes HTTP access logs to extract, parse, and analyze data such as the most frequently accessed URLs, malicious traffic patterns, and user agents. The goal is to help identify traffic trends, detect anomalies, and gain insights into website usage.

**Features**
- Log Parsing:
  - Uses regular expressions to extract key fields like host, request type, URL, HTTP status code, and user agent from each log entry.
- Top URL Analysis:
  - Identifies the most requested URLs along with their access counts.
- Malicious Traffic Detection:
  - Filters out requests associated with bots, spiders, or other suspicious user agents.
  - Highlights potentially malicious activities like attacks on login pages or unusual HTTP requests.
- User Agent Analysis:
  - Aggregates and analyzes user agents to understand traffic sources (e.g., browsers, bots, etc.).

**How It Works**
1. Load Apache Log File:
   - Specify the path to the log file in the script (default: access_log.txt).
2. Parse Logs:
   - The regular expression extracts key fields like IP address, request type, URL, and user agent.
3. Analyze Data:
   - Count and rank requested URLs.
   - Filter out bot traffic and focus on human activity.
   - Generate insights about frequently visited pages and abnormal traffic patterns.
