Project Overview: Devops-Pi-Security
Devops-Pi-Security is a Raspberry Pi-based DevOps portfolio project designed to demonstrate proficiency in Linux system administration, infrastructure automation, containerization, and monitoring—targeting entry-level roles such as Junior Systems Administrator, Security Analyst, or Site Reliability Engineer (SRE). This project leverages a self-hosted environment to showcase practical, industry-relevant skills aligned with modern DevOps practices, including Agile methodologies, Infrastructure as Code (IaC), CI/CD pipelines, cloud integration, and security best practices.

Current Features
Secure Web Hosting: An Apache HTTP server deployed with HTTPS, secured via Let’s Encrypt certificates, and accessible at pi-security.duckdns.org. Port 80 redirects to 443, ensuring encrypted traffic, with firewall rules managed via UFW.
Dynamic DNS: Integrated Duck DNS to maintain a consistent public endpoint, automating IP updates with a custom Bash script and cron job.
Containerization: Apache is containerized using Docker (devops-pi-apache), running on port 8080 to avoid conflicts with the live server, demonstrating portability and modern deployment practices.
Version Control: All configurations, scripts, and Docker assets are tracked in a Git repository (https://github.com/Bpeter57/devops-pi-security), with a proprietary license to protect intellectual property.
In-Progress Development
Monitoring: Implementing Prometheus and Grafana to monitor system and application performance. Prometheus is installed but currently failing due to a configuration error targeting Docker metrics (localhost:8080). Node Exporter is planned to add system-level metrics (e.g., CPU, memory), with Grafana dashboards in setup phase.
Planned Enhancements
Orchestration: Deploy the Dockerized Apache instance in a lightweight Kubernetes cluster (k3s) on the Raspberry Pi, showcasing container orchestration and scalability.
Infrastructure as Code (IaC): Automate server provisioning and configuration using Terraform for infrastructure definitions and Ansible for application deployment, ensuring repeatability and error prevention.
CI/CD Pipelines: Integrate Jenkins or GitHub Actions to automate Docker image builds, testing, and deployment, reflecting continuous integration and deployment workflows.
Cloud Deployment: Extend the project to AWS (EC2) using the Free Tier, demonstrating hybrid cloud capabilities and familiarity with public cloud platforms.
Security Hardening: Add tools like Fail2ban to protect against brute-force attacks, enhancing the security posture of the system.
Technical Skills Demonstrated
Linux Administration: Configuration of Apache, UFW, and system services on Raspberry Pi OS.
Networking: Management of ports, DNS, and HTTPS redirection.
DevOps Tools: Docker for containerization, Git for version control, and ongoing work with Prometheus/Grafana for monitoring.
Automation: Bash scripting for DNS updates and planned IaC with Terraform/Ansible.
Problem-Solving: Debugging configuration errors (e.g., Apache syntax, Prometheus setup) to maintain system reliability.
