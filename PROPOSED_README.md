# CurriculumGen: AI-Powered Technical Syllabus Generator CLI Tool

## Purpose

CurriculumGen is a robust, dynamic command-line interface (CLI) tool designed to automate the creation of structured and standardized technical course syllabi and comprehensive learning paths. It intelligently generates educational content based on user-specified technology stacks and learning objectives.

## Architecture Overview

mermaid
graph TD
    A[CLI Interface (Click)] --> B(Syllabus Generation Logic)
    B --> C{Tech Stack Analysis}
    B --> D(Learning Path Structuring)
    C --> E[CurriculumGen Core]
    D --> E
    E --> F(Output Formatting)
    F --> G[Syllabus File (Markdown/JSON)]
    subgraph Core Engine
        E
    end


## Table of Contents

*   [Purpose](#purpose)
*   [Architecture Overview](#architecture-overview)
*   [Table of Contents](#table-of-contents)
*   [AI Agent Directives](#ai-agent-directives)
*   [Development Setup](#development-setup)
*   [Usage](#usage)
*   [Contributing](#contributing)
*   [License](#license)

## AI Agent Directives

<details>
<summary>View AI Agent Directives</summary>

### 1. Identity & Prime Directive

*   **Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
*   **Context:** Current Date is **December 2025**. You are building for the 2026 standard.
*   **Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
*   **Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. Input Processing & Cognition

*   **Speech-to-Text Interpretation Protocol:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **Mandatory MCP Instrumentation:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. Context-Aware Apex Tech Stacks (Late 2025 Standards)

*   **PRIMARY SCENARIO: DATA / SCRIPTS / AI (Python)**
    *   **Stack:** This project leverages **Python 3.10+**. Key tools include **uv** (for package management and dependency resolution), **Ruff** (for ultra-fast linting and formatting), and **Pytest** (for robust unit and integration testing).
    *   **Architecture:** Adheres to a **Modular Monolith** pattern, ensuring clear separation of concerns for features like syllabus generation logic, tech stack analysis, and CLI interface, while maintaining a unified deployment.
    *   **AI Integration:** **Not applicable** for this specific project's core function, which focuses on structured syllabus generation rather than generative AI content. If AI features were integrated, prioritize modular design, clear API contracts, and robust error handling.
    *   **CLI Framework:** Uses `Click` for a powerful and intuitive command-line interface.

### 4. Operational Directives

*   **Version Control:** Git is the sole VCS. All commits must be atomic and include a clear, concise message following Conventional Commits.
*   **Testing & Verification:**
    *   **Unit Tests:** **Pytest** is mandatory for all core logic. Aim for >90% code coverage.
    *   **Linting & Formatting:** **Ruff** must be configured to enforce consistent code style and identify potential issues across the entire codebase. Run `ruff check --fix` and `ruff format` before committing.
    *   **Dependency Management:** **uv** must be used for installing dependencies and managing virtual environments. Ensure `uv.lock` is committed.
*   **Security:**
    *   **Dependency Scanning:** Regularly scan dependencies for vulnerabilities using tools integrated with `uv` or equivalent.
    *   **Secret Management:** NEVER hardcode secrets. Use environment variables or secure configuration management.
*   **Documentation:** README.md is the SSOT. All significant changes must be reflected here. Docstrings are required for all public functions and classes.

</details>

## Development Setup

Follow these steps to set up the development environment:

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/CurriculumGen-Technical-Syllabus-Generator-CLI-Tool.git
    cd CurriculumGen-Technical-Syllabus-Generator-CLI-Tool
    

2.  **Create and activate a virtual environment using uv:**
    bash
    uv venv
    source .venv/bin/activate
    

3.  **Install dependencies:**
    bash
    uv pip install -r requirements.txt
    

4.  **Install development dependencies (including dev tools):**
    bash
    uv pip install -r requirements-dev.txt
    

## Usage

Once installed, CurriculumGen can be run from the command line.

### Basic Syllabus Generation:

bash
curriculumgen generate --tech-stack python,django,pytest --title "Python Web Development Fundamentals" --output syllabus.md


### Advanced Learning Path Generation:

bash
curriculumgen generate-path --tech-stack javascript,react,redux,testing-library --level intermediate --output learning_path.json


*(Refer to `curriculumgen --help` for a complete list of commands and options.)*

## Contributing

We welcome contributions! Please follow the guidelines in the **[CONTRIBUTING.md](https://github.com/chirag127/CurriculumGen-Technical-Syllabus-Generator-CLI-Tool/blob/main/.github/CONTRIBUTING.md)** file.

## License

This project is licensed under the **CC BY-NC 4.0** license. See the [LICENSE](https://github.com/chirag127/CurriculumGen-Technical-Syllabus-Generator-CLI-Tool/blob/main/LICENSE) file for more details.
