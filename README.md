# Salesforce Permissions Tools

> **Advanced toolkit to simplify management, auditing, and synchronization of Salesforce security metadata.**

[![Status](https://img.shields.io/badge/Status-Active-success)]() [![Stack](https://img.shields.io/badge/Python-Streamlit-blue)]() [![Castellano](https://img.shields.io/badge/Lang-Castellano-red)](README_ES.md)

**Salesforce Permissions Tools** is a utility suite designed for Salesforce administrators and architects who need to go beyond standard Setup limitations. It offers a **Modern Graphical Interface (GUI)** for mass operations that would typically require complex scripts or manual XML editing.

> ⚠️ **Note:** This repository is a **public demonstration** (Landing Page) for the `Salesforce-Tools` project. The source code and automation scripts are kept in a private repository.

---

## 🚀 Key Features

### 1. 🖥️ Graphical Interface (GUI)
Forget the command line. A clean web-based interface (built with Streamlit) that allows you to:
- Select SFDX-connected orgs.
- Visualize progress bars for mass operations.
- Download reports and backups in Markdown/JSON instantly.

### 2. 🔄 Permissions Synchronization (`Sync View`)
Synchronize **View All** and **Modify All** permissions between environments (e.g., Prod -> UAT) with surgical precision.
- **Intelligent Diff**: Detects what is missing and deploys only what is necessary.
- **Categorization**: Automatically distinguishes between Standard, Custom, and Managed Package objects.
- **Dry-Run Mode**: Simulates changes before deploying to avoid production errors.

### 3. 🤔 Bulk Editor
- **Grid Editing**: Modify thousands of permissions (CRUD+FLS) in an Excel-like interface.
- **Advanced Filters**: Hides noise from unused standard objects.
- **Smart Deploy**: Automatic generation of `package.xml` and destructive/additive deployment as needed.

### 4. 🔍 Auditing & Security
- **Profile Comparator**: Visualize permission differences side-by-side (✅ vs ❌).
- **Connected Apps Monitor**: Detects and revokes dangerous OAuth sessions (e.g., Workbench in Prod).
- **Named Credentials Scan**: Alerts if a Sandbox has credentials pointing to Production endpoints.
- **Activity Auditor**: Login history analysis to detect unused licenses.

### 5. 🚑 Apex Doctor
- **AI Diagnosis**: Analyzes exception logs and automatically diagnoses the root cause.
- **Source Map**: Downloads relevant code from the Org to show the error context.

---

## 🛠️ Tech Stack

The tool is built prioritizing portability and security:

- **Core**: Python 3.9+
- **GUI**: Streamlit (Web-based local interface)
- **Integration**: Salesforce CLI (`sf`) for authentication and deployments.
- **Deployment**: Docker-ready for execution on servers or CI/CD pipelines.

---

## 🏭 Use Cases

1.  **Pre-GoLive Audit**: Verify that UAT and PROD have the same critical permissions.
2.  **Technical Cleanup**: Identify obsolete or empty profiles and permission sets.
3.  **Security**: Detect data leaks or insecure configurations in Sandboxes.

---

## 📬 Access and Contact

This toolkit is a proprietary solution developed to optimize Salesforce DevOps operations.

If you are interested in using these tools in your organization or seeing a technical demo:

- **Email**: [sergiogonzalezhidalgo@gmail.com](mailto:sergiogonzalezhidalgo@gmail.com)
- **GitHub**: [@SergioXp](https://github.com/SergioXp)

---

## 👤 Author

**Sergio González Hidalgo**
- 📧 [sergiogonzalezhidalgo@gmail.com](mailto:sergiogonzalezhidalgo@gmail.com)
