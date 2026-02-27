# My Cycode Assessment - Juice Shop Project

## Project Overview
I deployed the OWASP Juice Shop using Docker on Render.

## Live Application


## Project Screenshots
### 1. Application Homepage

### 2. Render Deployment Status


## Discussion Questions

### 1. Is there anything wrong with committing directly to master?
Yes. It creates a security blind spot and bypasses 'Shift Left' security gates like SAST and Secret Scanning.

### 2. How would you prevent that?
By implementing Branch Protection Rules and Status Checks, along with Pre-commit hooks.

### 3. Repository Settings Changes
In production, I would use a CODEOWNERS file to enforce expert review and restrict direct access to master.

## Final Walkthrough

### Connection Process
Integrated Cycode via GitHub App using a dedicated Organization for full SDLC visibility (Code, Build, and Issues).

### Platform Overview
Utilized Cycode as an ASPM solution to consolidate security findings and map the software supply chain.

### Findings
- Secrets: Identified exposed tokens in the commit history.
- SAST: Detected critical vulnerabilities including SQL Injection and XSS.
- SCA: Flagged outdated dependencies with known CVEs.

## Final Walkthrough

### Connection Process
Integrated Cycode via GitHub App using a dedicated Organization for full SDLC visibility (Code, Build, and Issues).

### Platform Overview
Utilized Cycode as an ASPM solution to consolidate security findings and map the software supply chain.

### Findings
- Secrets: Identified exposed tokens in the commit history.
- SAST: Detected critical vulnerabilities including SQL Injection and XSS.
- SCA: Flagged outdated dependencies with known CVEs.

### Final Proof of Detection
- Status: Violation Successfully Detected.
- Finding: Generic Secret/Password found in security_test.txt.
- Impact: Confirmed real-time secret scanning is active and reporting to the ASPM dashboard.
