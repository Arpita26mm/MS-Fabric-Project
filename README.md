![WhatsApp Image 2025-05-19 at 10 53 05 PM](https://github.com/user-attachments/assets/92814857-ad54-4a21-b1eb-b201977d9e70)

# PIPELINE CREATION IN MS-FABRIC

## Description📄:

This project showcases a fully UI-based data pipeline built using Microsoft Fabric. It automates the movement, transformation, and storage of CSV files from multiple sources (OneLake, GitHub) with no custom code. The final output is a structured table ready for reporting and analytics.

## ⭐ Features

### Automated File Handling
- **Triggered pipeline**: Activates when a new file is dropped into the OneLake source folder.
- **Copy & Delete**: Copies the file to a destination folder and deletes it from the source after a successful copy.
- **GitHub Integration**: Copies a second file from a public GitHub repository.

### Metadata & Conditional Flow
- **Get Metadata**: Retrieves metadata of all files in the destination folder.
- **If Condition Check**: Iterates through files to find a specific file by name.
- **Conditional Copy**: If the file is found, it's copied to the reporting folder.

### Data Transformation
- **Dataflow Activity**: Transforms the data file in the reporting folder.
- **Table Output**: Final transformed data is stored as a managed table at Tables/dbo/report.

### Nested Pipeline Execution
- **Invoke Pipeline Activity**: Used to trigger a sub-pipeline within the main pipeline for modular processing and reusability.

## 🛠️ Tools Used

- **Microsoft Fabric** (Data Pipeline, Dataflow)
- **OneLake**
- **GitHub** (as a source repository)

## ⚠️ Note
**This is a no-code UI project created entirely within Microsoft Fabric. This repository exists for:**
- **Documenting the pipeline design**
- **Sharing flow diagrams and descriptions**
- **Keeping a log of project structure and purpose**


## ✨ Preview

<p align="center">
  <img width="540" height="317.6" alt="Screenshot 2025-05-19 at 10 05 09 PM" src="https://github.com/user-attachments/assets/14d28625-f7ea-4954-9a3f-bfbb1213148f" />
</p>


