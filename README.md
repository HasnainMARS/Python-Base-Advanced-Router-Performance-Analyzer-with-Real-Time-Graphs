# Advanced Router Performance Analyzer with Real-Time Graphs

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Graphs-orange)
![Status](https://img.shields.io/badge/Status-Educational%20Only-red)

🚀 An **educational tool** to analyze router performance by safely sending requests, monitoring responses, and visualizing system usage with **real-time graphs**.

----

## ⚠️ Disclaimer

This project is for **educational and diagnostic purposes only**.
Do **NOT** use it on networks, routers, or devices you do not own or lack explicit permission to test.
Unauthorized testing may be illegal and disruptive.

---

## ✨ Features

* 🌐 HTTP request testing across common router endpoints
* 🔌 Telnet (port 23) connection attempts
* 📡 ICMP ping requests
* 📊 Real-time system monitoring with `matplotlib`:

  * CPU usage
  * Memory usage
  * Network throughput (sent/received)
  * Requests per second
* 📈 Detailed performance report at the end of each test

---

## 📦 Installation

Clone this repository:

```bash
git clone https://github.com/HasnainMARS/Python-Base-Advanced-Router-Performance-Analyzer-with-Real-Time-Graphs.git
cd Python-Base-Advanced-Router-Performance-Analyzer-with-Real-Time-Graphs
```

Create a virtual environment (recommended):

```bash
conda create -n router-test python=3.10
conda activate router-test
```

Install dependencies:

```bash
pip install -r requirements.txt
```

or manually:

```bash
pip install requests psutil matplotlib
```

---

## ▶️ Usage

Edit the target IP address in `main()` of `advanced_router_analyzer.py`:

```python
target_ip = "1354.1589.16.21"  # replace with your router IP
```

Run the analyzer:

```bash
python advanced_router_analyzer.py
```

✅ While the test runs:

* A live **graph window** will show resource usage and request rates.
* The terminal will display real-time stats.
* A final performance report will print at the end.

---

## 📊 Example Output

Console output snippet:

```
🚀 STARTING COMPREHENSIVE ROUTER PERFORMANCE TEST
🎯 Target: 132.1558.145.12 <<<<<<Replace with your IP
⏱ Duration: 30 seconds
🕐 Start Time: 2025-09-29T10:42:00
======================================================================
📊 MONITOR: CPU: 15% | RAM: 42% | REQ/s: 35.00 | NET: ↑12.1KB/s ↓10.7KB/s
...
📈 Test complete! Graphs will remain open for a short while...

📊 COMPREHENSIVE ROUTER PERFORMANCE REPORT
======================================================================
⏱ Test Duration: 30.15 seconds
📊 Total Operations: 1,050
📈 Operations/Second: 34.8
✅ Success Rate: 94.5% (993/1,050)
...
🏆 ROUTER PERFORMANCE ASSESSMENT:
💚 VERY GOOD - Strong consumer router
======================================================================
```

---

## 📁 Project Structure

```
router-analyzer/
├── advanced_router_analyzer.py   # main script
├── requirements.txt              # dependencies
└── README.md                     # this file
```

---

## 🛠 Requirements

* Python 3.8+
* [Requests](https://pypi.org/project/requests/)
* [psutil](https://pypi.org/project/psutil/)
* [matplotlib](https://matplotlib.org/)

---

## 🚧 Roadmap

* [ ] Add CLI arguments (`--ip`, `--duration`, `--workers`)
* [ ] Save performance logs to CSV/JSON
* [ ] Export graphs to PNG automatically

---

## 📜 License

MIT License — free to use, modify, and share.
Use responsibly.

---

## 🙌 Contributing

PRs are welcome! If you have improvements (e.g., better graphs, safer tests, logging), open a pull request.

---

## 💡 Educational Insights

* Real-time graphs visualize **system resource usage** during load.
* CPU spikes = processing load on your computer.
* Memory usage shows script footprint.
* Network graphs illustrate request/response patterns.
* Final report helps understand router resilience under stress.


