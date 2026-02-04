# -Medical-Chatbot-with-LLMs-LangChain-Pinecone-Flask-AWS

Here is a professionally structured `README.md` for your project. I have organized it to be clear, scannable, and developer-friendly.

---

# Medical Chatbot using LLMs & Generative AI

A robust end-to-end medical chatbot leveraging the power of **Large Language Models (GPT)**, **LangChain** for orchestration, and **Pinecone** as a vector database. The application is served via a **Flask** web interface and is designed for deployment on **AWS**.

## Tech Stack Used

* **Language:** Python
* **Framework:** Flask
* **Orchestration:** LangChain
* **LLM:** OpenAI GPT
* **Vector Database:** Pinecone
* **Cloud:** AWS

---

## Getting Started

Follow these steps to set up the project locally.

### Prerequisites

* Anaconda or Miniconda installed.
* Pinecone API Key.
* OpenAI API Key.

### Installation

1. **Clone the Repository**
```bash
git clone https://github.com/entbappy/Build-a-Complete-Medical-Chatbot-with-LLMs-LangChain-Pinecone-Flask-AWS.git
cd Build-a-Complete-Medical-Chatbot-with-LLMs-LangChain-Pinecone-Flask-AWS

```


2. **Create and Activate Environment**
```bash
conda create -n medibot python=3.10 -y
conda activate medibot

```


3. **Install Dependencies**
```bash
pip install -r requirements.txt

```


4. **Environment Configuration**
Create a `.env` file in the root directory and add your credentials:
```env
PINECONE_API_KEY = "your_pinecone_api_key"
OPENAI_API_KEY = "your_openai_api_key"

```



---

## Execution Flow

### 1. Vector Embeddings

Before running the application, you must process the medical data and store the embeddings in Pinecone.

```bash
python store_index.py

```

### 2. Launch the Application

Start the Flask server to interact with the chatbot.

```bash
python app.py

```

### 3. Access

Once the server is running, open your web browser and navigate to:
**`http://localhost:5000`** (or the port specified in your terminal).

---

## Project Structure

| File/Folder | Description |
| --- | --- |
| `app.py` | Main Flask application file. |
| `store_index.py` | Script to push data embeddings to Pinecone. |
| `src/` | Contains helper functions and logic (Prompt templates, data loading). |
| `templates/` | HTML files for the web interface. |
| `static/` | CSS and JavaScript files for UI. |
| `requirements.txt` | List of Python dependencies. |

---

## Deployment

This project is optimized for **AWS**. You can deploy it using:

* **EC2 Instance:** Host the Flask app on a virtual server.
* **Docker:** Containerize the application for consistent deployment.
* **CI/CD:** Use GitHub Actions to automate the deployment to AWS.

Would you like me to generate a specific **GitHub Actions** workflow file or a **Dockerfile** to help with the AWS deployment?
