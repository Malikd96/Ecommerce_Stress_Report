# Ecommerce_Stress_Report

# Ecommerce Load & Stress Testing Project

## 📌 Project Overview
This project analyzes the performance and stability of a publicly accessible e-commerce application (https://automationexercise.com) using Apache JMeter. The goal was to evaluate the system under both normal and extreme conditions by performing load and stress tests on the product search functionality.

---

## 🛠️ Tools Used
- **Apache JMeter 5.6.3** – For simulating load and collecting performance metrics.
- **OWASP ZAP** – For penetration testing (optional security scanning).
- **Windows 11** – Operating environment.
- **GitHub** – For version control and code collaboration.

---

## 🧪 Test Scenarios

### ✅ Load Test
- Simulated **50 concurrent users** over **5 minutes**.
- Targeted endpoint: Search functionality (searching for products).
- Metrics Captured:
  - Response Time: Avg 396 ms
  - Throughput: 10.2 requests/min
  - Error Rate: 0%

### 🔥 Stress Test
- Gradually increased load from **50 to 500 concurrent users**.
- Goal: Identify application breaking point and performance degradation.
- Metrics Captured:
  - Max Response Time: ~1214 ms
  - Throughput drop and error % increase after 400 users
  - System maintained stability up to 300–350 users

---

## 📈 Key Findings
- The application handles normal load (50 users) efficiently with **0% errors**.
- Under stress, performance begins to degrade beyond **350 users**.
- Throughput is relatively consistent until saturation, then drops sharply.
- No security vulnerabilities were exploited during OWASP ZAP scan, but headers like `Strict-Transport-Security` were missing.

---

## 📂 Project Structure
