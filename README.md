🤖 AI-Powered CV Screening & Candidate Management System

An automated CV screening system built using n8n, Google Gemini (LLM), Gmail API, and Google Sheets.
This workflow collects candidate applications, analyzes resumes using AI, assigns a rating, stores candidate data, and automatically notifies both HR and the applicant.

🚀 Features

📄 Accepts candidate applications via web form

📎 Upload and parse PDF resumes

🧠 AI-based resume analysis & scoring

📊 ATS-style compatibility scoring (1–10 + score out of 100)

📑 Automatically logs candidates into Google Sheets

📧 Sends confirmation email to candidate

📬 Notifies HR with candidate details and AI rating

🛠 Tech Stack

n8n – Workflow automation

Google Gemini 1.5 Flash – Resume analysis

Gmail API – Automated email notifications

Google Sheets API – Candidate data storage

PDF Extract Node – Resume text extraction

🔄 Workflow Overview
1️⃣ Application Form (Webhook Trigger)

Candidates submit:

Full Name

Email

Expected Salary

LinkedIn

Resume (PDF)

2️⃣ Resume Processing

Extracts text from uploaded PDF.

Sends resume content to Gemini LLM for analysis.

3️⃣ AI Evaluation

The model generates:

Compatibility Rating (1–10)

ATS Score (out of 100)

Interview Recommendation

Response limited to 75 words.

4️⃣ Data Storage

Candidate details + AI rating are automatically appended to Google Sheets.

5️⃣ Email Automation

📧 Confirmation email sent to candidate.

📩 Notification email sent to HR with full details + AI rating.

🧠 AI Prompt Logic

The system:

Limits response to 75 words

Evaluates resume against Software Engineer job description

Outputs structured scoring and recommendation

Ensures concise and HR-ready feedback

📊 Google Sheets Structure

The following fields are stored:

Full Name

Email

Expectation

LinkedIn

CV Filename

AI Rating

⚙️ Setup Instructions

Install and configure n8n.

Import the workflow JSON.

Connect credentials:

Google Gemini API

Gmail OAuth

Google Sheets OAuth

Update:

HR email address

Google Sheets document ID

Activate workflow.

Share the form webhook URL for applications.

🎯 Use Cases

Automated HR pre-screening

Startup hiring pipeline

Internal recruitment automation

AI-assisted ATS scoring

Resume filtering before interviews

🔮 Possible Improvements

Add multi-role job description selection

Add resume keyword highlighting

Store parsed resume text in database

Add rejection email automation

Add dashboard for HR analytics

Add bias-checking layer

📄 License

This project is open-source and available under the MIT License.



Make a recruiter-friendly project description

Generate an architecture diagram
