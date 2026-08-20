---
certifications:
- SOC 2 Type II
- HIPAA
- GDPR
- CCPA
description: Demostack publishes a trust center on its own marketing site rather than a hosted trust portal (no Vanta/Drata/SafeBase instance, no subprocessor list, no document request flow). It names its attestation, auditor and effective date, its privacy posture, its HIPAA position, its scanning and pentest tooling, and its vulnerability disclosure program.
kind: trust-center
layout: security
name: Demostack Trust Center
name_suffix: Trust Center
overview: Demostack maintains a public trust center documenting SOC 2 Type II, HIPAA, GDPR, and CCPA compliance.
provider_name: Demostack
provider_slug: demostack
slug: demostack-trust-center
source_filename: demostack-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nsource: https://www.demostack.com/trust-center\nurl: https://www.demostack.com/trust-center\ndescription: >-\n  Demostack publishes a trust center on its own marketing site rather than a\n  hosted trust portal (no Vanta/Drata/SafeBase instance, no subprocessor list, no\n  document request flow). It names its attestation, auditor and effective date,\n  its privacy posture, its HIPAA position, its scanning and pentest tooling, and\n  its vulnerability disclosure program.\ncertifications:\n  - name: SOC 2 Type II\n    auditor: PwC\n    effective: '2023-10-31'\n    opinion: unqualified\n    statement: >-\n      \"Demostack has earned its SOC 2 attestation with PWC, effective October 31,\n      2023. The Auditor's report is 'unqualified,' meaning no control gaps were\n      identified.\"\n    note: >-\n      Demostack's own product-updates copy names it \"SOC 2 Type II compliance\n      through an audit by PwC\". The effective\
  \ date is 2023-10-31; no more recent\n      report period is published.\n  - name: HIPAA\n    role: Business Associate\n    statement: >-\n      \"Demostack is compliant with the HIPAA Privacy and Security standards as a\n      Business Associate, and we have the policies, procedures and systems\" to\n      protect ePHI.\n  - name: GDPR\n    statement: >-\n      \"Demostack recognizes the importance of Privacy and Data Protection\n      regulations such as GDPR and CCPA, and aligns with these and other\n      frameworks. We promote Privacy by Design.\"\n    dpa: Data Processing Agreement based on post-Schrems II Standard Contractual Clauses.\n  - name: CCPA\n    statement: Named alongside GDPR as a framework Demostack aligns with.\nnot_claimed:\n  - ISO 27001\n  - ISO 27017\n  - ISO 27018\n  - PCI DSS\n  - FedRAMP\n  - CSA STAR\nsecurity_posture:\n  encryption: Data encrypted at rest and in flight.\n  data_sales: '\"We never sell your data to any third party.\"'\n  continuous_scanning:\
  \ [Google Security Command Center, Snyk]\n  penetration_testing: HackerOne\n  vulnerability_disclosure: security/demostack-vulnerability-disclosure.yml\n  platform_controls: [SSO, RBAC]\n  platform_controls_source: https://www.demostack.com/pricing\ntransparency:\n  status_page: https://status.demostack.com/\n  availability_statistics: 90-day availability published on the status page\ngaps:\n  - No subprocessor list published.\n  - No document request / NDA flow for the SOC 2 report.\n  - No hosted trust portal (trust.demostack.com does not resolve).\n  - The published SOC 2 effective date is 2023-10-31 with no newer period named.\nevidence:\n  - source: https://www.demostack.com/trust-center\n    http_status: 200\n    keywords: [soc 2, pwc, hipaa, gdpr, ccpa, hackerone, snyk, vulnerability disclosure program]\n  - source: https://www.demostack.com/security\n    http_status: 200\n    keywords: [soc 2, trust center]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demostack/refs/heads/main/security/demostack-trust-center.yml
summary_line: SOC 2 Type II, HIPAA, GDPR, CCPA
tags:
- Sales Demo
- Demo Automation
- Product Simulation
- Webhook
- CRM Integration
- Sales Enablement
- Presales
- Sales Engineering
- Analytics
- Artificial Intelligence
- MCP
trust_url: https://www.demostack.com/trust-center
---
