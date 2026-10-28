# Container Observability

## 1. Application Log Analysis (404 Error Line)
Below is the specific log entry captured when simulating an invalid request (`/hidden-admin-page`), showing the HTTP `404 Not Found` response code:

```text
172.17.0.1 - - [28/Oct/2026:11:54:42 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
