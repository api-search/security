---
certification_count: 4
certifications:
- SOC 1
- SOC 2
- ISO 27001
- ISO 27701
description: ''
kind: trust-center
layout: security
name: Agiloft Trust Center
name_suffix: Trust Center
overview: Agiloft maintains a public trust center documenting SOC 1, SOC 2, ISO 27001, and ISO 27701 compliance.
provider_name: Agiloft
provider_slug: agiloft
slug: agiloft-trust-center
source_filename: agiloft-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nprobe: true\nurl: https://www.agiloft.com/terms-policies/security\nnote: >-\n  Agiloft has no separate trust.agiloft.com portal (the host does not resolve). Its security and\n  compliance posture is published as a page in the Terms & Policies directory on the main site.\n  Certifications below were read from that page directly; the automated probe additionally matched\n  HIPAA and GDPR, which on that page refer to AWS's compliance as Agiloft's hosting provider rather\n  than to Agiloft's own attestations, so they are recorded separately under hosting_provider.\ncertifications:\n- SOC 1\n- SOC 2\n- ISO 27001\n- ISO 27701\nhosting_provider:\n  provider: AWS\n  claims_on_page: [SSAE 18, SOC 2 Type 2, HIPAA, GDPR]\n  note: >-\n    These are AWS's compliance claims, cited on Agiloft's security page as properties of the\n    hosting infrastructure. They are not Agiloft attestations and are kept out of the\n    certifications list on purpose.\n\
  practices:\n- >-\n    Third-party penetration assessments of the Agiloft application and hosting infrastructure,\n    performed annually and after every major upgrade, using both manual and automated techniques\n    to search for technical vulnerabilities.\n- Fully redundant AWS hosting, available inside or outside the USA.\nrelated_policies:\n- {name: Security, url: 'https://www.agiloft.com/terms-policies/security'}\n- {name: Data Processing Addendum, url: 'https://www.agiloft.com/terms-policies/data-processing-addendum'}\n- {name: EU Data Act Addendum, url: 'https://www.agiloft.com/terms-policies/eu-data-act-addendum'}\n- {name: Subprocessor List, url: 'https://www.agiloft.com/terms-policies/subprocessor-list'}\n- {name: Privacy Shield Notice, url: 'https://www.agiloft.com/terms-policies/privacy-shield-notice'}\n- {name: Service Level Addendum, url: 'https://www.agiloft.com/terms-policies/service-level-addendum'}\n- {name: Terms & Policies directory, url: 'https://www.agiloft.com/terms-policies'}\n\
  evidence:\n- source: https://www.agiloft.com/terms-policies/security\n  http_status: 200\n  fetched: '2026-09-12'\n  quote: >-\n    \"With SOC 1, SOC 2, ISO 27001, and ISO 27701 certification, Agiloft's customers can be\n    confident that their data is secure.\"\nvulnerability_disclosure:\n  published: false\n  note: >-\n    No security.txt (404 on every host), no bug bounty program on HackerOne, Bugcrowd or Intigriti,\n    and no responsible-disclosure or vulnerability-disclosure page — /responsible-disclosure,\n    /security/responsible-disclosure and /vulnerability-disclosure all 404 on www.agiloft.com. The\n    security page describes penetration testing but names no intake channel for an outside\n    reporter. No VulnerabilityDisclosure artifact is written and no Security-typed disclosure\n    pointer is emitted on that basis; the Security pointer in apis.yml points at the published\n    security policy page, which does exist.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agiloft/refs/heads/main/security/agiloft-trust-center.yml
summary_line: SOC 1, SOC 2, ISO 27001, ISO 27701
tags:
- Contract Lifecycle Management
- Contract Management
- Legal
- Procurement
- Enterprise Software
- No-Code
- Workflow-Automation
- Document Automation
- Webhook
- SCIM
- Company
trust_url: https://www.agiloft.com/terms-policies/security
---
