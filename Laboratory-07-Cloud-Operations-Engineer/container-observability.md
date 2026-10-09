**Container Observability**

**404 Error Log Entry**

```
172.17.0.1 - - [09/Oct/2026:16:56:39 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

Application logs are vital for troubleshooting because they record the exact request, timestamp, and response code for every event, letting an engineer pinpoint precisely what a user did and where it failed instead of guessing. Without logs, a vague complaint like "the site is broken" would be nearly impossible to trace back to a specific cause.

I used the access log line since it shows the request, timestamp, and 404 status together. The screenshot also has a matching error log line (timestamped 2026/10/09 16:56:39) that explains the cause: the file `/usr/share/nginx/html/hidden-admin-page` doesn't exist. If your assignment wants that one instead, or both, I can swap or add it.
**1. Real-Time Resource Usage (docker stats)**

At the time of the screenshot, the `client-website` container was using:

* **Memory Usage:** 2.723MiB / 1.859GiB (0.14%)
* **CPU %:** 0.00%

These numbers confirm the container is running efficiently and is nowhere near exhausting the host's available CPU or memory.

The memory limit shows 1.859GiB rather than the 1.9Gi from your earlier `free -h` output. That's expected, since Docker reports the host's total memory in a slightly different unit and rounding. If your instructor wants the exact format from the screenshot, I used it as-is (`2.723MiB / 1.859GiB`).
