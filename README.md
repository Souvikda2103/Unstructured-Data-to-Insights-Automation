# 📄 Unstructured Data to Insights Automation  
🔗 👉 Workflow: Automated Invoice Processing (Google Drive → OCR → AI → Google Sheets)

## 🎯 Objective  
To build an end-to-end automation system that reads **unstructured invoice files** (PDF & images) from Google Drive, extracts key information using **OCR + Google Gemini**, and updates Google Sheets with clean, structured data — eliminating manual entry, errors, and repetitive work.

---

## 🧾 What This Automation Does  
This workflow takes care of everything from file collection to structured data entry:

- Automatically scans invoice folder in Google Drive  
- Handles both **PDFs** and **image files**  
- Extracts text using **OCR** or file reader  
- Uses **AI (Google Gemini)** to pull out important fields  
- Cleans, validates, and formats the extracted data  
- Appends the output into two Google Sheets:  
  - **Invoice Details**  
  - **Invoice Items**

A single click = complete invoice processing. 🚀

---

## 🧠 Solution Breakdown

### **1. Workflow Trigger (Manual / Scheduled)**
Start the workflow with one click, or set it to run daily.

### **2. Locate Google Drive Folder**
Fetch all files from the invoices folder.

### **3. Loop Through Files**
Process documents one by one, just like manual review.

### **4. Format Detection**
Use a Switch to branch processing:
- PDF → Extract from File  
- PNG/JPG → OCR API  

### **5. Convert to Text**
- PDFs → File extract  
- Images → OCR.Space API  

### **6. AI-Based Information Extraction**
Pass extracted text to **Google Gemini** to generate JSON with fields like:
- Invoice number  
- Name  
- Amount  
- Date  
- Item list  

### **7. Clean & Validate**
- Remove invalid invoice files  
- Fix missing or inconsistent fields  
- Standardize formats (dates, numbers)

### **8. Append to Google Sheets**
- Invoice metadata → *Invoice Details* sheet  
- Item list → *Invoice Items* sheet  
- Add UID to prevent duplicate entries  

### **9. Final Output**
Clean, standardized, analysis-ready data.  
Zero manual effort.

---

## 💬 Conclusion  
This system transforms messy, unstructured invoice files into clean, structured data — completely automated and error-free.  
A practical use-case showing the power of AI + Automation in solving real business problems.

---

#AI #Automation #Codebasics #n8n #GoogleGemini #OCR #GoogleSheets #InvoiceAutomation #WorkflowAutomation #UnstructuredData #FinTech #ProductivityTools

