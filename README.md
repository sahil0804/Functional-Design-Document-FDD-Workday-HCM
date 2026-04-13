# Workday HCM: Onboarding & IT Provisioning Automation

## 📌 Project Overview
This repository contains a simulated Workday HCM integration project demonstrating the end-to-end lifecycle of an HR technology rollout. It showcases the ability to translate complex HR business requirements into technical workflows, bridging the gap between functional design and data execution.

**Author:** Sahil Mehta  
**Role:** Business Analyst / Functional Lead  

## 🎯 The Business Problem
Many enterprise organizations suffer from disjointed onboarding processes where HR manually emails IT to provision accounts for new hires. This results in missing data, security risks, and costly Day-1 system access delays.

## 💡 The Solution
This project simulates the configuration and integration of the Workday "Hire" and "Onboarding Setup" Business Processes (BPs) to trigger automated downstream IT account provisioning. 

## 📂 Repository Structure
This repository is split into two core competencies: **Functional Design** and **Technical Integration**.

* 📄 **`Sahil_Mehta_Mock_FDD.pdf`** * The complete Functional Design Document.
    * Includes As-Is/To-Be process mapping, Jira User Stories with strict acceptance criteria, Workday Security Group models, and a RAID log.
* 📁 **`/data`** * `dummy_workday_export.xml`: Simulated Workday XML output of hired workers.
    * `it_provisioning_payload.json`: The final transformed data ready for API ingestion.
* 📁 **`/scripts`** * Python and XSLT scripts used to parse, transform, and clean the heavy Workday XML output into a lightweight, IT-friendly JSON payload.

## 🛠️ Skills & Technologies Demonstrated
* **Business Analysis:** Requirements Gathering, As-Is/To-Be Mapping, RAID Logs, Agile/Jira User Stories.
* **Workday HCM Concepts:** Business Processes (BPs), Core HCM, Onboarding Setup, Custom Reports/EIBs, Security Roles.
* **Data Transformation:** Python (Pandas), XML, XSLT, JSON, API payload structuring.

## 🚀 How to Run the Script
1. Clone the repository to your local machine.
2. Navigate to the `/scripts` directory.
3. Run `python wd_to_ad_sync.py` to watch the script extract the mock XML data, apply the business logic (filtering for future hires), and generate the JSON payload in the `/data` folder.
