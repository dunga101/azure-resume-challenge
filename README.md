# Azure Resume Challenge

This project is a cloud-hosted professional resume built using Microsoft Azure.  
It demonstrates practical cloud engineering fundamentals including static web hosting, cost-aware architecture, security-by-default configuration, and disciplined version control.

**Live Resume:**  
https://azresumestoragedm.z9.web.core.windows.net/

---

## Architecture Overview (Phase 1)

**Pattern:** Static Website Hosting on Azure Storage

The resume is hosted using Azure Blob Storage’s Static Website feature, allowing global access over HTTPS without managing servers or compute resources.

### Azure Services Used
- Azure Storage Account (StorageV2)
- Blob Static Website

### Region
- **Canada Central**  
  Chosen as the primary Canadian Azure region, aligning with user location and standard enterprise deployment practices.

---

## Repository Structure

```
azure-resume-challenge/
├── frontend/
│ ├── index.html
│ └── styles.css
├── .gitignore
└── README.md
```
---

## Frontend Implementation

### Technologies
- HTML5
- CSS3

### Design Principles
- Clear visual hierarchy for recruiter readability
- Conservative, professional styling
- Separation of content (HTML) and presentation (CSS)
- Mobile-friendly layout

---

## Security & Governance

- HTTPS enforced by default
- Secure transfer required
- Minimum TLS version: 1.2
- Public access limited to static web endpoint
- Azure resource tagging applied for ownership and cost tracking

---

## Cost Considerations

This project is intentionally designed to operate at minimal cost.

- Azure Storage (static website): ~$0
- No compute resources used
- No databases in Phase 1

**Estimated annual cost:** Less than $5 CAD

---

## Future Enhancements

Planned next phases of the challenge include:

- Visitor counter using Azure Functions (serverless)
- Azure Table Storage for persistence
- CI/CD automation using GitHub Actions
- Infrastructure-as-Code for Azure resources
- Additional documentation and diagrams

---

## Purpose

This project is part of a personal cloud portfolio to demonstrate real-world Azure usage, engineering discipline, and production-minded decision making — not certification-only knowledge.
