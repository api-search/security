---
certifications:
- ISO/IEC 27001:2013
- SOC 1
- SOC 2
- GDPR
- HIPAA
- FedRAMP
description: ''
kind: trust-center
layout: security
name: Creatio Trust Center
name_suffix: Trust Center
overview: Creatio maintains a public trust center documenting ISO/IEC 27001:2013, SOC 1, SOC 2, GDPR, HIPAA, and FedRAMP compliance.
provider_name: Creatio
provider_slug: creatio
slug: creatio-trust-center
source_filename: creatio-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.creatio.com/our-technologies/security\ndocs:\n  security: https://www.creatio.com/our-technologies/security\n  shared_responsibility: https://www.creatio.com/gdpr/shared-security-responsibility-model\n  gdpr: https://www.creatio.com/GDPR\n  ai_trust_and_governance: https://www.creatio.com/ai/ai-trust-and-governance\n  legal: https://www.creatio.com/legal\nsummary: >-\n  Creatio does not run a hosted trust center (trust.creatio.com returns 404) and\n  does not publish a certificate portal with downloadable attestations. It does\n  publish a security page naming its certifications and its testing program.\n  Certificates themselves are not linked from the page — a buyer requests them\n  through sales.\ntrust_center_url: null\ntrust_center_note: >-\n  Probed https://trust.creatio.com/ -> 404 and https://www.creatio.com/company/security\n  -> 404. The security content lives at /our-technologies/security.\ncertifications:\n\
  \  - name: ISO/IEC 27001:2013\n    status: certified\n    evidence: >-\n      \"ISO / IEC 27001: 2013 compliance certificate issued to the Creatio cloud\n      services.\"\n    document_url: null\n  - name: SOC 1\n    status: claimed\n    evidence: Listed among the standards Creatio's data processing centers comply with.\n    document_url: null\n  - name: SOC 2\n    status: claimed\n    evidence: Listed among the standards Creatio's data processing centers comply with.\n    document_url: null\n  - name: GDPR\n    status: compliant\n    evidence: >-\n      \"The data processing centers are compliant with international industry\n      standards, including GDPR.\" Creatio also publishes a shared security\n      responsibility model and a Data Processing Addendum.\n    document_url: https://www.creatio.com/gdpr/shared-security-responsibility-model\n  - name: HIPAA\n    status: claimed\n    evidence: >-\n      \"Creatio complies with the HIPAA security requirements.\" The HIPAA\n      compliance\
  \ option is listed as an Enterprise-plan capability on the\n      pricing comparison.\n    document_url: null\n  - name: FedRAMP\n    status: badge-displayed\n    evidence: >-\n      A FedRAMP compliance badge is displayed on the security page. No\n      authorization package, agency sponsor or Marketplace listing is linked, so\n      this is recorded as displayed-but-unverified rather than authorized.\n    document_url: null\nsecurity_program:\n  vulnerability_scanning: true\n  penetration_testing: true\n  penetration_testing_note: >-\n    \"Regular internal and external penetration testing for the network and\n    software.\" Third-party tools are also used for scanning and security\n    testing. No report or summary is published.\n  compliance_audits: true\n  bug_bounty: false\n  vulnerability_disclosure_program: false\n  disclosure_note: >-\n    No vulnerability disclosure policy, security@ contact, or bug bounty program\n    was found. /.well-known/security.txt is WAF-blocked (HTTP\
  \ 403) on\n    www.creatio.com, academy.creatio.com and community.creatio.com — blocked,\n    not served, so it is not a published disclosure channel. No listing found on\n    HackerOne, Bugcrowd or Intigriti.\ninfrastructure:\n  hosting:\n    - Amazon Web Services\n    - Microsoft Azure\n  note: Cloud instances are hosted on AWS and Azure data processing centers.\ngaps:\n  - No trust center or certificate portal — attestations are sales-gated.\n  - No published vulnerability disclosure policy or security.txt (403, WAF-blocked).\n  - FedRAMP badge is displayed without a linked authorization.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatio/refs/heads/main/security/creatio-trust-center.yml
summary_line: ISO/IEC 27001:2013, SOC 1, SOC 2, GDPR, HIPAA, FedRAMP
tags:
- Company
- Saas
- CRM
- No-Code
- Low-Code
- Business Process Management
- Workflow-Automation
- Sales
- Marketing
- Customer Service
- OData
- AI Agents
trust_url: ''
---
