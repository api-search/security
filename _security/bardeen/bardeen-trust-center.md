---
certifications:
- SOC 2 Type 2
- GDPR
- CASA Tier 2
- CASA Tier 3
- OWASP ASVS
description: Bardeen publishes its security, privacy and compliance posture on a single page at https://www.bardeen.ai/security. There is no dedicated trust-center host (trust.bardeen.ai does not resolve) and no self-serve document portal; the page states that a "Compliance and Security Center" for continuous posture monitoring is available to Business and Enterprise customers only, so certification reports are gated behind a commercial relationship.
kind: trust-center
layout: security
name: Bardeen Trust Center
name_suffix: Trust Center
overview: Bardeen maintains a public trust center documenting SOC 2 Type 2, GDPR, CASA Tier 2, CASA Tier 3, and OWASP ASVS compliance.
provider_name: Bardeen
provider_slug: bardeen
slug: bardeen-trust-center
source_filename: bardeen-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nprobe: true\nsource: https://www.bardeen.ai/security\nurl: https://www.bardeen.ai/security\nstatus: 200\ndescription: >-\n  Bardeen publishes its security, privacy and compliance posture on a single page at\n  https://www.bardeen.ai/security. There is no dedicated trust-center host (trust.bardeen.ai does\n  not resolve) and no self-serve document portal; the page states that a \"Compliance and Security\n  Center\" for continuous posture monitoring is available to Business and Enterprise customers only,\n  so certification reports are gated behind a commercial relationship.\ncertifications:\n  - name: SOC 2 Type 2\n    body: AICPA\n    since: '2024-04-01'\n    evidence: \"As of April 1, 2024, we are proud to announce our compliance with the AICPA SOC 2\n      Type 2 standards, ensuring that our systems and processes meet rigorous criteria for security.\"\n  - name: GDPR\n    body: EU\n    evidence: \"we adhere to the EU's GDPR compliance\
  \ checklist for US companies, affirming our\n      commitment to data protection and privacy for our international users.\"\n  - name: CASA Tier 2\n    body: App Defense Alliance\n    evidence: \"Bardeen meets the stringent requirements of Tier 2 and Tier 3 of the Cloud\n      Application Security Assessment (CASA) as defined by the App Defense Alliance.\"\n  - name: CASA Tier 3\n    body: App Defense Alliance\n    evidence: same statement as CASA Tier 2\n  - name: OWASP ASVS\n    body: OWASP\n    evidence: \"built upon the industry-recognized OWASP Application Security Verification\n      Standard (ASVS)\"\ncontrols:\n  encryption_in_transit: TLS 1.2\n  encryption_at_rest: AES-256\n  infrastructure_as_code: true\n  peer_review: true\n  dependency_scanning: true\n  data_residency_note: >-\n    App data is persisted in the user's local browser storage by default and not in Bardeen's cloud;\n    cloud instances used for always-on automations are described as having no storage and erasing\n\
  \    data when a playbook finishes.\ngated:\n  name: Compliance and Security Center\n  available_to: Business and Enterprise subscription tiers\n  self_serve: false\n  note: Continuous posture monitoring and certification artifacts are customer-only; no public\n    document request flow is published.\nevidence:\n  - source: https://www.bardeen.ai/security\n    status: 200\n    fetched: '2026-08-29'\n    keywords: [soc 2 type 2, gdpr, casa, owasp asvs, tls 1.2, aes-256]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bardeen/refs/heads/main/security/bardeen-trust-center.yml
summary_line: SOC 2 Type 2, GDPR, CASA Tier 2, CASA Tier 3, OWASP ASVS
tags:
- AI Automation
- Workflow-Automation
- Web Scraping
- Data Enrichment
- Browser Extension
- Sales Automation
- No Code
- Go-To-Market
trust_url: https://www.bardeen.ai/security
---
