# ☁️ Cybersecurity Cloud Risk Analyst Internship: GSU Capstone

### **Role:** Lead Cloud Risk Analyst 
### **Client:** Georgia State University Cybersecurity Services Team
### **Duration:** Spring 2025 (Jan - April)
### **Tools:** AWS CloudShell, Prowler (CLI), Qualys TotalCloud, Microsoft Teams, Google Meets

---

## 📌 Project Executive Summary
Engaged as a Cybersecurity Cloud Risk Analyst to conduct a comprehensive **Cloud Security Posture Management (CSPM)** assessment of the Georgia State University AWS Sandbox environment. The objective was to identify security misconfigurations, validate compliance against federal standards, and deliver a strategic remediation plan to the GSU Cybersecurity Services Team.

Operating within a 5-person team, I facilitated the deployment of both open-source (**Prowler**) and enterprise (**Qualys TotalCloud**) scanning tools. We successfully identified critical vulnerabilities including **Identity and Access Management (IAM)** and **Storage (S3)**, mapped these findings to **NIST SP 800-171**, and presented a formal risk mitigation strategy to client stakeholders.

---

## 🛠️ Technical Implementation & Methodology

### 1. Automated Vulnerability Scanning (CSPM & CNAPP)
We utilized a dual-tool approach to ensure comprehensive coverage of the AWS environment.
* **Prowler Deployment (CLI-Based):**
    * Executed Prowler via **AWS CloudShell** using Linux command-line interface.
    * Overcame technical challenges regarding ephemeral CloudShell sessions by automating installation scripts for each assessment session.
    * Generated JSON and CSV reports analyzing thousands of data points across the AWS infrastructure.
* **Qualys TotalCloud (GUI-Based):**
    * Deployed Qualys agents to monitor runtime security and compliance.
    * Contrasted findings between Prowler (infrastructure focus) and Qualys (workload focus) to eliminate false positives.

### 2. Framework Cross-Walking & Compliance Mapping
A major challenge identified during the project was that **Qualys TotalCloud** did not provide native mapping to our required standard, **NIST SP 800-171**.
* **Manual Control Mapping:** I led the initiative to manually cross-reference Qualys technical findings to **NIST SP 800-171 Rev. 2** control families.
* **Multi-Framework Alignment:** Successfully mapped single technical failures (e.g., Lack of MFA) across multiple regulatory standards to demonstrate the "ripple effect" of non-compliance:
    * **NIST SP 800-171:** Controls 3.1.1, 3.5.3 (Access Control & Authentication)
    * **NIST SP 800-53:** AC-2, IA-2
    * **ISO/IEC 27001:2013:** A.9.2
    * **SOC 2:** CC 6.1

### 3. Risk Calculation & Matrix Development
To translate technical jargon into business intelligence, we developed a custom **4x4 Risk Matrix**.
* **Methodology:** Calculated risk using the formula `Risk = Likelihood × Impact`.
* **Scoring System:** Findings were categorized as *Critical, High, Medium, or Low*.
* **Strategic Prioritization:** This matrix allowed the client to visualize which vulnerabilities posed an immediate threat to the university's data integrity vs. those that were acceptable operational risks.

---

## 🚨 Key Findings & Remediation

During the assessment, we identified several critical security gaps. Two notable examples included:

### Finding 1: Lack of MFA on Root Account (Critical)
* **The Risk:** The AWS Root Account is the most privileged identity. Without Multi-Factor Authentication (MFA), a compromised password grants attackers unrestricted access to deal big-time damage,such as delete resources or steal data.
* **Compliance Violation:** Failed **NIST 800-171 Control 3.5.3** (Use of multifactor authentication for local and network access).
* **Remediation Recommendation:** Implementation of hardware keys (YubiKey) or virtual MFA devices (Google Authenticator) for all privileged accounts.

### Finding 2: S3 Bucket Public Access Block Not Enabled (High)
* **The Risk:** "Block Public Access" was disabled at the account level. This misconfiguration increases the likelihood of accidental data leaks where sensitive PII could be exposed to the public internet.
* **Compliance Violation:** Failed **NIST 800-171 Control 3.1.3** (Control the flow of CUI in accordance with approved authorizations).
* **Remediation Recommendation:** Enable "Block Public Access" at the account level and implement bucket policies denying `Principal: *`.

---

## 🧠 Challenges Overcome

* **Tool Limitation Workarounds:** When Qualys failed to provide the necessary regulatory context, I did not wait for someone else to do it; I researched the control families and performed the mapping manually to ensure the client received accurate compliance data.
* **Technical Environment Constraints:** Prowler required consistent re-configuration in the AWS CloudShell environment. We optimized our setup process to reduce downtime during weekly assessment windows.
* **Team Coordination:** Held a 100% attendance rate in weekly meetings with the team/client to ensure all deliverables were ready for the client presentation deadlines.

---

## 📂 Project Artifacts

Below are the documents and presentations delivered to the Georgia State University Cybersecurity Team:

* **📄 Executive Summary:** [View Executive Summary](images/Executive Summary - GSU Cybersecurity Team copy.docx.pdf)
* **📊 Final Client Presentation:** [View PowerPoint Slides](Cloud_Risk_Assessment_Team_Presentation.pptx)
* **📝 Deep Dive: NIST 800-171 Finding:** [View Technical Finding Report](AWS_Prowler_Failed_Finding/NIST_800-171_Deepdive)
* **📅 Project Schedule:** [View Project Timeline](Weekly_CIS_4980_Spring_2025_Capstone_Schedule_with_GSU_Cybersecurity_Team.xlsx_-_Sheet1.csv)

---

## 💡 Skills & Competencies Demonstrated

| Technical Skills | GRC & Strategy | Soft Skills |
| :--- | :--- | :--- |
| **AWS Cloud Security** (IAM, S3, VPC) | **NIST RMF & 800-171** | **Executive Presentation** |
| **Linux CLI** (Bash, Shell Scripting) | **ISO 27001 & SOC 2** | **Client Relationship Mgmt** |
| **Vulnerability Scanning** (Prowler, Qualys) | **Risk Scoring & Matrices** | **Technical Writing** |
| **Python** (Script execution) | **Compliance Mapping** | **Team Leadership** |

---

[Back to Projects](Projects.md)

[Back to Main Portflio Home](index.md)
