# 📄 Unstructured Data to Insights Automation  
🔗 👉 Workflow: Automated Invoice Processing (Google Drive → OCR → AI → Google Sheets)

---

## 🎯 Objective  
To build an end-to-end automation system that reads unstructured invoice files (PDF & images) from **[Google Drive](https://www.google.com/drive/)**, extracts key information using **OCR + [Google Gemini](https://ai.google.dev/)**, and updates **[Google Sheets](https://www.google.com/sheets/about/)** with clean, structured data — eliminating manual entry, errors, and repetitive work.

---

## 🧾 What This Automation Does  

This workflow takes care of everything from file collection to structured data entry:

- Automatically scans an invoice folder in **Google Drive**  
- Handles both **PDFs** and **image files**  
- Extracts text using **OCR** or file reader  
- Uses **Google Gemini** AI to extract structured fields  
- Cleans, validates, and formats the extracted data  
- Updates two Google Sheets:  
  - **Invoice Details**  
  - **Invoice Items**  

A single click = complete invoice processing. 🚀

---

## 🧠 Solution Breakdown  

### **1. Workflow Trigger (Manual / Scheduled)**  
Triggered manually or via schedule using **[n8n Automation](https://n8n.io/)**.

### **2. Locate Google Drive Folder**  
Fetch all files from the invoice storage folder in **Google Drive**.

### **3. Loop Through Files**  
Process documents one by one — similar to doing it manually, but fully automated.

### **4. Format Detection**  
Use a Switch node to branch processing paths:  
- **PDF → Extract from File**  
- **PNG/JPG → OCR API**

### **5. Convert to Text**  
- PDFs → Extract text via n8n file reader  
- Images → OCR conversion using **[OCR.Space API](https://ocr.space/ocrapi)**

### **6. AI-Based Information Extraction**  
Use **Google Gemini** to extract fields like:  
- Invoice number  
- Customer name  
- Amount  
- Date  
- Item list  

### **7. Clean & Validate**  
- Filter out invalid files  
- Standardize dates, numbers  
- Ensure clean, structured formatting  

### **8. Append to Google Sheets**  
- Invoice metadata → **Invoice Details**  
- Items list → **Invoice Items**  
- UID generated to avoid duplicates  

### **9. Final Output**  
- Clean, analysis-ready data  
- No manual effort  
- Always up-to-date Google Sheets  

---

## 💬 Conclusion  
This automation converts messy, unstructured invoice files into clean, structured, actionable data — **fully automated and error-free**.  

A powerful example of how **AI + Automation** can eliminate repetitive work and improve operational efficiency in real-world business workflows.

---

## 🔗 Useful Links  

- **n8n Automation Platform:** [https://n8n.io/  ](http://localhost:5678/workflow/oM9CDB3K8ZfhFuw3)
- **Google Drive:** [https://www.google.com/drive/  ](https://drive.google.com/drive/folders/1ruDVlJULqPnki-FWJOOXOuB8UFwwS-kA)
- **Google Sheets:** [https://www.google.com/sheets/about/  ](https://docs.google.com/spreadsheets/d/1F6aaQhVvg_hjTlrkoWp8dcoEqA5P2VRQfAfWPR7BblA/edit?gid=665692375#gid=665692375)  

---

#AI #Automation #Codebasics #n8n #GoogleGemini #OCR #GoogleSheets #GoogleDrive #InvoiceAutomation #WorkflowAutomation #UnstructuredData #FinTech #ProductivityTools
