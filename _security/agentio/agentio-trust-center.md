---
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Agentio Trust Center
name_suffix: Trust Center
overview: Agentio maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: Agentio
provider_slug: agentio
slug: agentio-trust-center
source_filename: agentio-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nurl: https://www.agentio.com/security\nnote: >-\n  Agentio has no trust.agentio.com or security.agentio.com host (both fail to resolve). It\n  publishes a single security-and-privacy page on its marketing site that names one\n  certification and describes the program. There is no trust portal, no downloadable report,\n  no subprocessor list, and no vulnerability-disclosure contact on that page — so this repo\n  records a trust page, not a vulnerability-disclosure program.\ncertifications:\n- SOC 2 Type 2\nprogram:\n  governance: >-\n    Security and Privacy teams establish policies and controls, monitor compliance with them,\n    and prove security and compliance to third-party auditors. Policies are stated as\n    least-privilege access, defense-in-depth layering, consistent enterprise-wide application,\n    and iterative maturing of controls.\n  data_protection:\n  - all datastores with customer data are encrypted at\
  \ rest\n  - TLS 1.2 or higher everywhere data crosses potentially insecure networks\n  - application secrets encrypted and stored in Google Cloud Platform Secret Manager\n  product_security:\n  - vulnerability scanning required at key stages of the Secure Development Lifecycle\n  enterprise_security:\n  - centrally managed corporate devices with MDM and anti-malware\n  - endpoint security alerts monitored 24/7/365\n  - MDM-enforced disk encryption, screen lock, and software updates\nevidence:\n- source: https://www.agentio.com/security\n  http_status: 200\n  keywords:\n  - soc 2 type 2\n  - compliance\n  - governance\n  - data protection\n  - secure development lifecycle\n- source: https://trust.agentio.com/\n  http_status: 0\n  note: host does not resolve\n- source: https://www.agentio.com/trust\n  http_status: 404\nx-evidence:\n  fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentio/refs/heads/main/security/agentio-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Company
- AdTech
- Advertising
- Creator Economy
- Influencer Marketing
- Marketing
- Artificial Intelligence
- YouTube
- MCP
- Agents
- Analytics
trust_url: https://www.agentio.com/security
---
