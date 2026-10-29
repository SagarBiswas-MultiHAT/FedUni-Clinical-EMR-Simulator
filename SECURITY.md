# Security Policy

## Supported Versions

The following versions of the EMR Simulation Web Application currently receive security updates:

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |
| < 1.0   | :x:                |

## Reporting a Vulnerability

Security and privacy are essential, especially in medical and clinical simulation environments. If you identify any security issue or vulnerability, please follow responsible disclosure practices:

1. Do NOT open a public GitHub issue for security vulnerabilities.
2. Email the maintainer directly at the contact address listed in the repository profile.
3. Include detailed steps to reproduce the issue, expected versus actual behavior, and proof of concept where applicable.

You can expect an initial acknowledgement within 48 hours and regular updates as a fix is developed and deployed.

## Sensitive Data Guidelines

- This project is strictly a training simulator. Never input real Protected Health Information (PHI) or identifiable patient details.
- Always keep connection strings, user credentials, and cryptographic keys out of source control.
- Ensure production environments configure ASP.NET Data Protection keys in a secure key vault rather than unencrypted local storage.

