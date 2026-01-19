# Prometheus & Grafana Monitoring – Practical Implementation 🚀

This project demonstrates a **practical implementation of Prometheus and Grafana** for monitoring a Node.js backend application. It covers metric collection, visualization, and alerting using containerized services.

---

## 📌 Overview

In this project, I built a **simple Node.js backend** that exposes Prometheus-compatible metrics and deployed it along with **Prometheus and Grafana** using **Docker Compose**.

The goal was to understand:

* How Prometheus scrapes metrics from services
* How Grafana visualizes those metrics
* How alerts can be configured based on metric thresholds

---

## 🛠️ Tech Stack

* **Node.js**
* **Prometheus**
* **Grafana**
* **Docker & Docker Compose**

---

## 📊 Metrics Implemented

The Node.js backend exposes the following Prometheus metrics:

* **Counter** – to track total number of requests
* **Gauge** – to track current values (e.g., active users or memory usage)
* **Histogram** – to measure request duration and latency distribution

Metrics are exposed via a `/metrics` endpoint for Prometheus scraping.

---

## 🐳 Dockerized Setup

All services are containerized and connected using a shared Docker network:

* **Node.js Backend**
* **Prometheus**
* **Grafana**

Docker Compose is used to orchestrate and run the complete monitoring stack.

---

## 🌐 Access URLs

Once the services are up and running:

* **Prometheus UI:** [http://localhost:9090](http://localhost:9090)
* **Grafana UI:** [http://localhost:3001](http://localhost:3001)

In Grafana:

* Prometheus is added as a data source
* Dashboards and visualizations are created
* Alert rules are configured based on metrics

---

## 🚀 How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/Banti4750/Prometheus-practical.git
   cd Prometheus-practical
   ```

2. Start all services using Docker Compose:

   ```bash
   docker-compose up --build
   ```

3. Access Prometheus and Grafana using the URLs mentioned above.

---

## 📚 Reference

Learning resource used for this implementation:
[https://projects.100xdevs.com/tracks/prom-graf-1/Prometheus-and-Grafana-15](https://projects.100xdevs.com/tracks/prom-graf-1/Prometheus-and-Grafana-15)

---

## 🎯 Key Learnings

* Exposing application metrics in Node.js
* Prometheus scraping and querying (PromQL)
* Grafana dashboards and alerting
* Containerized monitoring setup using Docker Compose

---

## 🤝 Author

**Banti Kumar**
GitHub: [https://github.com/Banti4750](https://github.com/Banti4750)

Feel free to ⭐ the repository if you find it helpful!
