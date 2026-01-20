# AI-Driven Code Reviewer

![Project Logo](logo.png)

> **A smart, AI-powered assistant for automated code analysis, error detection, and optimization suggestions.** > *Developed during the Virtual Internship at Infosys Springboard.*

---

## 📋 Table of Contents
- [About the Project](#-about-the-project)
- [Key Features](#-key-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Installation & Setup](#-installation--setup)
- [Usage Guide](#-usage-guide)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)

---

## 📖 About the Project

The **AI-Driven Code Reviewer** is a web-based application designed to assist developers in improving their code quality. Leveraging the power of Large Language Models (LLMs) via **Google's Generative AI**, this tool analyzes Python code snippets to identify potential errors, suggest improvements, and enforce coding standards.

This project was built as part of the **Infosys Springboard Virtual Internship**, aiming to automate the code review process and provide instant, actionable feedback to developers.

---

## 🚀 Key Features

* **🔍 Automated Code Analysis**: Instantly parses Python code to understand structure and logic.
* **🐛 Error Detection**: Identifies syntax errors and potential runtime issues using static analysis.
* **🎨 Style Checking**: Checks code against PEP-8 standards using `pylint` logic to ensure readability.
* **🤖 AI Suggestions**: Utilizes Google's Generative AI (Gemini/PaLM) to provide intelligent refactoring suggestions and bug fixes.
* **💬 Interactive Chatbot**: A built-in chat interface to ask specific questions about the code.
* **📄 AST Parsing**: Visualizes the Abstract Syntax Tree (AST) of the code for deeper structural understanding.

---

## 🛠 Tech Stack

* **Programming Language**: Python 3.11.0
* **Web Framework**: Streamlit (for the User Interface)
* **AI Model**: Qwen (Qwen2.5-7B-Instruct / HuggingFace API)
* **Static Analysis**: AST (Abstract Syntax Tree), Pylint
* **Version Control**: Git & GitHub

---

## 📂 Project Structure

Here is an overview of the key files in the repository:

```text
📂 AI-Driven-Code-Reviewer
├── 📄 app.py                  # Main entry point for the Streamlit application
├── 📄 chatbot.py              # Logic for the interactive AI chatbot
├── 📄 ai_suggester.py         # Interface with Google's Generative AI for suggestions
├── 📄 code_parser.py          # Handles parsing of Python code (AST)
├── 📄 error_detector.py       # Identifies syntax and logical errors
├── 📄 style_checker.py        # Checks code for style and PEP-8 compliance
├── 📄 chatmodel_google.py     # Configuration and setup for Google AI models
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
* A Google Cloud API Key for Generative AI (Gemini).

### Steps

1. **Clone the Repository**
```bash
git clone [https://github.com/TAK-PRAVEEN/AI-Driven-Code-Reviewer.git](https://github.com/TAK-PRAVEEN/AI-Driven-Code-Reviewer.git)
cd AI-Driven-Code-Reviewer

```


2. **Create a Virtual Environment (Optional but Recommended)**
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

```


3. **Install Dependencies**
```bash
pip install -r requirements.txt

```


4. **Set Up API Keys**
* Obtain your API key from [Google AI Studio](https://aistudio.google.com/).
* Create a `.env` file in the root directory or configure it directly in the script (depending on implementation in `chatmodel_google.py`).


```env
GOOGLE_API_KEY=your_api_key_here

```


5. **Run the Application**
```bash
streamlit run app.py

```



---

## 🖥 Usage Guide

1. **Launch the App**: After running the command, the application will open in your default web browser (usually at `http://localhost:8501`).
2. **Input Code**: Paste your Python code snippet into the provided text area.
3. **Analyze**: Click the **"Review Code"** or **"Analyze"** button.
4. **View Results**:
* **Bug Report**: See detected errors.
* **Style Review**: Check for PEP-8 compliance.
* **AI Suggestions**: Read how the AI recommends fixing or optimizing the code.


5. **Chat**: Use the chatbot sidebar/section to ask "Why is this line wrong?" or "How can I make this loop faster?"

---

## 🔮 Future Enhancements

* Support for multiple programming languages (Java, C++, JavaScript).
* Integration with GitHub Webhooks for automatic Pull Request reviews.
* More advanced security vulnerability scanning.
* User authentication and history saving.

---

## 👤 Author

**Praveen Tak** * **Role**: Intern at Infosys Springboard

* **GitHub**: [TAK-PRAVEEN](https://www.google.com/search?q=https://github.com/TAK-PRAVEEN)
* **LinkedIn**: [Praveen Tak](https://www.google.com/search?q=https://www.linkedin.com/in/praveentak/)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](https://www.google.com/search?q=LICENSE) file for details.
