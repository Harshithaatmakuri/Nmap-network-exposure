# 🔍 Nmap Network Exposure Analysis – Cybersecurity Internship Task 1

## ✅ Objective

Perform a local network scan using **Nmap**, identify active devices, detect open TCP ports, and analyze potential security risks based on exposed services.

---

## 🛠️ Tools & Configuration

- **Tool Used:** Nmap
- **Scan Type:** SYN Scan (`-sS`)
- **IP Range Scanned:** `192.168.1.0/24`

---

## 📊 Scan Results

The following open ports were discovered across the scanned IP range:

| Port | Service | Risk Description |
|------|---------|------------------|
| **22** | SSH     | Common target for brute-force attacks |
| **80** | HTTP    | Might expose outdated/unpatched web applications |
| **443** | HTTPS  | Ensure SSL certificates are valid and properly configured |
| **3306** | MySQL | Direct exposure of databases poses a high risk |

---

## 🔍 Analysis & Findings

- Open ports allow external communication with services running on your network devices.
- Services like SSH and MySQL, if exposed and unprotected, increase the **attack surface**.
- Weak or default configurations can be easily exploited using automated tools.

---

## 🔐 Security Implications

- **SSH (Port 22):** Should be limited to specific IPs or disabled if unused.
- **HTTP (Port 80):** Ensure web servers are patched and monitored.
- **MySQL (Port 3306):** Never expose database services directly to the internet.
- **General Advice:** Regularly audit open ports and remove unnecessary services.

---

## 📌 Conclusion

Using **Nmap** for network scanning helps detect services and exposures early. This task helped identify key weaknesses and understand how attackers could exploit improperly secured services. Mitigating these exposures is crucial for maintaining a secure environment.

---

## 📁 Files Included

- `README.md` – Full report and analysis  
- `Nmap_Report_Task_1.html` – HTML version of the scan report (optional rename suggestion from `TASK-1.html`)

---

## 🧾 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.
