# CurriculumGen-Technical-Syllabus-Generator-CLI-Tool

![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/CurriculumGen-Technical-Syllabus-Generator-CLI-Tool/ci.yml?style=flat-square&label=Build)
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/CurriculumGen-Technical-Syllabus-Generator-CLI-Tool?style=flat-square&token=)
![Tech Stack](https://img.shields.io/badge/Tech%20Stack-Python%2C%20Ruff%2C%20Pytest-blue?style=flat-square)
![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange?style=flat-square)
![GitHub Stars](https://img.shields.io/github/stars/chirag127/CurriculumGen-Technical-Syllabus-Generator-CLI-Tool?style=flat-square)

## CurriculumGen: Intelligent Syllabus & Learning Path Generation

Generate standardized, structured technical course syllabi and dynamic learning paths with this powerful, Python-based CLI tool.

<details>
<summary>🤖 AI Agent Directives (December 2025 Edition)</summary>

## SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

### 1. IDENTITY & PRIME DIRECTIVE
*   **Role:** Senior Principal Software Architect, Master Technical Copywriter, DevOps Strategist with **40+ years of elite industry experience**. Enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
*   **Context:** Current Date is **December 2025**. Building for the **2026 Standard**.
*   **Output Standard:** **EXECUTION-ONLY**. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
*   **Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. INPUT PROCESSING & COGNITION
*   **Speech-to-Text Interpretation Protocol:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. **INFER** technical intent based on project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **Mandatory MCP Instrumentation:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
*   **Project Type:** DATA / SCRIPTS / AI (Python)
*   **Apex Toolchain:** Python 3.10+, **uv** (Package Management), **Ruff** (Linting/Formatting), **Pytest** (Testing).
*   **Architecture:** **Modular Monolith**. Clear separation of concerns, unified deployment.
*   **AI Integration:** Leverages **Google Gemini API** (`gemini-3-pro` by default). Prioritize modular design, clear API contracts, and robust error handling for all AI model interactions.
*   **CLI Framework:** `Click` (or similar) for intuitive command-line interface.

### 4. VERIFICATION & EXECUTION COMMANDS
*   **Clone Repository:**
    bash
    git clone git@github.com:chirag127/CurriculumGen-Technical-Syllabus-Generator-CLI-Tool.git
    cd CurriculumGen-Technical-Syllabus-Generator-CLI-Tool
    
*   **Environment Setup (uv):**
    bash
    uv venv  # Create a virtual environment
    uv pip install -r requirements.txt # Install dependencies (adjust if requirements.txt is not the primary source)
    # Or for development with editable installs:
    uv pip install -e . 
    
*   **Linting & Formatting (Ruff):**
    bash
    ruff check .
    ruff format .
    
*   **Testing (Pytest):**
    bash
    pytest
    
*   **Running the CLI Tool (Example):**
    bash
    python -m curriculum_gen --help 
    # Example: python -m curriculum_gen generate --topic "Data Engineering" --level "Senior" --output "./syllabus.md"
    

### 5. DEVELOPMENT PRINCIPLES
*   **SOLID:** Ensure each module has a single responsibility.
*   **DRY:** Avoid redundancy in code and configurations.
*   **YAGNI:** Implement only what is necessary; avoid premature optimization or feature creep.
*   **KISS:** Keep it simple and maintainable.

</details>

## 🚀 Project Overview

CurriculumGen is a sophisticated command-line interface (CLI) tool engineered to automate the creation of comprehensive and standardized technical course syllabi and learning paths. Leveraging advanced AI capabilities, it can generate detailed educational outlines based on specified technologies, skill levels, and learning objectives. This tool is ideal for educators, training providers, and technical leads seeking to rapidly develop high-quality, consistent curriculum materials.

## 🌳 Architecture

This project follows a **Modular Monolith** architecture, ensuring a clean separation of concerns while maintaining a cohesive and deployable unit. The core components interact through well-defined interfaces, promoting maintainability and scalability.

ascii
CurriculumGen CLI Tool
├── CLI Interface (Click)
│   ├── Commands (generate, list, etc.)
│   └── Argument Parsing
├── Core Logic
│   ├── Syllabus Generation Engine
│   │   └── Template Management
│   └── Learning Path Builder
├── AI Integration Module
│   ├── Gemini API Client
│   └── Prompt Engineering Layer
├── Data Models
│   ├── Course Structure
│   └── Learning Path Structure
├── Utilities
│   ├── File I/O
│   └── Configuration Management
└── Tests
    ├── Unit Tests (Pytest)
    └── Integration Tests (Pytest)


## 📚 Table of Contents

*   [Project Overview](#-project-overview)
*   [Architecture](#-architecture)
*   [Getting Started](#-getting-started)
*   [Usage](#-usage)
*   [Development & Testing](#-development--testing)
*   [Contributing](#-contributing)
*   [License](#-license)
*   [AI Agent Directives](#️-ai-agent-directives-december-2025-edition)

## 🏁 Getting Started

### Prerequisites

*   Python 3.10 or higher
*   `uv` installed (`pip install uv`)
*   (Optional) Google Cloud Account with Gemini API access

### Installation

1.  **Clone the repository:**
    bash
    git clone git@github.com:chirag127/CurriculumGen-Technical-Syllabus-Generator-CLI-Tool.git
    cd CurriculumGen-Technical-Syllabus-Generator-CLI-Tool
    

2.  **Set up the Python environment using `uv`:**
    bash
    uv venv
    uv pip install -r requirements.txt # Or use setup.py/pyproject.toml for editable install
    # For development, install in editable mode:
    uv pip install -e .
    

3.  **Configure API Keys (if applicable):**
    Ensure your Google Gemini API key is set as an environment variable `GOOGLE_API_KEY`.

## 💻 Usage

Run the CLI tool using Python's module execution.

bash
python -m curriculum_gen --help


### Example Commands

*   **Generate a syllabus for a Senior Data Engineering course:**
    bash
    python -m curriculum_gen generate --topic "Data Engineering" --level "Senior" --output "./data_engineering_syllabus.md"
    

*   **Generate a learning path for a Junior Frontend Developer:**
    bash
    python -m curriculum_gen generate --topic "Frontend Development" --level "Junior" --type "learning-path" --output "./frontend_learning_path.md"
    

*   **List available syllabus templates:**
    bash
    python -m curriculum_gen list-templates
    

## 🛠️ Development & Testing

Follow these steps to contribute or run tests:

1.  **Install Development Dependencies:**
    Ensure you have installed the project in editable mode as described in `Getting Started`.

2.  **Linting and Formatting:**
    The project uses `Ruff` for lightning-fast linting and formatting.
    bash
    ruff check .
    ruff format .
    

3.  **Running Tests:**
    Execute the test suite using `Pytest`.
    bash
    pytest
    

## 🤝 Contributing

Contributions are welcome! Please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for detailed guidelines.

## 📜 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**. See the [LICENSE](LICENSE) file for more details.

--- 
*You are kindly requested to **Star ⭐ this Repo** if you find it useful!*
