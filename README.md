# 📝 Exam-Gen: AI Question Paper Generator ✨

Exam-Gen is an intelligent Streamlit web application designed to assist educators by automating the creation of diverse and well-structured exam papers. By leveraging a Retrieval-Augmented Generation (RAG) pipeline, this tool analyzes source documents (like textbook chapters or notes) and generates a unique question paper based on user-defined parameters.

![Exam-Gen Screenshot]
*(Optional: Add a screenshot of your app here later)*

## 🚀 Features

- **Multi-Document Support**: Upload multiple PDF files to form a comprehensive knowledge base.
- **Dynamic Exam Structure**: Specify the exact number of questions needed for various mark values (1, 2, 3, 4, 5, and 10 marks).
- **Intelligent Topic Analysis**: Automatically identifies the main topics in the source material to ensure a balanced and diverse set of questions.
- **Semantic Uniqueness Filter**: Over-generates and filters questions to prevent semantic duplicates, ensuring each question is unique.
- **PDF Export**: Download the generated Question Paper and Answer Key as separate, professionally formatted PDF files.
- **Modern UI**: A clean, intuitive, and fun user interface built with Streamlit.

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **AI/NLP Framework**: LangChain
- **Generative LLM**: Google Gemini API
- **Embedding Model**: `sentence-transformers/all-MiniLM-L6-v2`
- **Vector Database**: ChromaDB
- **Topic Modeling**: BERTopic
- **PDF Handling**: PyMuPDF, FPDF2

## ⚙️ Setup and Installation

Follow these steps to run the project locally.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/Exam-Gen.git](https://github.com/YOUR_USERNAME/Exam-Gen.git)
    cd Exam-Gen
    ```

2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    # Windows
    .\venv\Scripts\Activate
    # macOS/Linux
    source venv/bin/activate
    ```

3.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up your API Key:**
    - Create a `.env` file in the root directory.
    - Add your Google Gemini API key to it:
      ```
      GOOGLE_API_KEY="YOUR_API_KEY_HERE"
      ```

5.  **Run the Streamlit app:**
    ```bash
    streamlit run app.py
    ```