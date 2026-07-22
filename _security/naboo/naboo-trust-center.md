---
certifications:
- SOC 2 Type II
- ISO 27001:2022
- GDPR
- HIPAA
- Penetration Testing
description: ''
kind: trust-center
layout: security
name: Naboo Trust Center
name_suffix: Trust Center
overview: Naboo maintains a public trust center documenting SOC 2 Type II, ISO 27001:2022, GDPR, HIPAA, and Penetration Testing compliance.
provider_name: Naboo
provider_slug: naboo
slug: naboo-trust-center
source_filename: naboo-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nprobe: false\nsource: https://www.naboo.ai/security/\nurl: https://www.naboo.ai/security/\nsummary: >-\n  Naboo publishes a Security & Trust page describing its compliance posture,\n  data-protection controls, and deployment models. Certifications are largely\n  in-progress/roadmap; a program (GDPR, HIPAA BAA, annual pen testing) is\n  established with supporting documents (SOC 2 letter of engagement, controls\n  matrix, pen-test summary, DPA/BAA) available under NDA.\ncertifications:\n  - name: SOC 2 Type II\n    status: in-progress\n    detail: Audit window underway; letter of engagement available on request under NDA.\n  - name: ISO 27001:2022\n    status: roadmap\n    detail: Implementation targeted H2 2026.\n  - name: GDPR\n    status: compliant\n    detail: Naboo operates as data processor; customer is controller. DPA available.\n  - name: HIPAA\n    status: baa-available\n    detail: BAA executed per customer engagement; healthcare\
  \ customers deploy air-gapped or VPC by default.\n  - name: Penetration Testing\n    status: annual\n    detail: Third-party independent testing; latest report available under NDA.\ncontrols:\n  encryption_in_transit: TLS 1.3 for all inter-component connections\n  encryption_at_rest: AES-256\n  kms: [AWS KMS, GCP KMS, Azure Key Vault, HashiCorp Vault]\n  rbac: Permissions mirrored from source systems (GitHub teams, Jira projects, Slack channels, Confluence spaces) and enforced at every graph traversal, at retrieval time.\n  audit_logging: Per-query audit logging shipped to customer SIEM; customer-controlled retention.\n  tenant_isolation: Each deployment runs in the customer environment with separate keys, data, and audit trail.\n  no_model_training: Customer data is never used to improve any model.\ndeployment_models:\n  - on-premises\n  - customer-vpc\n  - air-gapped\nsecurity_contact: security@naboo.ai\ndocuments_under_nda:\n  - SOC 2 letter of engagement\n  - controls matrix\n  - pen-test\
  \ summary\n  - sample DPA/BAA\n  - incident-response runbook\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/naboo/refs/heads/main/security/naboo-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001:2022, GDPR, HIPAA, Penetration Testing
tags:
- Company
- Artificial Intelligence
- AI Agents
- Knowledge Graph
- Reasoning Layer
- GraphQL
- Model Context Protocol
- Enterprise Software
- Developer Infrastructure
- RAG
trust_url: https://www.naboo.ai/security/
---
