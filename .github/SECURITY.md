# Security Policy

## Supported Versions

We are committed to providing a secure and reliable tool. We actively monitor and patch vulnerabilities in the following actively supported versions:

*   **1.x.x** (Latest Stable)

Older versions may not receive security updates.

## Reporting a Vulnerability

We take security very seriously. If you discover any security vulnerabilities in **CurriculumGen-Technical-Syllabus-Generator-CLI-Tool**, please report them responsibly.

**Do not publicly disclose the vulnerability until it has been addressed.**

To report a vulnerability, please follow these steps:

1.  **Create a Private Issue:** Go to the [**Issues**](https://github.com/chirag127/CurriculumGen-Technical-Syllabus-Generator-CLI-Tool/issues) tab on GitHub.
2.  **Prefix the Title:** Start the issue title with `[SECURITY VULNERABILITY]` (e.g., `[SECURITY VULNERABILITY] Potential RCE in input parsing`).
3.  **Provide Details:** In the issue description, include:
    *   A clear and concise description of the vulnerability.
    *   The affected version(s) of the software.
    *   Detailed steps to reproduce the vulnerability.
    *   Any supporting evidence (logs, screenshots, proof-of-concept code).
    *   Your suggested mitigation or fix, if you have one.
4.  **Set to Private:** Ensure the issue is created as **private** (visible only to you and repository administrators).

Once reported, our security team will review the vulnerability and work on a fix. We will aim to acknowledge your report within **48 hours** and provide regular updates on the progress. We will also credit you in the release notes once the vulnerability is fixed and publicly disclosed.

## Supported Security Tools

This repository is configured to use the following security best practices and tools:

*   **Dependency Scanning:** GitHub's Dependabot is enabled to automatically scan for vulnerable dependencies and create pull requests to update them.
*   **Static Analysis Security Testing (SAST):** While not explicitly detailed here, our CI pipeline (`.github/workflows/ci.yml`) is designed to integrate SAST tools in the future for proactive code scanning. The current focus is on code quality via Ruff.
*   **Code Linting & Formatting:** **Ruff** is used to enforce coding standards and catch potential issues early in the development cycle. This contributes to overall code health and reduces the surface area for certain types of vulnerabilities.
*   **Python Dependency Management:** **uv** is used for secure and efficient management of project dependencies, ensuring reproducible builds and minimizing risks associated with package acquisition.

## Responsible Disclosure Timeline

We aim to follow a responsible disclosure process:

1.  **Report Received:** Acknowledge receipt of the security report.
2.  **Triage & Verification:** Investigate and verify the reported vulnerability.
3.  **Fix Development:** Develop and test a patch.
4.  **Coordinated Disclosure:** Once the patch is ready, we will coordinate with the reporter for a public disclosure, typically including the fix in a new release.

Thank you for helping to keep **CurriculumGen-Technical-Syllabus-Generator-CLI-Tool** secure!
