# AI-Driven Code Reviewer

![Project Logo](logo.png)

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://ai-driven-code-reviewer.streamlit.app/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/)

> **A smart, AI-powered assistant for automated code analysis, error detection, and optimization suggestions.**
> *Developed during the Virtual Internship at Infosys Springboard.*

---

## 📋 Table of Contents
- [About the Project](#-about-the-project)
- [Live Demo](#-live-demo)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Installation & Setup](#-installation--setup)
- [Usage Guide](#-usage-guide)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)

---

## 📖 About the Project

The **AI-Driven Code Reviewer** is a web-based application designed to assist developers in improving their code quality. Leveraging the power of the **Qwen 2.5** Large Language Model (via Hugging Face), this tool analyzes Python code snippets to identify potential errors, suggest improvements, and enforce coding standards.

This project was built as part of the **Infosys Springboard Virtual Internship**, aiming to automate the code review process and provide instant, actionable feedback to developers.

---

## 🌐 Live Demo

Check out the deployed application live on Streamlit Cloud:
👉 **[Click here to try the AI Code Reviewer](https://ai-driven-code-reviewer.streamlit.app/)**

---

## 🚀 Key Features

* **🔍 Automated Code Analysis**: Instantly parses Python code to understand structure and logic.
* **🐛 Error Detection**: Identifies syntax errors and potential runtime issues using static analysis.
* **🎨 Style Checking**: Checks code against PEP-8 standards to ensure readability.
* **🤖 AI Suggestions**: Utilizes the **Qwen-2.5-7B-Instruct** model to provide intelligent refactoring suggestions and bug fixes.
* **💬 Interactive Chatbot**: A built-in chat interface to ask specific questions about your code logic.
* **📄 AST Parsing**: Visualizes the Abstract Syntax Tree (AST) of the code for deeper structural understanding.

---

## 🛠 Tech Stack

* **Programming Language**: Python 3.11
* **Web Framework**: Streamlit (User Interface)
* **AI Model**: Qwen/Qwen2.5-7B-Instruct (via Hugging Face Inference API)
* **Static Analysis**: AST (Abstract Syntax Tree), Pylint
* **Version Control**: Git & GitHub

---

## 📂 Project Structure

Here is an overview of the key files in the repository:

```text
📂 AI-Driven-Code-Reviewer
├── 📄 app.py                  # Main entry point for the Streamlit application
├── 📄 chatbot.py              # Logic for the interactive AI chatbot
├── 📄 ai_suggester.py         # Interface with Hugging Face API for suggestions
├── 📄 code_parser.py          # Handles parsing of Python code (AST)
├── 📄 error_detector.py       # Identifies syntax and logical errors
├── 📄 style_checker.py        # Checks code for style and PEP-8 compliance
├── 📄 prompt_ui.py            # UI components for input prompts
├── 📄 node_visitor.py         # Helper for traversing the AST nodes
├── 📄 requirements.txt        # List of Python dependencies
└── 📄 logo.png                # Project logo

```

---

## ⚙️ Installation & Setup

Follow these steps to run the project locally on your machine.

### Prerequisites

* Python 3.8 or higher installed.
* A **Hugging Face Access Token** (Read permission).

### Steps

1. **Clone the Repository**
```bash
git clone [https://github.com/TAK-PRAVEEN/AI-Driven-Code-Reviewer.git](https://github.com/TAK-PRAVEEN/AI-Driven-Code-Reviewer.git)
cd AI-Driven-Code-Reviewer

```


2. **Create a Virtual Environment (Recommended)**
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate

```


3. **Install Dependencies**
```bash
pip install -r requirements.txt

```


4. **Set Up API Keys**
* Get your Access Token from [Hugging Face Settings](https://huggingface.co/settings/tokens).
* Create a `.streamlit/secrets.toml` file (for Streamlit) or a `.env` file depending on your setup:


**For Streamlit Local Run (.streamlit/secrets.toml):**
```toml
HUGGINGFACE_ACCESS_TOKEN = "your_hf_token_here"

```


5. **Run the Application**
```bash
streamlit run app.py

```



---

## 🖥 Usage Guide

1. **Launch the App**: Open the link in your browser (local or live).
2. **Input Code**: Paste your Python code snippet into the text area.
3. **Analyze**: Click the **"Review Code"** button.
4. **View Results**:
* **Bug Report**: See detected errors.
* **Style Review**: Check for PEP-8 compliance.
* **AI Suggestions**: See how Qwen recommends fixing the code.


5. **Chat**: Use the sidebar to ask questions like "How can I optimize this function?".

---

## 🔮 Future Enhancements

* Support for multiple programming languages (Java, C++, JavaScript).
* Integration with GitHub Webhooks for automatic Pull Request reviews.
* More advanced security vulnerability scanning.
* User authentication and history saving.

---

## 👤 Author

**Praveen Tak**

* **Role**: Intern at Infosys Springboard
* **GitHub**: [TAK-PRAVEEN](https://www.google.com/search?q=https://github.com/TAK-PRAVEEN)
* **LinkedIn**: [Praveen Tak](https://www.google.com/search?q=https://www.linkedin.com/in/praveentak/)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](https://www.google.com/search?q=LICENSE) file for details.
