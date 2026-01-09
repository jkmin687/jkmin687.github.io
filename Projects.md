---
layout: default
title: Projects
---

### [Home](index.md) | [About Me](AboutMe.md) | [Resume](documents/Full_Resume.pdf) | [Professional Statement](Professional_Statement.md)

---

# 📂 Projects, Programs, Experience, and Certifications

This page represents my passion and dedication to cybersecurity, showcasing a collection of projects, hands-on labs, and professional programs that have helped shape my journey. Each project has provided me with the opportunity to dive deeper into cybersecurity principles, gain practical, real-world experience, and sharpen my technical skills. From formal training initiatives to independent explorations, this portfolio reflects my growth as I pursue my goal of becoming a skilled cybersecurity professional.

As you explore this page, you’ll find the highlights of programs I’ve completed, projects I’ve worked on, and labs where I’ve challenged myself to continuously learn and improve upon my skills. I’ve also included links to reports, datasets, and presentations to give you more insight into my work. I hope you enjoy following along on my journey as much as I’ve enjoyed living it—thank you for visiting!

---

## Table of Contents
- [Programs & Internships](#programs-and-internships)
  - [Cybersecurity Cloud Risk Analyst Internship (AWS)](#aws-project)
  - [Deloitte Cyber Program](#deloitte)
  - [PwC Cybersecurity Consulting (SOX Audit)](#pwc-cybersecurity)
  
- [Technical Projects](#projectsactivities)
  - [ServiceNow GRC: Automated NIST ComplianceGuard Dashboard](#servicenow)
  - [University of California Maturity Assessment](#ucnistcsf)
  - [Web Development: CodePath Intro to Web Dev](#codepath)
 
- [Certifications](#certifications)
  - [CompTIA Security+ Certification](#certifications)

---

<a name="programs-and-internships"></a>
## Programs & Internships

<a name="aws-project"></a>
### GSU Cybersecurity Cloud Risk Analyst Internship
[View Full Report](Cyber_Risk_Internship.md)
   - Served as a **Cloud Risk Analyst** responsible for assessing the security posture of a simulated **AWS environment** handling Controlled Unclassified Information (CUI).
   - **Executed Automated Vulnerability Scans** using **AWS Prowler** and **Qualys TotalCloud**, analyzing thousands of lines of JSON output to identify critical misconfigurations such as open S3 buckets and lack of MFA on root accounts.
   - **Performed Framework Mapping**, translating technical scan findings into **NIST SP 800-171** control gaps (e.g., Mapping "MFA Missing" to *Control 3.5.3*).
   - **Developed a Risk Register**, calculating risk scores based on likelihood and impact, and assigning severity levels (Critical/High/Medium/Low) to guide executive remediation prioritization.
   - **Cross-Walked Compliance Standards**, demonstrating how the identified NIST gaps also resulted in non-compliance with **ISO 27001** and **SOC 2** requirements.

<a name="deloitte"></a>
### Deloitte Cyber Program
[View Full Report](programs/Deloitte_Cyber_Program.pdf)
   - Served as a Cybersecurity Analyst investigating the **web activity logs** of a suspected security breach.
   - Conducted **Behavioral Traffic Analysis** on server logs to distinguish between legitimate human users and automated bots, specifically identifying headless browsing patterns where API data was queried without dashboard resources needed to display data.
   - Identified the anomaly a specific User ID that exhibited a mechanical "heartbeat" signature, executing requests at the exact same second every hour (e.g., XX:00:48).
   - Analyzed session persistence, discovering a "zombie script" that continued to query the system for 16 hours despite receiving consecutive 401 Unauthorized errors, indicating non-human user traits.

<a name="pwc-cybersecurity"></a>
### PwC Cyber Security Consulting Program: SOX & ITGC
[View Full Report](programs/PwC_Cyber_Security_Consulting_Program.pdf)
   - Served as a **Cyber Security Consultant** assessing a client's **Procure-to-Pay (P2P) Standard Operating Procedures (SOP)** lifecycle against **Sarbanes-Oxley (SOX)** compliance requirements.
   - **Conducted Segregation of Duties (SoD) Analysis**, identifying a critical control failure where a single user possessed the ability to both *create* a vendor and *process* payments, creating a high risk for fraud.
   - **Executed Test of Design (ToD)** and **Operating Effectiveness (OE)** testing on IT General Controls (ITGCs), specifically reviewing Change Management logs and Access Control lists.
   - **Drafted an Audit Deficiencies Report**, clearly documenting the "Condition, Criteria, Cause, and Effect" of the identified failures.
   - **Presented Strategic Remediation Plans** to the Audit Committee, recommending the implementation of Role-Based Access Control (RBAC) to resolve the SoD conflicts.

---

<a name="projectsactivities"></a>
## Technical Projects

<a name="servicenow"></a>
### ServiceNow GRC: Automated "NIST ComplianceGuard" Application
[View Full Report](programs/ServiceNow_ComplianceGuard_Dashboard.pdf.pdf)
   - Engineered a custom Governance, Risk, and Compliance (GRC) Application within ServiceNow, migrating an organization from static Excel spreadsheets to an automated system of record based on the **NIST SP 800-53** framework.
   - **Architected the Database Schema** by extending the core Task table to ensure audit trail inheritance and executed ETL (Extract, Transform, Load) operations to normalize raw data using Transform Maps and Coalescing strategies.
   - Reduced **Mean Time to Respond (MTTR)** to critical compliance failures by **99%** (cutting reaction time from ~24 hours to <5 seconds) by implementing **Server-Side Logic** and **Flow Designer** workflows that instantly trigger remediation incidents.
   - Conducted **User Acceptance Testing (UAT)** via a "Smoke Test" simulation (SIM-999), verifying that a control failure immediately triggered the automated remediation workflow and alert system.
   - **Designed a "CISO Command Center" Dashboard**, providing executives with real-time visualization of the organization's security posture through **Compliance Overview** charts and **Critical Action Item** lists.

<a name="ucnistcsf"></a>
### University of California NIST CSF Maturity Assessment
[View Full Report](programs/UC_NISTCSF.md)
   - Conducted a Policy-to-Framework Traceability Audit, mapping the University of California System’s comprehensive security policy library against all **108 Subcategories of the NIST Cybersecurity Framework (CSF) v1.1.**
   - Executed a **Quantitative Maturity Assessment** utilizing the **National Cyber Security Review (NCSR) methodology**, assigning maturity scores (Scale 1-7) to evaluate the "Test of Design" for controls across the Identify, Protect, Detect, Respond, and Recover functions.
   - Developed a **Gap Analysis Dashboard** on Microsoft Excel, creating color-coded visualizations to immediately highlight critical policy deficiencies versus areas of optimized process maturity.
   - Engineered a scalable control matrix, structuring the data to be **"cross-walkable"** to other regulatory standards (e.g., ISO 27001 and NIST SP 800-53), allowing for "test once, comply many" audit efficiency.
   - Performed Open-Source Intelligence (OSINT) Analysis, simulating a third-party risk assessment by evaluating the organization's security posture strictly through publicly available governance documentation

<a name="codepath"></a>
### CodePath Intro to Web Development Project
[View Full Report](programs/Codepath_Web101.md)
   - Completed an intensive 10-week **Intro to Web Development** course, gaining foundational knowledge in developing a function website from the bottom-up.
   - **Developed a Responsive Website** utilizing **HTML, CSS, and JavaScript**, ensuring cross-browser compatibility and mobile responsiveness.
   - **Implemented API Integrations**, fetching data from external sources to display dynamic content to the user.

---

<a name="certifications"></a>
## Certifications

  - [CompTIA Security+ Certification](images/CompTIA_Security+_Certificate.pdf)

---

[Back to Main Portfolio](index.md)

---
