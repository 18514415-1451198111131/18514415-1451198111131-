# Cloud Workload Analysis

This project explores the **Cloud Workload Dataset for Scheduling Analysis**, which simulates real-world cloud computing environments and captures various metrics including resource utilization, task execution, and scheduling efficiency. The goal of this project is to perform meaningful data exploration and visualization to gain insights into performance patterns.

---

## 🔍 Dataset Overview

The dataset contains **5,000 records** with 15 features related to cloud workload scheduling, including:

- `Job_ID`
- `Task_Start_Time`, `Task_End_Time`
- `CPU_Utilization (%)`
- `Memory_Consumption (MB)`
- `Task_Execution_Time (ms)`
- `System_Throughput (tasks/sec)`
- `Task_Waiting_Time (ms)`
- `Number_of_Active_Users`
- `Network_Bandwidth_Utilization (Mbps)`
- `Job_Priority`, `Scheduler_Type`, etc.

---

## 📊 Analysis Performed

### 1. Scatter Plot: CPU Utilization vs. Error Rate

This analysis investigates the relationship between CPU usage and system error rate during task execution.

```python
plt.figure(figsize=(8,5))
sns.scatterplot(x='CPU_Utilization (%)', y='Error_Rate (%)', data=df)
plt.title('CPU Utilization vs. Error Rate')
plt.xlabel('CPU Utilization (%)')
plt.ylabel('Error Rate (%)')
plt.grid(True)
plt.show()


📈 Insight:
This scatter plot reveals potential correlations between high CPU load and increased error rates.

It aids in understanding performance bottlenecks and system behavior under various load conditions.


📦 Tools Used
Python

Pandas for data manipulation

Seaborn and Matplotlib for data visualization

Jupyter Notebook as the development environment

✅ Conclusion
This visual insight is useful for optimizing workload scheduling and ensuring cloud system reliability. Further exploration may include time-series analysis, resource allocation trends, and predictive modeling based on usage patterns.

📁 How to Use
Clone the repository

Open cloud_workload_analysis.ipynb in Jupyter

Run all cells to reproduce the analysis

🙋‍♂️ Author
Thendo Netshandama
Email: tnetshandama90@gmail.com
Location: South Africa