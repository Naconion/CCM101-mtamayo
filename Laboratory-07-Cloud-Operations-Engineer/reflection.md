# Mission Reflection

###  Why is it important to check the host server's resources even if your containers are running perfectly?
Even if my containers are running smoothly, they still rely on the host machine’s actual hardware. 
If the host server runs out of overall disk space or RAM, the host itself or the Docker engine can crash, bringing down all running containers regardless of their individual limits. 
Checking host health ensures the system has enough headroom before traffic spikes hit.

### If a user complains that they cannot log into a web application, how would the docker logs command help you solve the problem?
Running `docker logs` lets me see the actual request history and server responses in real time. I can check if the login attempt generated a `404 Not Found`, a `500 Internal Server Error`, or a database connection error. Seeing the exact timestamp and HTTP status code helps me pinpoint whether it's a broken route, a backend crash, or just invalid credentials without guessing.

### What is the difference between monitoring logs (Checkpoint 4) and monitoring metrics (Checkpoint 5)?
Logs are detailed event records that show *what* happened, like specific HTTP requests, user activity, and software errors. 
Metrics, on the other hand, are numerical performance data that show *how much* resources are being used, such as CPU usage percentage, memory consumption, and network I/O.

### How do you think large enterprise companies monitor thousands of containers at the same time?
Large enterprise companies use automated observability platforms like Prometheus and Grafana. 
Prometheus regularly collects performance metrics and log data across hundreds or thousands of containers, while Grafana visualizes all that data into clean, real-time dashboards with automatic alerts if something starts failing.

### How has your ability to troubleshoot Linux environments improved?
My confidence in using terminal commands to diagnose issues has grown a lot. 
Instead of just running containers and hoping they work, I now know how to check physical hardware stats, inspect container logs, and monitor live metrics to prove system health and fix errors quickly.
