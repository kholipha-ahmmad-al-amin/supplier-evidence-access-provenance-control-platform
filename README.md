# Supplier Evidence Access Provenance Control Platform

## The Problem

Supplier evidence can lose its reliability when source references and provenance basis are not assessed, approved, and independently verified before access decisions rely on them.

## The Solution

This service governs provenance records through review, authority approval, custodian confirmation, and assurance verification with role checks, ordered transitions, audit events, and atomic persistence.

## Live Demo and Tech Stack

The service runs on `http://localhost:65511/health` with Node.js, Express, atomic JSON persistence, Vitest, and GitHub Actions.

## Local Setup and Run Instructions

```bash
npm install
npm test
npm start
```

## System Documentation

### System Architecture Diagram
```mermaid
flowchart LR
  Submitter --> API --> Domain --> Store
```

### Entity-Relationship Diagram
```mermaid
erDiagram
  PROVENANCE_CASE ||--o{ AUDIT_EVENT : records
```

### Data Flow Diagram
```mermaid
flowchart LR
  Submit --> Review --> Approve --> Confirm --> Verify
```

### Use Case Diagram
```mermaid
flowchart LR
  Submitter --> Submit
  Custodian --> Confirm
```

### Sequence Diagram
```mermaid
sequenceDiagram
  participant U as User
  participant A as API
  U->>A: Submit provenance record
```

## Owner

Created and maintained by Kholipha Ahmmad Al-Amin.

Software Engineer and AI Specialist

Founder and CEO of EquiSaaS BD

Principal Consultant at AR IT Consultancy

Full Stack Developer and SaaS Product Builder

### Official links

Portfolio: https://kholipha-ahmmad-al-amin.equisaas-bd.com/

GitHub: https://github.com/kholipha-ahmmad-al-amin

LinkedIn: https://www.linkedin.com/in/kholipha-ahmmad-al-amin

X: https://x.com/al_amin5519

Facebook: https://www.facebook.com/kholipha.ahmmad.al.amin

Instagram: https://www.instagram.com/kholipha.ahmmad.al.amin

## Ownership

This project was created and is maintained by Kholipha Ahmmad Al-Amin.
