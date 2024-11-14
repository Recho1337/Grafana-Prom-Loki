**Deploying the Monitoring Stack Locally**

*Prerequisites*

Docker: Ensure Docker is installed and running on your system.
Docker Compose: Install Docker Compose to manage multi-container Docker applications.

*Steps*

Clone the Repository:
    
    git clone https://github.com/recho1337/Grafana-Prom-Loki.git
    cd Grafana-Prom-Loki

*Start the Services:*

```docker-compose up -d```

This command will pull the necessary images, create and start the containers in detached mode.

*Accessing the Services*

Grafana:
    Open your browser and navigate to http://localhost:3000.
    Use the default credentials:
        Username: admin
        Password: recho123
    Remember to change the password for security reasons.

Prometheus:
    Open your browser and navigate to http://localhost:9090.

*Additional Notes*

Data Persistence:
    The configuration uses volumes to persist data collected by Prometheus, Grafana, and Promtail. This data will be stored in the ./data directory.
Security:
    The default Grafana password is not secure. Change it after the initial login.
    Consider adding authentication and authorization mechanisms to protect your monitoring stack.
Customization:
    You can customize the configuration files (e.g., Prometheus configuration, Grafana dashboards) to tailor the monitoring to your specific needs.

*By following these steps, you'll have a fully functional monitoring stack running locally. You can then use Grafana to visualize metrics and logs from your applications and system.*
