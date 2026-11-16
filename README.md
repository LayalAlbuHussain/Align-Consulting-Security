# Align-Consulting-Security
Company Web Security Skills Framework

Version: 1.1
Type: Stack-Agnostic Security Framework
Status: Initial Reference Implementation

Overview

The Company Web Security Skills Framework is a reusable collection of security policies, AI skills, implementation examples, and validation tools designed to help developers build secure web dashboards.

The main goal is to standardize security practices across company projects, regardless of the technologies or AI coding assistants being used.

Instead of defining security requirements from scratch for every new dashboard, developers can reuse this framework with AI assistants such as Claude and ChatGPT/Codex.

The framework provides structured security instructions to guide AI-assisted development while supporting security validation through automated tests and code scanning.

Objectives

* Establish consistent security requirements across web applications.
* Provide reusable security instructions for AI coding assistants.
* Reduce security inconsistencies between projects.
* Integrate security practices into frontend, backend, and API development.
* Support automated security checks during development.
* Maintain a centralized, version-controlled security reference.

Framework Contents

The ZIP package contains the following main components:

Component	Description
policy/	Company security policies, control matrix, and quality requirements.
skills/	Eight reusable AI security skills.
templates/	Instruction templates for Claude Code and Codex.
examples/	Reference implementation and technology-adapter template.
tests/	Executable reference authorization tests.
tools/	Scripts for validating the framework and running configured tests.
.github/workflows/	GitHub Actions workflows for security checks.
ci/	Security review checklist and legacy example.

Security Skills

The framework includes eight security skills:

Skill	Purpose
Authentication	Secure user authentication and session management.
Authorization	Role-based permissions, access control, and tenant isolation.
Frontend Security	Protection against frontend vulnerabilities such as XSS.
Backend Security	Secure backend operations and server-side validation.
API Security	API access control, request validation, and abuse protection.
Data Protection	Protection of sensitive data and secrets.
Audit Logging	Secure logging of security-relevant activities.
Security Review	Security review guidance and verification checklist.

Each skill contains structured guidance for AI coding assistants to apply relevant security practices during development.

Security Standards

The framework is informed by industry-recognized security guidance, including:

* OWASP Application Security Verification Standard (ASVS)
* OWASP API Security Top 10
* OWASP secure coding recommendations

Note: The current version does not implement or verify every OWASP ASVS requirement. A complete control-by-control mapping and compliance assessment would require additional work.

How to Use

1. Download and Extract

Download the framework ZIP package and extract its contents into the development environment.

2. Integrate with an AI Assistant

For Claude Code, the security skills can be placed under:

.claude/skills/

For OpenAI Codex, they can be placed under:

.agents/skills/

Alternatively, developers using ChatGPT or Claude chat can attach the security policy and skill files as reference documents.

3. Apply Security Instructions

Developers can provide the following instruction to their AI assistant:

Read the Company Web Security Skills Framework and apply all relevant security requirements during the development of this web dashboard. Implement the required security controls across the frontend, backend, and APIs. Generate relevant security tests and report any unverified requirements or remaining security risks.

4. Run Reference Security Checks

The framework includes executable reference tests.

Run the following commands from the framework root:

python tools/check_framework.py
python -m unittest discover -s tests -v

These commands validate the framework structure and run reference authorization tests.

They do not validate the security of a new dashboard automatically.

5. Configure Security CI Checks

The package includes a GitHub Actions security workflow that provides:

* Framework structure validation.
* Reference authorization unit tests.
* Semgrep static application security scanning.

Additional application-specific tests and security scanners must be configured before using the framework as a release security gate.

Important Limitations

This framework is an initial foundation for secure AI-assisted development.

It is not a complete security solution, a security certification, or a guarantee that an application is secure.

Before production adoption, each project must adapt the requirements to its technology stack, implement appropriate integration tests, configure required CI security gates, and complete a security review.

Future Improvements

Planned enhancements may include:

* Detailed OWASP ASVS control mapping.
* Technology-specific security implementation templates.
* Automated API security integration tests.
* Dependency and secret scanning.
* Expanded security compliance reporting.
* Centralized management of approved security skill versions.

Conclusion

The Company Web Security Skills Framework provides a reusable foundation for implementing consistent security practices across AI-assisted web development projects.

By combining security policies, reusable AI skills, reference implementations, and automated checks, the framework aims to make secure development more consistent, maintainable, and scalable across the organization.
