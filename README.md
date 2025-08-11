# Automated Meeting Assistant

**Problem:** Meetings are essential, but notes are often messy and important action items get lost. This wastes time and creates a lack of accountability.

**Solution:** This tool uses a powerful Large Language Model via the Hugging Face API to turn a raw meeting transcript into a concise summary and a clear, actionable checklist. This provides instant clarity and ensures nothing is forgotten.

---

### Key Features
*   **Concise Summarization:** Get the key points of a long meeting in seconds.
*   **Action Item Extraction:** Automatically identifies tasks, owners, and deadlines.
*   **Lightweight & Powerful:** Leverages state-of-the-art AI models without requiring a powerful computer or large downloads.

---

### Demo
*(A GIF of the working app will go here once the project is complete)*

---

### Tech Stack
*   **Language:** Python
*   **UI:** Streamlit
*   **Core AI:** Hugging Face Inference API (`Mistral-7B-Instruct`)
*   **API Communication:** `requests` library

---

### How to Run Locally
1.  **Clone the repository:** 
    ```bash
    git clone https://github.com/IanOchiengAI/project-meeting-summarizer.git
    ```
2.  **Navigate into the project directory:**
    ```bash
    cd project-meeting-summarizer
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Set up your API Key:**
    *   Create a new folder named `.streamlit` in the main project directory.
    *   Inside this folder, create a file named `secrets.toml`.
    *   Add your Hugging Face API token to this file like so:
        ```toml
        HF_API_TOKEN = "hf_YourSecretTokenGoesHere"
        ```
5.  **Run the Streamlit app:**
    ```bash
    streamlit run app/main_app.py
    ```
