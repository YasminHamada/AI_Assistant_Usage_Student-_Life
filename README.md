# 🎓 AI Assistant Usage – Student Life

By Yasmine Hamada

📅 September 2025

# 📊 Project Overview

This repository presents an end-to-end Business Intelligence (BI) solution developed using Microsoft Azure (Lakehouse + Warehouse + Power BI).

The project analyzes a dataset simulating 10,000 student sessions of interacting with AI assistants (like ChatGPT) for academic tasks.

It covers session behavior, student demographics, academic disciplines, AI effectiveness, and overall satisfaction—providing deep insights into how students use AI tools in education.

# 🛠️ Tech Stack
| Component | Technology |
| --------- | ---------- |
| Data Ingestion | Azure Data Factory |
| Lakehouse      | Azure Data Lake / Delta Lake |
| Warehouse      | Azure Synapse / Azure SQL DWH |
| Visualization | Power BI |
| Scripting | T-SQL, DAX |

# 📝 Data Description

The dataset contains 10,000 records of student-AI interaction sessions with details about session context, student levels, and AI usage effectiveness.

📂 Key Columns

 . 🆔 Session ID – Unique session identifier

 . 🎓 Student Level – High School, Undergraduate, Graduate

 . 📖 Discipline – Field of study (e.g., CS, Psychology, etc.)

 . 📅 Session Date – Date of the session

 . ⏱️ Session Length (Min) – Duration of AI interaction

 . 💬 Total Prompts – Number of AI prompts/messages used

 . 📝 Task Type – Nature of task (Coding, Writing, Research, etc.)

 . 🤖 AI Assistance Level – 1–5 scale (how helpful AI was)

 . 🎯 Final Outcome – e.g., Assignment Completed, Idea Drafted

 . 🔁 Used Again – Whether the student reused the AI tool

 . ⭐ Satisfaction Rating – 1–5 overall rating


# 📊 Project Layers

 1- 🗄️ Data Source Layer
 
      Raw dataset (CSV) with session details.
      
 2- 🏞️ Lakehouse (Bronze → Silver → Gold)
 
       . Bronze Layer (Raw): Ingest raw data in original format
       
       . Silver Layer (Cleaned): Apply transformations, cleaning, validation
       
       . Gold Layer (Curated): Business-ready tables for analytics

 3- 🏢 Data Warehouse – Star Schema 
 
     . Fact Table:
     
        Fact_Session

     . Dimensions:

       1- Dim Student Level

       2- Dim Discipline

       3- Dim Task Type

       4- Dim Final Outcome

       5- Dim Date

 4- 📦 Warehouse Analytics Model

     Created measures & KPIs in DAX:

     . Total Sessions
     
     . Total Prompts
     
     . Avg. Rating
     
     . Avg. Session Length

 5- 📈 Power BI Dashboard

    
<img width="904" height="514" alt="task _type_bi" src="https://github.com/user-attachments/assets/6306ed74-5b43-4437-b70f-2a923e74b88a" />





<img width="912" height="525" alt="session_level_bi" src="https://github.com/user-attachments/assets/6f56c7c9-afbe-40f9-9c23-ca17419eeeed" />





 <img width="898" height="514" alt="discipline" src="https://github.com/user-attachments/assets/b0557508-3db4-41ee-ac4d-7a7032a180ac" />
       
 
