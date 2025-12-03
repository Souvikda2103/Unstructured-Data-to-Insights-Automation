# 📄 Unstructured Data to Insights Automation  
🔗 👉 Workflow: Automated Invoice Processing (Google Drive → OCR → AI → Google Sheets)

---

## 🎯 Objective  
To build an end-to-end automation system that reads unstructured invoice files (PDF & images) from Google Drive, extracts key details using OCR + Google Gemini, and updates Google Sheets with clean, structured data — eliminating manual entry, errors, and repetitive work.

---

## 🧾 What This Automation Does  

This workflow fully automates the journey from raw invoice files to structured data:

- Automatically scans an invoice folder in **Google Drive**  
- Handles **PDF** and **image (PNG/JPG)** formats  
- Extracts text using either File Reader or OCR  
- Uses Google Gemini to pull out structured fields  
- Validates and cleans extracted data  
- Updates two Google Sheets:
  - **Invoice Details**
  - **Invoice Items**

✨ A single click processes all invoices end-to-end.

---

## 🧠 Solution Breakdown  

### 1️⃣ Workflow Trigger  
Triggered manually or on schedule using n8n.

### 2️⃣ Locate Google Drive Folder  
Fetches all invoice files from the selected Drive folder.  
🔗 Your Folder:  
https://drive.google.com/drive/folders/1ruDVlJULqPnki-FWJOOXOuB8UFwwS-kA

### 3️⃣ Loop Through Files  
Processes every document — similar to manual review, but fully automated.

### 4️⃣ Format Detection  
Uses Switch logic to detect:
- **PDF → Extract from File**
- **PNG/JPG → OCR API**

### 5️⃣ Convert to Text  
- PDFs → Extract text directly  
- Images → OCR using OCR API

### 6️⃣ AI-Based Information Extraction  
Google Gemini extracts:
- Invoice number  
- Customer name  
- Date  
- Amount  
- Item list  

### 7️⃣ Clean & Validate  
- Filters out invalid files  
- Cleans and standardizes data  
- Repairs missing or inconsistent fields  

### 8️⃣ Append to Google Sheets  
Updates your Google Sheets automatically:

🔗 Invoice Sheet:  
https://docs.google.com/spreadsheets/d/1F6aaQhVvg_hjTlrkoWp8dcoEqA5P2VRQfAfWPR7BblA/edit?gid=665692375#gid=665692375

- Invoice details → Invoice Details sheet  
- Item list → Invoice Items sheet  
- UID generated to avoid duplicates  

### 9️⃣ Final Output  
- Clean, structured data  
- Fully automated  
- Always up to date  

---

## 💬 Conclusion  
This automation transforms messy, unstructured invoice files into clean, structured insights — **completely automated and error-free**.  
A great example of how AI + Automation removes repetitive work and increases operational efficiency.

---

## 🔗 Useful Links  
- **n8n Automation Workflow:** http://localhost:5678/workflow/oM9CDB3K8ZfhFuw3  
- **Google Drive Folder:** https://drive.google.com/drive/folders/1ruDVlJULqPnki-FWJOOXOuB8UFwwS-kA  
- **Google Sheet:** https://docs.google.com/spreadsheets/d/1F6aaQhVvg_hjTlrkoWp8dcoEqA5P2VRQfAfWPR7BblA/edit?gid=665692375#gid=665692375  

---

#AI #Automation #Codebasics #n8n #GoogleGemini #OCR #GoogleSheets #GoogleDrive #InvoiceAutomation #WorkflowAutomation #UnstructuredData #FinTech #ProductivityTools

#AI #Automation #Codebasics #n8n #GoogleGemini #OCR #GoogleSheets #GoogleDrive #InvoiceAutomation #WorkflowAutomation #UnstructuredData #FinTech #ProductivityTools
