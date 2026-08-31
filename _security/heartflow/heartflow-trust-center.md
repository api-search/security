---
certifications:
- SOC 2 Type 2
- ISO/IEC 27001:2022
- ISO 13485:2016
- HITRUST
- HIPAA
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Heartflow Trust Center
name_suffix: Trust Center
overview: HeartFlow maintains a public trust center documenting SOC 2 Type 2, ISO/IEC 27001:2022, ISO 13485:2016, HITRUST, HIPAA, GDPR, and CCPA compliance.
provider_name: HeartFlow
provider_slug: heartflow
slug: heartflow-trust-center
source_filename: heartflow-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nprobe: true\nsource: https://security.heartflow.com/\nurl: https://security.heartflow.com/\nplatform: SafeBase (Drata)\ndiscovery: >-\n  Linked from the site footer as \"Heartflow Trust Center\" at\n  https://www.heartflow.com/heartflow-trust-center/, which 301s to\n  https://security.heartflow.com/. The host sits behind a Cloudflare interactive\n  challenge, so a plain curl gets 403; a browser user-agent renders the real page.\ncertifications:\n- SOC 2 Type 2\n- ISO/IEC 27001:2022\n- ISO 13485:2016\n- HITRUST\n- HIPAA\n- GDPR\n- CCPA\nprograms:\n  product_security:\n  - Audit Logging\n  - Multi-Factor Authentication\n  - Role-Based Access Control\n  data_security:\n  - Access Monitoring\n  - Data Backups\n  - Encryption-at-rest\n  application_security:\n  - Application Penetration Testing\n  - Secure Development Training\n  - Software Bill of Materials (SBOM)\n  ai_security:\n  - AI Training Data and Bias\n  - AI Security\n  - AI\
  \ Monitoring\n  infrastructure:\n  - Amazon Web Services\n  - Business Continuity / Disaster Recovery\n  - Capacity Planning & Management\n  endpoint_security:\n  - Anti-Malware\n  - Disk Encryption\n  - Mobile Device Management\n  network_security:\n  - Firewall\n  - IDS/IPS\n  - Network Penetration Testing\n  corporate_security:\n  - Asset Management Practices\n  - Email Protection\n  - Employee Handbook\ngaps:\n- >-\n  No vulnerability disclosure or responsible-disclosure contact is published on the\n  trust center, and no /.well-known/security.txt is served on any Heartflow host.\n- >-\n  No public subprocessor list is displayed; document access on SafeBase trust centers\n  is normally NDA-gated.\nevidence:\n- source: https://security.heartflow.com/\n  http_status: 403\n  note: >-\n    403 is a Cloudflare interactive challenge served to non-browser clients, not a\n    dead page — the page renders for a browser user-agent. Certifications above were\n    read from that rendered page.\n\
  - source: https://www.heartflow.com/about/\n  http_status: 200\n  note: >-\n    Company About page carries the same certification badges — ISO 13485 / EN ISO\n    13485, SOC 2 (AICPA), HITRUST, ISO 27001.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heartflow/refs/heads/main/security/heartflow-trust-center.yml
summary_line: SOC 2 Type 2, ISO/IEC 27001:2022, ISO 13485:2016, HITRUST, HIPAA, GDPR, CCPA
tags:
- Company
- Healthcare
- Medical Imaging
- Artificial Intelligence
- Cardiology
- Diagnostics
- Medical Devices
- Radiology
- Clinical Decision Support
- Machine-Learning
trust_url: https://security.heartflow.com/
---
