# 📚 Intelligent Research Assistant

> **Note on this fork**
> Fork of a two-person academic project, originally at
> [shalakapadalkar16/Intelligent-Research-Assistant](https://github.com/shalakapadalkar16/Intelligent-Research-Assistant).
> Both contributors are credited at the bottom of this README.

## 📌 Overview

The **Intelligent Research Assistant** is a **Streamlit** and **FastAPI-based web application** that allows users to:

- Search for **research papers** related to a given topic using **Elasticsearch**.
- Retrieve **detailed metadata** including **title, authors, publication date, abstract, and PDF link**.
- Generate **summaries** of research papers using the **Ollama AI API**.

This project helps researchers, students, and professionals quickly gather and understand relevant research literature.

---

## 🚀 Features

✔ **Search Research Papers**: Query research papers stored in an **Elasticsearch** index.  
✔ **View Paper Details**: Get **authors, publication date, and abstracts** for each paper.  
✔ **Summarization**: Generate **concise summaries** using **Ollama API**.  
✔ **Fast & Responsive UI**: Built with **Streamlit** for an interactive experience.  
✔ **API Backend**: Powered by **FastAPI** for smooth interactions.

---

## 🛠️ Tech Stack

### **Frontend (UI)**

- **Streamlit** – Provides a clean and simple user interface.

### **Backend**

- **FastAPI** – Handles API requests for search and summarization.
- **Elasticsearch** – Stores and retrieves research papers.
- **Ollama API** – Provides AI-based text summarization.

---

## 📂 Project Structure

```ini
Intelligent-Research-Assistant/
│── backend/
│   ├── main.py          # FastAPI server
│   ├── requirements.txt # Backend dependencies
│── frontend/
│   ├── app.py           # Streamlit app
│   ├── requirements.txt # Frontend dependencies
│── README.md            # Project Documentation
│── docker-compose.yml   # Docker configuration (Optional)
└── .gitignore           # Ignore unnecessary files
```

---

## 🔧 Installation & Setup

### **1️⃣ Clone the Repository**

```bash
git clone https://github.com/your-username/Intelligent-Research-Assistant.git
cd Intelligent-Research-Assistant
```

### **2️⃣ Set Up Backend (FastAPI)**

#### **🔹 Install Dependencies**

```bash
cd backend
pip install -r requirements.txt
```

#### **🔹 Run FastAPI Server**

```bash
uvicorn main:app --reload
```

FastAPI will start at: `http://127.0.0.1:8000`

---

### **3️⃣ Set Up Frontend (Streamlit)**

#### **🔹 Install Dependencies**

```bash
cd ../frontend
pip install -r requirements.txt
```

#### **🔹 Run Streamlit App**

```bash
streamlit run app.py
```

Streamlit will start at: `http://localhost:8501`

---

## 🖥️ API Endpoints (FastAPI)

### **1️⃣ Search Papers**

🔗 `GET /search/?query=<your_query>`  
📌 __Example:__

```bash
curl -X GET "http://127.0.0.1:8000/search/?query=machine learning"
```

### **2️⃣ Summarize a Paper**

🔗 `GET /summarize/?paper_title=<paper_title>`  
📌 __Example:__

```bash
curl -X GET "http://127.0.0.1:8000/summarize/?paper_title=Deep Learning"
```

---

## 🐳 Docker Support (Optional)

If you want to run this project inside **Docker**, use the `docker-compose.yml` file:

```bash
docker-compose up --build
```

---

## 🤝 Contributing

💡 Contributions are **welcome**! If you’d like to improve this project:

1. **Fork** this repository.
2. **Create a new branch** (`git checkout -b feature-branch`).
3. **Commit your changes** (`git commit -m "Added new feature"`).
4. **Push to your fork** (`git push origin feature-branch`).
5. **Submit a Pull Request**!

---

## 📜 License

⚖️ This project is **open-source** and available under the **MIT License**.

---

## 📞 Contact

## 🔹 **Contributor:** [Durgesh Sakhardande](https://www.linkedin.com/in/durgesh-s/)  
🔹 **GitHub:** [DurgeshS-25](https://github.com/DurgeshS-25)  
🔹 **Email:** [sakhardande.d@northeastern.edu](mailto:sakhardande.d@northeastern.edu)

## 🔹 **Contributor:** [Shalaka Padalkar](https://www.linkedin.com/in/shalaka-padalkar/)  
🔹 **GitHub:** [shalakapadalkar16](https://github.com/shalakapadalkar16)  
🔹 **Email:** [padalkar.sha@northeastern.edu](mailto:padalkar.sha@northeastern.edu)

