## What this pipeline does

This repo demonstrates a beginner-friendly DevSecOps workflow that runs security checks automatically on every push and pull request.

### Security checks
- **SAST (Static Application Security Testing)** with CodeQL

### Where results appear
- **Actions tab**: shows the workflow run logs
- **Security → Code scanning alerts**: shows security findings

### Why this matters
This is a baseline pattern for enforcing security in CI/CD pipelines to catch issues early in the SDLC.

## Vulnerable vs Secure Example

- `insecure_login()` demonstrates a SQL Injection vulnerability
- `safe_login()` fixes the issue using parameterized queries

This shows how DevSecOps pipelines can detect issues early and how developers remediate them securely.

## What to look for in the results
- CodeQL may flag `insecure_login()` (intentionally vulnerable example)
- `safe_login()` demonstrates the remediation using parameterized queries
