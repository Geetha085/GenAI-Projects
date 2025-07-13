
# 📚 Multi-PDF Chatbot using LangChain, FAISS, and HuggingFace

This Streamlit app lets you **chat with multiple PDF documents**. Upload one or more PDFs, and ask questions about their content. It uses **LangChain** for conversational retrieval, **FAISS** for vector search, and **HuggingFace** models for embeddings and language generation.

---

## 🚀 Features

* Upload multiple PDF files
* Extracts and chunks text using LangChain
* Creates semantic embeddings with `hkunlp/instructor-xl`
* Stores embeddings in a FAISS vectorstore
* Uses `flan-t5-xxl` from HuggingFace for LLM-powered Q\&A
* Remembers chat history with conversational memory

---

## 🧠 Tech Stack

* **Python**
* **Streamlit** – for the web interface
* **LangChain** – for chaining the components
* **FAISS** – for efficient vector similarity search
* **HuggingFace Transformers** – for embeddings and language model
* **PyPDF2** – for reading PDF files
* **dotenv** – for managing API keys

---

## 📂 File Structure

```bash
.
├── app.py                  # Main Streamlit app
├── htmlTemplates.py        # HTML templates for chatbot UI
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

---

## 📦 Installation

1. **Clone the repo**

```bash
git clone https://github.com/your-username/multi-pdf-chatbot.git
cd multi-pdf-chatbot
```

2. **Create and activate a virtual environment** (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate  # on Windows use: venv\Scripts\activate
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Add your HuggingFace API Key**

Create a `.env` file in the root directory and add:

```env
HUGGINGFACEHUB_API_TOKEN=your_api_key_here
```

---

## ▶️ How to Run

```bash
streamlit run app.py
```

---

## 📌 Notes

* If you're running on a low-spec machine, you can switch to a smaller model like `flan-t5-base`.
* The `hkunlp/instructor-xl` embedding model can be heavy. If you hit memory limits, try `all-MiniLM-L6-v2`.

---

## 📄 Example Use Cases

* Chat with academic papers or research documents
* Analyze financial reports
* Explore legal contracts
* Review product manuals or policy PDFs

---

## 🙌 Acknowledgments

* [LangChain](https://github.com/hwchase17/langchain)
* [HuggingFace Transformers](https://huggingface.co/models)
* [FAISS](https://github.com/facebookresearch/faiss)
* [Streamlit](https://streamlit.io/)

