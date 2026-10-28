# Container Observability

## Application Log Analysis (404 Error Line)
Below is the specific log entry captured when simulating an invalid request (`/hidden-admin-page`), showing the HTTP `404 Not Found` response code:

```text
172.17.0.1 - - [28/Oct/2026:11:54:42 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

## 2-Sentence explanation of why application logs are vital for troubleshooting.

Application logs act as a reliable event trail by recording exact timestamps, client IP addresses, and specific HTTP response codes requested. They enable developers and Site Reliability Engineers to precisely isolate when, where, and why an error occurred without needing to guess.

## Client-Website CPU and Memory usage

```text
CONTAINER ID   NAME             CPU %     MEM USAGE / LIMIT     MEM %     NET I/O           BLOCK I/O     PIDS 
5091d7394c70   client-website   0.00%     2.719MiB / 1.859GiB   0.14%     3.84kB / 5.29kB   0B / 12.3kB   2 
```
