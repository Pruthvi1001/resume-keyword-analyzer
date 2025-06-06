# Smart Resume Keyword Analyzer

A web-based tool built with Python and Flask that parses a user's PDF resume and a job description to calculate a keyword match score. It uses NLTK for natural language processing to identify key terms and provides actionable feedback to help users tailor their resume for specific job applications.

<img width="1440" alt="Screenshot 2025-06-06 at 6 24 24 PM" src="https://github.com/user-attachments/assets/dfb9ecc6-18d3-442c-b2f2-02931b59012a" />
<img width="1440" alt="Screenshot 2025-06-06 at 6 24 59 PM" src="https://github.com/user-attachments/assets/779c8fb6-6c98-4c0c-aadd-e4673612534f" />


## Features

*   **PDF Resume Parsing:** Extracts raw text from uploaded PDF resumes using PyPDF2.
*   **Keyword Extraction:** Processes text from both the resume and job description using NLTK to tokenize, lemmatize, and remove stopwords.
*   **Noun-Based Filtering:** Identifies and extracts key nouns, which often represent critical skills and technologies.
*   **Match Score Calculation:** Compares the two sets of keywords and calculates a percentage match score.
*   **Dynamic UI:** Provides instant feedback with matched keywords, missing keywords, and a dynamic progress bar.
*   **Responsive Design:** A clean, professional interface that works on desktop and mobile.

## Technologies Used

*   **Backend:** Python, Flask
*   **NLP:** NLTK (Natural Language Toolkit)
*   **File Handling:** PyPDF2
*   **Frontend:** HTML5, CSS3, Bootstrap 5, JavaScript
*   **Deployment:** (Mention where you plan to host it, e.g., PythonAnywhere, Heroku, etc. - even if it's just a plan)

## Setup and Installation

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/resume-keyword-analyzer.git
    cd resume-keyword-analyzer
    ```

2.  **Create and activate a virtual environment:**
    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install the dependencies:**
    ```sh
    pip install -r requirements.txt
    ```

4.  **Download NLTK data models:**
    ```sh
    python setup_nltk.py
    ```

5.  **Run the Flask application:**
    ```sh
    flask --app app run --debug
    ```

Open your browser and navigate to `http://127.0.0.1:5000`.
