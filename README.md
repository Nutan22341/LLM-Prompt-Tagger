# 🚀 PromptNER

**PromptNER** is a lightweight web application that combines **Named Entity Recognition (NER)** using **spaCy** with the power of a **locally running Large Language Model (LLM)** using **Phi-4 Mini via Ollama**.

It allows users to input natural language prompts and:
- Highlights named entities such as `PERSON`, `LOCATION`, `ORGANIZATION`, and `DATE` using spaCy.
- Sends the prompt to a locally running **Phi-4 Mini** model via Ollama and displays a contextual response.

---

## ✨ Features
- Real-time named entity recognition (NER) using spaCy
- LLM-generated intelligent responses using Phi-4 Mini (Ollama)
- Responsive, dark-themed web interface
- Lightweight and runs completely locally — no cloud required

---

## 🧰 Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** FastAPI
- **NER Engine:** spaCy (`en_core_web_sm`)
- **LLM:** Phi-4 Mini (via Ollama)
- **Server:** Uvicorn
## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Nutan22341/LLM-Prompt-Tagger.git

## Install the requirements.txt
pip install -r requirements.txt
python -m spacy download en_core_web_sm

## Ensure Ollama is installed
ollama run phi4-mini

## Start the FastAPI server
uvicorn main:app --reload

