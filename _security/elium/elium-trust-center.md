---
certifications:
- ISO/IEC 27001:2022
- SecNumCloud
- GDPR
- EU AI Act
- EcoVadis Silver
description: ''
kind: trust-center
layout: security
name: Elium Trust Center
name_suffix: Trust Center
overview: Elium maintains a public trust center documenting ISO/IEC 27001:2022, SecNumCloud, GDPR, EU AI Act, and EcoVadis Silver compliance.
provider_name: Elium
provider_slug: elium
slug: elium-trust-center
source_filename: elium-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nsource: https://elium.com/trust\nurl: https://elium.com/trust\nhttp_status: 200\nprobed: '2026-08-17'\nsections:\n  overview: https://elium.com/trust\n  resources: https://elium.com/trust/resources\n  controls: https://elium.com/trust/controls\n  subprocessors: https://elium.com/trust/subprocessors\n  updates: https://elium.com/trust/updates\nsecurity_contact: security@elium.com\nsecurity_contact_note: >-\n  Published as a mailto link on both the trust overview (\"Contact our security team\") and the controls page\n  (\"Email security team\"). Elium states the mailbox \"handles vendor reviews, RFPs, audits, and architecture\n  questions\".\ncertifications:\n- ISO/IEC 27001:2022\n- SecNumCloud\n- GDPR\n- EU AI Act\n- EcoVadis Silver\ncertifications_not_claimed: [SOC 2, HIPAA, PCI DSS, FedRAMP, HDS]\ndocuments_on_request:\n  count: 8\n  process: >-\n    \"Request the DPA in the Resources section above. We aim to counter-sign\
  \ within five working days.\"\n  documents:\n  - Elium AI - technical details\n  - ISO 27001 certificate\n  - Statement of Applicability (ISO 27002:2022)\n  - Penetration test report (2025)\n  - Penetration test report (2024)\n  - Cyber insurance certificate (2026)\n  - Data Processing Agreement\n  - List of third-party providers\n  note: >-\n    None of the eight is downloadable without a request - the certificate itself, the SoA and both\n    penetration-test reports are gated behind a form. Only the certification names are public.\ncontrols:\n  url: https://elium.com/trust/controls\n  domains: [Physical Security, Network Security, Data Security, General Data Protection, Quality & Service,\n    Reversibility, 'Backup & Recovery']\n  highlights:\n  - control: Encryption in transit\n    detail: >-\n      \"All data transfers enforce a secure connection (HTTPS with TLS 1.3 or TLS 1.2, using strong cipher\n      suites including AES-256-GCM and ChaCha20-Poly1305).\"\n  - control: Security\
  \ audits\n    detail: >-\n      \"Penetration tests are conducted regularly by independent third parties and vulnerability scans are\n      automated. Findings are assessed and remediated per defined SLAs.\"\n  - control: Incident management\n    detail: >-\n      Severity classification, coordinated response, customer notification, and \"priority-based SLAs with\n      defined acknowledgement and resolution targets\"; every incident triggers a post-incident root-cause\n      and lessons-learned review.\n  - control: Enterprise SSO\n    detail: >-\n      \"SAML2 and OpenID connectors are available for seamless enterprise SSO integration, including\n      ADFS/Microsoft.\"\n  - control: Support team access\n    detail: >-\n      Support access to a customer platform requires professional SSO, MFA and a time-limited random\n      password, with an audit-trail notification to both the employee and the customer's administrators.\n  - control: Availability\n    detail: >-\n      \"The monthly\
  \ uptime rate is guaranteed and monitored by an external service. Availability metrics are\n      published and contractually committed.\"\n  - control: Audit log\n    detail: Administrative and security events are preserved in a tamper-evident audit log.\ndata_residency:\n  default: European Union - Google Cloud Platform, Belgium region, with redundancy across European data centres\n  sovereign: 3DS Outscale sovereign French cloud (SecNumCloud-qualified)\n  on_premise: supported (https://elium.com/on-premise)\n  policy: Hosting region is set per tenant and never mixed.\nai_data_policy: >-\n  \"Customer content is never used to train or fine-tune models - ours or our providers'. Generative-AI calls\n  run with zero data retention contractually enforced with every LLM provider.\"\nsubprocessors:\n  url: https://elium.com/trust/subprocessors\n  count: 22\n  named:\n  - {name: Google Cloud Platform, region: EU, role: default compute and storage}\n  - {name: Aiven, region: EU, role: managed\
  \ database hosting}\n  - {name: 3DS Outscale, region: EU (France), role: sovereign SecNumCloud-qualified cloud}\n  - {name: SparkPost, region: 'EU (Belgium)', role: email processing}\n  - {name: Mixpanel, region: 'EU (Netherlands)', role: product analytics}\n  - {name: Datadog, region: 'EU (Germany)', role: application logs}\nstatus_page: https://status.elium.com/\nevidence:\n- {source: 'https://elium.com/trust', http_status: 200, keywords: [ISO/IEC 27001:2022, SecNumCloud, GDPR,\n      EU AI Act, EcoVadis Silver, trust center, security@elium.com]}\n- {source: 'https://elium.com/trust/controls', http_status: 200, keywords: [penetration tests, vulnerability\n      scans, incident management, TLS 1.3, SAML2, OpenID, audit log, uptime]}\n- {source: 'https://elium.com/trust/subprocessors', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elium/refs/heads/main/security/elium-trust-center.yml
summary_line: ISO/IEC 27001:2022, SecNumCloud, GDPR, EU AI Act, EcoVadis Silver
tags:
- Company
- SaaS
- Knowledge Management
- Knowledge Base
- Enterprise Search
- AI Search
- GraphQL
- MCP
- Collaboration
- Documentation
- RAG
- Europe
trust_url: https://elium.com/trust
---
