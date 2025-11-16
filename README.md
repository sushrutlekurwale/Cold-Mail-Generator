
# **Cold Mail Generator**

The **Cold Mail Generator** is an end-to-end GenAI application designed for service-based companies to create personalized cold emails for potential clients.
The system extracts job listings from a company’s Careers page, matches them with relevant portfolio items using a vector database, and generates tailored cold emails.

---

## 🚀 **Features**

* **Llama 3.3–powered email generation** for producing context-aware, professional cold emails.
* **Scrape job listings** directly from any Careers page URL.
* **Structured role parsing** to convert extracted job postings into clean, machine-readable descriptions.
* **ChromaDB vector search** for retrieving relevant portfolio/project links based on the job description.
* **Interactive Streamlit UI** for an easy, user-friendly workflow.


---

## 🏗️ **Architecture Overview**

1. User provides a **Careers page URL**.
2. App scrapes the page and extracts specific job listings.
3. Extracted job data is converted into **structured role descriptions**.
4. Relevant project/portfolio links are retrieved from **ChromaDB** using embeddings.
5. All context is fed into **Llama 3.1** to generate a polished, customized cold email.
6. Email is displayed in the **Streamlit interface**.



## 🛠️ **Setup Instructions**

### 1. **Clone the repository**

```bash
git clone https://github.com/your-username/cold-mail-generator.git
cd cold-mail-generator
```

### 2. **Set up environment variables**

Create a `.env` file inside the `app/` directory:

```
GROQ_API_KEY=your_api_key_here   # or your Llama model API key path
```

Get your API key from:
[https://console.groq.com/keys](https://console.groq.com/keys)

### 4. **Run the Streamlit app**

```bash
streamlit run app/main.py
```

---

## 📌 **Example Use Case**

**Scenario:**
Meesho is hiring a *Android Engineer*.
TechSoft, a software services company, wants to reach out with a targeted cold email offering dedicated engineering talent.

The BD representative enters Meesho’s Careers page URL.
The tool extracts the job listing, retrieves relevant portfolio samples from ChromaDB, and generates a tailored email instantly.

---


## 📜 **Screenshot**


