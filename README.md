# 🚀 AI Career Opportunity Assistant  

An AI-powered automation system that intelligently filters job and internship opportunities from emails using workflow automation and LLM-based evaluation.

<br>

## 📌 Overview  

In today’s job market, students receive a large number of job and internship emails, most of which are irrelevant, repetitive, or unstructured.  

This project automates the entire process by:
- Extracting job-related data from emails  
- Identifying valid opportunities  
- Matching them with user preferences  
- Storing only relevant results  

<br>

## ⚙️ System Architecture  

Email → Validation → AI Agent 1 → Condition Check → AI Agent 2 → Decision → Google Sheets  

<br>

## 🧠 Key Features  

- 📩 Automated email processing using Gmail trigger  
- 🤖 AI-based job data extraction  
- 🎯 Personalized filtering based on user profile  
- 💰 Salary-based decision logic (≥ 4 LPA for jobs)  
- 📊 Structured storage in Google Sheets  
- ⚠️ Edge case handling (empty emails, non-job content, multiple roles)  

<br>

## 🔍 How It Works  

### 1. Email Trigger  
- Captures incoming emails automatically  

### 2. AI Agent 1 (Extraction)  
- Identifies job/internship emails  
- Extracts structured data:
  - Company  
  - Role  
  - Salary  
  - Link  
  - Deadline  

### 3. Condition Filtering  
- Removes non-job emails  

### 4. AI Agent 2 (Relevance Check)  
- Matches job data with user profile  
- Outputs:
  - Relevance (true/false)  
  - Match score  
  - Reason  

### 5. Final Decision  
- Relevant → Stored in Selected Sheet  
- Not Relevant → Stored in Rejected Sheet  

<br>

## 📸 Project Screenshots  

### 🔹 Workflow (n8n Implementation)
![Workflow](assets/workflow_n8n.png)

<br>

### 🔹 Workflow Logic Flowchart
![Flowchart](assets/workflow_flowchart.png)

<br>

### 🔹 Selected Opportunities Output
![Selected](assets/selected_list.png)

<br>

### 🔹 Rejected Opportunities Output
![Rejected](assets/rejected_list.png)

<br>

### 🔹 Lean Canvas (Product Thinking)
![Lean Canvas](assets/lean-canvas.png)

<br>

## 🧪 Edge Case Handling  

The system handles:
- Empty emails  
- Non-job emails  
- Multiple opportunities in one email  
- Missing salary or deadline  
- Low-paying jobs (< 4 LPA)  

<br>

## 🛠️ Tech Stack  

- n8n (Workflow Automation)  
- OpenAI API (LLM Processing)  
- Gmail API (Email Input)  
- Google Sheets (Data Storage)  

<br>

## 📂 Project Structure  

```
ai-career-opportunity-assistant/
│
├── docs/           
├── assets/         
├── workflow/       
├── extras/         
└── README.md
```

<br>

## 📊 Results  

- Executed 100+ workflow runs for testing and validation  
- Reduced manual job filtering effort  
- Improved accuracy in identifying relevant opportunities  

<br>

## ⚠️ Limitations  

- Depends on API availability  
- Requires structured email content for best performance  
- Limited to email-based input sources  

<br>

## 🔮 Future Scope  

- Integration with LinkedIn and job platforms  
- Resume-based dynamic matching  
- Dashboard for analytics and tracking  
- Multi-user support  

<br>

## 👤 Author  

**Tripti Kumari**  
B.Tech CSE | Narula Institute of Technology  

- 📧 Email: vishwakarmap1305@gmail.com  
- 🔗 LinkedIn: https://www.linkedin.com/in/tripti-kumari-8b3abb253/  

<br>

## ⭐ Final Note  

> This project demonstrates how AI and automation can be combined to transform unstructured data into meaningful, actionable insights for smarter career decisions.
