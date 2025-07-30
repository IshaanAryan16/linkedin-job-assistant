# 💼 LinkedIn Job Application Assistant
**Your AI-Powered Job Hunting Companion**

Created as a Master's project for the GenAI module, this assistant transforms the often-tedious job application process into an automated, intelligent, and highly personalized experience. 
The modern job market is nothing short of a cut-throat battle between gladiators in the 
Colosseum, it has become more competitive than ever. With the ever-rising layoffs in the 
technology industry (or any industry affected by the sudden rise of the new age gold 
rush, GenerativeAI), a constant influx of skilled candidates (1000+ applicants for a role 
in a matter of minutes), and companies resorting to the use of AI-driven Applicant 
Tracking Systems (ATS) to match ideal candidates quickly, job seekers face a constant 
uphill battle. Submitting generic resumes (that the applicants created once, that too 
months ago) is not enough anymore, applications must be tailored exactly to what the 
job entails to pass the dreaded automated screening process to get a chance to stand out 
to the hiring managers. This challenge is even more harsh for Software engineers and 
other technical professionals, as roles demand specific skills that align with the job 
listed (eg, Kubernetes and Docker expertise for DevOps positions). The question is, if the 
ATS is getting smarter (AI-enabled), why shouldn’t the applicant? 

## 🚀 What It Does

This AI-powered agent takes the pain out of job applications by automating and enhancing every key step in the process:

### 🔎 Finds Relevant Jobs
Uses a custom LinkedIn scraper to continuously find new job listings tailored to the user's criteria (e.g., "Software Engineer in Ireland").

### 📊 Job Scoring & Matching
Automatically compares your CV with each job description using RAG (Retrieval-Augmented Generation) and assigns an Employability Score (1–10), complete with rationale.

### ✍️ Generates Custom Cover Letters
For high-scoring jobs, it drafts tailored cover letters using your real experiences and job keywords.

### 📝 Edits Your CV Dynamically
Uses a code interpreter to adjust your resume formatting and content to match the specific requirements of a job, exporting professionally formatted .docx files.

### 📂 Outputs Everything
Generates a CSV file containing:
- Job details
- Scores
- Cover letters
- CV edit suggestions
- Downloadable tailored resumes

## 🧠 How It Works

Under the hood, the assistant combines multiple OpenAI API capabilities and custom tools:

| Component | Role |
|-----------|------|
| 🧾 **File Search** | Ingests and semantically indexes your CV for personalized matching |
| 🔧 **Function Calling** | Scrapes LinkedIn in real-time & scores jobs |
| 🧠 **RAG** | Compares job descriptions to your CV using embeddings |
| 🧑‍💻 **Code Interpreter** | Edits and exports custom .docx CVs, preserving formatting |
| 🧵 **Threads API** | Keeps conversation context across interactions |

## 📚 Prerequisites

To run this project locally or build upon it, you'll need:

- Python 3.10+
- OpenAI API Key
- LinkedIn Job Scraper (or similar)
- Required Python packages:

```bash
pip install openai python-docx pandas beautifulsoup4
```

- Valid .docx or .pdf resume

> **Note:** This project does not use ChatGPT's frontend. It leverages the OpenAI Assistants API, which provides persistent, thread-based interactions and access to API tools.


## 🧪 Sample Workflow

1. Upload your CV in .pdf or .docx
2. Agent scrapes jobs (location/role defined by you)
3. Jobs are scored and ranked
4. Cover letters and CV edits are generated
5. Customized .docx CVs are exported and stored
6. Everything is saved to a structured CSV for tracking

## 🌟 Why It's Better Than ChatGPT

| Feature | ChatGPT | This Assistant |
|---------|---------|----------------|
| **CV Personalization** | Manual | Full CV awareness via file search |
| **Job Matching** | Hypothetical | Live LinkedIn scraping + scoring |
| **Output Format** | Plain Text | Downloadable .docx, scores, and CSV reports |
| **Automation** | User-driven | Fully autonomous pipeline (scraping → editing) |
| **Precision** | Generic Advice | Tailored feedback + skill-highlight recommendations |

## 📈 Future Improvements

- Add job scrapers for Indeed, IrishJobs.ie
- Integrate salary benchmarking APIs
- Build interview simulation and study plans
- Introduce human-in-the-loop CV suggestions
- Recommend courses or skills based on job trends

## 📖 Report

A full technical breakdown is available in `24222333_GenAI_Report.pdf`, covering:
- Assistant design flow
- Tool orchestration
- Prompt engineering
- Examples with screenshots
- Technical decisions & bibliography

## 🙏 Acknowledgements

**Project created by Ishaan Aryan**  
MSc in Computer Science, UCD  
Contact: ishaan.aryan16@gmail.com
