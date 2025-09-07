# Security Policy for FutureCalc

## Introduction

The security of FutureCalc is a top priority. As an educational financial tool, maintaining user trust is critical, even though the application is fully client-side and does not handle personally identifiable information (PII) or connect to real financial accounts.

We appreciate the efforts of security researchers and the community to help keep our project safe. This policy outlines the process for reporting vulnerabilities.

## Supported Versions

Security updates and support are provided only for the latest version of the code available on the `main` branch of this repository.

| Version | Supported          |
| ------- | ------------------ |
| Latest  | :white_check_mark: |

## Reporting a Vulnerability

If you discover a security vulnerability, please report it to us privately to protect the project and its users. **Please do not disclose the vulnerability publicly** until a resolution has been reached.

You can report a vulnerability through one of the following methods:

1.  **GitHub Private Vulnerability Reporting (Preferred Method):**
    *   Navigate to the **"Security"** tab of the FutureCalc repository.
    *   Click on **"Report a vulnerability"** on the left-hand side.
    *   Provide a detailed description of the vulnerability, including steps to reproduce it.

We will do our best to acknowledge your report within 48-72 hours.

## Scope

This security policy applies to the FutureCalc application hosted on GitHub Pages and the code within this repository.

### In-Scope Vulnerabilities

We are most interested in vulnerabilities such as:

*   **Cross-Site Scripting (XSS):** Any way to execute unintended JavaScript in a user's browser via the input fields.
*   **Data Validation Bypass:** Issues where malformed input can crash the application or lead to unexpected and dangerous behavior.
*   **Significant Calculation Flaws:** Bugs in the financial logic that would produce severely misleading results for a user.

### Out-of-Scope Vulnerabilities

The following issues are considered out of scope for this project:

*   Vulnerabilities related to the GitHub Pages platform itself (e.g., missing HTTP security headers like `Content-Security-Policy`, `HSTS`, or issues with GitHub's servers). As we do not control the hosting infrastructure, these should be reported to GitHub.
*   Reports on the "lack of a backend" or "data stored in `localStorage`." This is by design, as the tool is intentionally 100% client-side.
*   Social engineering or phishing attacks.
*   Reports from automated scanners with no proof-of-concept or clear impact.

---

Thank you for helping keep FutureCalc and its users safe.

MrGuato 
