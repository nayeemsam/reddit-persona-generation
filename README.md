
# Reddit Persona Generation Assignment

## 📌 **Project Overview**

This project demonstrates a pipeline to **extract user data from Reddit** and generate detailed user personas in a structured visual format. The task involved:

1. **Scraping user data** via Reddit API using Python.
2. Generating **persona summaries** using GPT-based persona logic.
3. **Presenting output** as a visual persona image for UX research or marketing design.

---

## ⚙️ **Implementation Details**

### ✅ **1. Code Functionality**

- **`main.py`**:
  - Uses `praw` to fetch Reddit user posts and comments.
  - Extracts user data and formats it for persona analysis.
  - Contains a `generate_persona()` function that uses OpenAI GPT to build personas.

### ✅ **2. Limitations**

Due to **OpenAI API quota limitations** on my account:

- The `generate_persona()` function could not be executed via API for all users.
- Instead, I followed the alternative recommended approach:

  1. **Ran my Python code** to extract user Reddit data.
  2. **Created a structured GPT prompt** with the extracted data to generate persona summaries via ChatGPT web interface.
  3. **Designed the final persona image** manually using Canva, following the same prompt logic as implemented in code.

---

## 📄 **Alternative Approach Details**

✔️ Extracted Reddit user data via:

```python
user_data = get_user_data(username)
print(user_data)
