---
certifications:
- SOC 2 Type II
- HIPAA
- HITECH
description: ''
kind: trust-center
layout: security
name: Nuna Trust Center
name_suffix: Trust Center
overview: Nuna maintains a public trust center documenting SOC 2 Type II, HIPAA, and HITECH compliance.
provider_name: Nuna
provider_slug: nuna
slug: nuna-trust-center
source_filename: nuna-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.nuna.com/trust/\nname: Nuna Trust Center\ntrust_center:\n  published: true\n  summary_page: https://www.nuna.com/trust/\n  url: https://app.vanta.com/nuna.com/trust/048n92bu6ryb8pixhtfn3i\n  platform: Vanta\n  self_service: true\n  note: >-\n    The Vanta-hosted trust center returns HTTP 200 but the body is a client-rendered SPA shell, so the\n    document inventory and control status are only readable in a browser. The certifications below are\n    quoted from Nuna's own server-rendered /trust/ page, not from the SPA.\ncertifications:\n- name: SOC 2 Type II\n  status: audited\n  evidence: >-\n    \"We undergo SOC 2 Type II audits and share the resulting security, availability, and\n    confidentiality reports with our customers.\"\n  trust_service_criteria:\n  - security\n  - availability\n  - confidentiality\n  report_access: on request to customers\n- name: HIPAA\n  status: compliant\n  evidence: >-\n    \"We\
  \ meet all HIPAA and HITECH requirements, including the Privacy, Security, and Breach\n    Notification Rules. All vendors and third parties operate under Business Associate Agreements\n    (BAAs).\"\n- name: HITECH\n  status: compliant\n  evidence: Stated alongside HIPAA on the /trust/ page.\nframeworks:\n- name: NIST AI Risk Management Framework\n  role: AI governance framework alignment\n  evidence: >-\n    \"Our AI governance framework is aligned with the NIST AI Risk Management Framework to ensure\n    safety, fairness, and transparency at every stage.\"\n- name: NIST (general)\n  role: policy framework for application security, data privacy, business continuity, change\n    management, incident response\n  evidence: '\"Our policies follow current HIPAA and NIST frameworks across core areas...\"'\nai_governance:\n  human_oversight: >-\n    \"We establish clear lines of accountability for all decisions made with the assistance of AI.\n    Human oversight is integrated into all sensitive\
  \ use-cases.\"\n  independent_review: >-\n    \"annual, independent security reviews and vulnerability assessments of our AI models and\n    infrastructure\"\n  training_on_customer_data: false\n  training_statement: >-\n    \"client data is never used to train any proprietary or third-party AI models. Instead, we\n    integrate commercially available foundation models in a secure configuration.\"\nnot_claimed:\n- ISO 27001\n- ISO 27017\n- ISO 27018\n- PCI DSS\n- FedRAMP\n- HITRUST\nx-evidence:\n- url: https://www.nuna.com/trust/\n  http_status: 200\n  fetched: '2026-08-26'\n- url: https://app.vanta.com/nuna.com/trust/048n92bu6ryb8pixhtfn3i\n  http_status: 200\n  content_type: text/html\n  fetched: '2026-08-26'\n  note: 200 but a 5.3 KB SPA shell; content requires script execution.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuna/refs/heads/main/security/nuna-trust-center.yml
summary_line: SOC 2 Type II, HIPAA, HITECH
tags:
- Company
- Healthcare
- Health Data
- Medicaid
- Medicare
- Analytics
- Chronic Care
- Digital Health
- Artificial Intelligence
- Mobile
trust_url: ''
---
