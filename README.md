# Teleginski Academy

Welcome to the **Teleginski Academy** repository, a project designed for learning and developing applications using Python.

---

## Overview

This project includes various components to create and run Python-based applications. It is structured to facilitate the learning of essential programming and software development concepts.

The repository also includes functionality for interacting with PDF documents using advanced natural language processing techniques, integrating libraries such as:

- 📝 **PyPDF2**: For reading and manipulating PDF files.
- 🔗 **LangChain**: A powerful framework for building natural language processing pipelines.
- 🤖 **OpenAI**: For utilizing advanced language models.

These tools are used in the `rag.py` script to provide intelligent answers based on the loaded PDFs' content.

---

## Repository Structure

Below is a description of the main files found in this repository:

- 📂 **Biblioteca.py**: Contains functions and classes that support the project's features.
- 🚀 **app.py**: The main entry point to run the application.
- 🛠 **gitignore.txt**: Specifies files and directories to be ignored by Git.
- 📜 **pyproject.toml**: Project configuration, including dependencies and build information.
- 🔍 **rag.py**: Script for interacting with PDF documents, utilizing the mentioned libraries to extract information and answer questions based on the content.

---

## Application Architecture

The **Teleginski Academy** architecture is modular and designed to be understandable and extensible. It follows a layered model with the following responsibilities:

### 1. Application Layer
- 📂 Represented by the `app.py` file, this layer is the main entry point for the user to interact with the application.
- Key responsibilities:
  - Execute the general program flow.
  - Coordinate calls to other layers (libraries and modules).
  - Manage user input and present results.

### 2. Business Logic Layer
- 🔧 Implemented in `Biblioteca.py` and `rag.py`.
- Key responsibilities:
  - **Biblioteca.py**:
    - Contains utility functions and classes for general application support.
    - Modularizes reusable logic.
  - **rag.py**:
    - Focused on interaction with PDF documents.
    - Uses libraries like `PyPDF2` to manipulate PDFs, extract text, and perform queries.
    - Employs `LangChain` and the `OpenAI` API for natural language processing and generating intelligent responses based on PDF content.
- This layer abstracts complex technical details, facilitating the development of new features.

### 3. Data Layer
- 📊 Represented by the PDF files provided by users and processed by `rag.py`.
- Key responsibilities:
  - Extracting and manipulating data from PDFs.
  - Temporary storage in memory for quick queries.
- Uses `PyPDF2` to read and structure text from files, serving as the basis for analyses.

### 4. Integrations and Dependencies
- 📑 **PyPDF2**:
  - Responsible for PDF file operations such as text reading and page manipulation.
- 🔗 **LangChain**:
  - Orchestrates complex question-and-answer flows, ensuring the application processes inputs and provides consistent responses.
- 🤖 **OpenAI**:
  - Utilizes advanced language models to interpret questions and generate responses based on data extracted from PDFs.
- ⚙️ The `pyproject.toml` file manages project dependencies and configurations, enabling easy maintenance and installation.

### 5. Configuration and Management Layer
- 📂 **gitignore.txt**:
  - Defines files and directories not to be versioned (e.g., sensitive or generated data).
- 📝 **pyproject.toml**:
  - Contains project metadata and specifies necessary dependencies.
- Environment settings can be adjusted to enable new features or future integrations.

---

## Requirements

To run the project, ensure you have the following installed:

- 🐍 **Python 3.8+**
- 📦 A dependency manager like `pip`

Required libraries can be installed from the `requirements.txt` file, which includes dependencies like `PyPDF2`, `LangChain`, and `OpenAI`.

---

## Installation

1. 📥 Clone this repository:
   ```bash
   git clone https://github.com/petersonchiquetto/Teleginski_academy.git
   ```

2. 📂 Navigate to the cloned directory:
   ```bash
   cd Teleginski_academy
   ```

3. 📦 Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## How to Run

### Main Application

🚀 To run the main application, use the following command:

```bash
python app.py
```

### PDF Interaction

🔍 To use the PDF interaction functionality, run the `rag.py` script with the following command:

```bash
python rag.py
```

This script allows you to load PDF files and ask questions about their content. Ensure all dependencies are correctly installed before running.

---

## How to Contribute

🛠 Contributions are always welcome! Follow the steps below to contribute:

1. 🍴 Fork this repository.
2. 🌱 Create a branch with your contribution:
   ```bash
   git checkout -b my-contribution
   ```
3. 💾 Commit your changes:
   ```bash
   git commit -m "My contribution: [description]"
   ```
4. 📤 Push your changes:
   ```bash
   git push origin my-contribution
   ```
5. 🔄 Open a Pull Request in this repository.

---

## Contact

If you have questions or suggestions, feel free to reach out:

- 👤 Author: **Peterson Chiquetto**
- 🌐 GitHub: [petersonchiquetto](https://github.com/petersonchiquetto)

---

## License

📜 This project is licensed under the [MIT License](LICENSE). See the license file for details.

