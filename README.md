# Reddit Persona Generation Assignment

## 📌 Project Overview

This project demonstrates a pipeline to **extract user data from Reddit** and generate detailed user personas for UX research and marketing insights.

────────────────────────────────────────────

## ⚙️ Implementation Methods

### 🔷 **Method 1: Full Automation (Extract Data + Generate Image via Code)**

✅ **Steps:**

1. Run the script:

   python main.py <reddit_profile_url>

2. The script will:

- Extract the username from the URL.
- Scrape posts and comments via Reddit API (`praw`).
- (If API quota available) Generate the persona summary using **OpenAI GPT** directly in code.
- Insert the persona details into a **pre-designed template PNG image** using `PIL`.
- Save the final persona as an **automatically generated PNG image** for direct submission.

✔️ **Requirement:** Active OpenAI API key with sufficient quota.

────────────────────────────────────────────

### 🔷 **Method 2: Semi-Automated (Extract Data via Code + Generate Persona via ChatGPT)**

✅ **Steps:**

1. Run your code to **extract Reddit user data only**:

   user_data = get_user_data(username)
   print(user_data)

2. Copy the **printed user data output**.

3. Paste it into **ChatGPT** using the prompt below to generate the persona details.

4. Insert the generated persona details manually into your **Canva template** to create the final PNG output for submission.

✔️ **Use Case:** This method is used when **OpenAI API quota is limited** but Reddit data extraction via code is mandatory to demonstrate programming skills.

────────────────────────────────────────────

### 📝 Persona Prompt for ChatGPT

You are an AI persona builder. Based on the following Reddit user data, generate:

1. Name
2. Age (if inferred)
3. Occupation (if inferred)
4. Status
5. Location (if inferred)
6. Tier / Archetype
7. Personality Traits
8. Motivations
9. Behaviour & Habits
10. Frustrations
11. Goals & Needs

Cite posts/comments if relevant. If information is not available, mention 'Not available'.

[PASTE USER DATA HERE]

────────────────────────────────────────────

## 💻 Dependencies (requirements.txt)

praw  
openai  
pillow

Install using:

   pip install -r requirements.txt

────────────────────────────────────────────

## 📄 Submission Contents

✅ `LLMproject.ipynb` – Reddit scraping and persona generation logic   
✅ `README.md` – this file  
✅ **Final persona image (PNG)** – created via Method 1 (code) or Method 2 (ChatGPT + Canva)

────────────────────────────────────────────

## 🚀 Future Scope

- Automate persona image generation fully using Python (`PIL`) with design templates.
- Extend to multiple Reddit users to build aggregated user archetypes.
- Integrate Canva API for direct automated persona image creation.

────────────────────────────────────────────

## ✨ Author

**Name:** [NAYEEM]  
**Email:** [nayeemfawaz30@gmail.com]  


────────────────────────────────────────────

### 📌 Note

This project demonstrates my skills in **API integration, data extraction, persona analysis, and visual design workflows** essential for data-driven UX research and marketing applications.

────────────────────────────────────────────
