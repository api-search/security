---
certifications:
- SOC 2
- GDPR
description: ''
kind: trust-center
layout: security
name: Commsor Trust Center
name_suffix: Trust Center
overview: Commsor maintains a public trust center documenting SOC 2 and GDPR compliance.
provider_name: Commsor
provider_slug: commsor
slug: commsor-trust-center
source_filename: commsor-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nurl: https://www.commsor.com/security\ntype: security-page\nsummary: >-\n  Commsor does not operate a dedicated trust center (no trust.commsor.com,\n  security.commsor.com, Vanta/Drata/SafeBase portal, and no public document\n  request flow). It publishes a single security page on the marketing site that\n  names two compliance postures — SOC 2 and GDPR — in prose, without report\n  dates, auditor, Type I/II designation, scope, or a downloadable report.\ncertifications:\n- name: SOC 2\n  claimed: true\n  type: null\n  report_available: false\n  auditor: null\n  statement: 'Commsor is SOC 2 compliant, ensuring our systems meet rigorous standards\n    for security, availability, and confidentiality.'\n- name: GDPR\n  claimed: true\n  report_available: false\n  statement: 'We are fully GDPR compliant and uphold the principles of data protection\n    for all users, especially those in the EU.'\nnot_claimed:\n- ISO 27001\n\
  - ISO 27017\n- ISO 27018\n- PCI DSS\n- HIPAA\n- FedRAMP\n- CSA STAR\n- SOC 3\ninfrastructure_statements:\n- 'Our infrastructure is hosted with trusted cloud providers that offer strong physical\n  and network security.'\n- 'Access to production environments is limited to authorized personnel and monitored\n  continuously.'\nprobed_hosts:\n- {url: 'https://trust.commsor.com/', found: false}\n- {url: 'https://security.commsor.com/', found: false}\n- {url: 'https://www.commsor.com/security', found: true, http_status: 200}\nevidence:\n- source: https://www.commsor.com/security\n  keywords: [soc 2, gdpr, compliance, security]\n  fetched: '2026-08-04'\ngaps:\n- SOC 2 claimed but no Type designation, audit window, auditor, or report-request flow.\n- No subprocessor list, no data-residency statement, no encryption specifics.\n- No named cloud provider(s).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commsor/refs/heads/main/security/commsor-trust-center.yml
summary_line: SOC 2, GDPR
tags:
- Company
- Sales
- Marketing
- Go To Network
- Referrals
- Relationship Intelligence
- Revenue Operations
- Community
- B2B
trust_url: https://www.commsor.com/security
---
