# Fill-a-Form

An intelligent system for automating document processing, specifically designed to extract information from source documents and fill out PDF forms using an event-driven agentic architecture with human-in-the-loop feedback.

---

## ✨ Features

* **Automated Form Filling:** Automatically extracts relevant information from source documents (e.g., a resume) to populate fields in a target PDF form (e.g., a job application).
* **Event-Driven Architecture:** Leverages an event-driven design pattern for asynchronous and parallel task execution within the agentic workflow.
* **Retrieval-Augmented Generation (RAG):** Integrates RAG to efficiently retrieve precise data from source documents, enhancing the agent's ability to answer form-related questions.
* **Intelligent Form Parsing:** Capable of parsing complex PDF forms, identifying required fields, and converting blank spaces into queries for the RAG system.
* **Human-in-the-Loop Feedback:** Incorporates mechanisms for human feedback, allowing for correction and refinement of agent-generated answers via text and voice instructions.
* **Multimodal Capability:** Supports processing spoken feedback to improve agent accuracy and user interaction.

---

## 🛠️ Technologies Used

* **Python**
* **LlamaIndex** (for building agentic workflows, RAG, and document parsing)
* **uv** (for dependency management and virtual environments)

---

## 🚀 Getting Started

Follow these steps to set up and run the Event-Driven Agentic Document Workflow locally.

### Prerequisites

* Python 3.9+
* `uv` installed: `pip install uv`

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/gamerguy27072/fill-a-form.git
    cd fill-a-form
    ```

2.  **Create and activate a virtual environment with `uv`:**
    ```bash
    uv venv
    source .venv/bin/activate # On macOS/Linux
    # .venv\Scripts\activate   # On Windows (in PowerShell/Cmd)
    ```

3.  **Install dependencies:**
    ```bash
    uv pip install -e .
    ```

### Configuration

* **API Keys:** You will likely need API keys for your Large Language Model (LLM) provider (e.g., OpenAI, Google AI) and potentially for any voice-to-text or text-to-speech services. Create a `.env` file in the root directory of the project and add your keys:
    ```
    OPENAI_API_KEY=your_openai_api_key
    # Add other keys as needed, e.g., GOOGLE_API_KEY, LLLAMA_CLOUD_API_KEY
    ```

---

## 💡 Usage

To run the Event-Driven Agentic Document Workflow, you will need to execute the code manually through the Jupyter Notebook:

1.  Ensure your virtual environment is active.
2.  Navigate to the `Notebooks` directory:
    ```bash
    cd Notebooks
    ```
3.  Open `Agent.ipynb` in a Jupyter Notebook environment (e.g., by running `jupyter lab` or `jupyter notebook` in the terminal and navigating to the file, or by opening it directly in VS Code).
4.  Run the cells within `Agent.ipynb` sequentially to observe and interact with the document processing workflow.

---

## 🚧 Work in Progress

This project is currently under active development. The following key objectives are planned:

* **Deployment:** The project is not yet deployed and therefore does not have a public-facing link.
* **API Endpoints:** Implementation of FastAPI routes to expose the document workflow functionalities as a web API for broader integration and accessibility.

---