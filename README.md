# MCP-Based Lead Qualification Chatbot (n8n)

## 📌 Project Overview
This project is an AI-powered **Lead Qualification Chatbot** built using **n8n**, **MCP Client–Server architecture**, and **Google Gemini AI**.  
The chatbot interacts with users, qualifies real-estate leads, schedules site visits, and stores lead data automatically in Google Sheets.

---

## 🧠 Key Features
- AI-driven conversational chatbot
- MCP Client–Server integration
- Lead qualification (BHK preference, time, confirmation)
- Site visit scheduling
- Automatic lead storage in Google Sheets
- Memory-enabled conversation handling

---

## 🏗️ Architecture

User Chat

↓

n8n Trigger (Chat Message)

↓

AI Agent (Google Gemini + Memory)

↓

MCP Client

↓

MCP Server

↓

Google Sheets (Lead Storage)

---

## ⚙️ Tech Stack
- **n8n**
- **Google Gemini Chat Model**
- **MCP Client & MCP Server**
- **Google Sheets**
- **AI Agent with Memory**

---

## 📂 Project Structure

MCP_Lead_Qualification_Chatbot/

├── workflows/

├── screenshots/

├── README.md


---

## 🔄 Workflows

### 1️⃣ MCP Client – Lead Qualification
- Receives user chat
- Uses AI Agent for conversation
- Collects:
  - Name
  - Mobile number
  - Apartment type
  - Site visit time
- Sends data to MCP Server

📸 Screenshot:
![Client Workflow](workflows/client_workflow.png)

---

### 2️⃣ MCP Server – Lead Storage
- Receives structured lead data
- Appends lead details to Google Sheets

📸 Screenshot:
![Server Workflow](workflows/server_workflow.png)

---

## 🧪 Sample Chat Flow
📸 Chat confirmation example:
![Chat Flow](screenshots/chat_confirmation1.png)
![Chat Flow](screenshots/chat_confirmation2.png)
![Chat Flow](screenshots/chat_confirmation3.png)
![Chat Flow](screenshots/chat_confirmation4.png)
![Chat Flow](screenshots/chat_confirmation5.png)
![Chat Flow](screenshots/chat_confirmation6.png)

---

## 📊 Output (Google Sheets)
All qualified leads are stored automatically.

📸 Example:
![Google Sheet](screenshots/google_sheet_output.png)

---

## 🚀 How to Use
1. Import JSON workflows into n8n
2. Configure:
   - Google Gemini API
   - Google Sheets credentials
3. Activate both workflows
4. Start chatting with users

---

## 🎯 Use Cases
- Real estate lead qualification
- Appointment scheduling bots
- Sales automation
- CRM data collection

---

## 👨‍💻 Author
**Prajwal Mavkar**  
Aspiring Data Analyst | AI & Automation Enthusiast
