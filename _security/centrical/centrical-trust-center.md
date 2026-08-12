---
certifications:
- ISO/IEC 27001
- ISO/IEC 27701
- SOC 2 Type II
- Cloud Security Alliance STAR Registry
- EU General Data Protection Regulation
- California Consumer Privacy Act
description: ''
kind: trust-center
layout: security
name: Centrical Trust Center
name_suffix: Trust Center
overview: Centrical maintains a public trust center documenting ISO/IEC 27001, ISO/IEC 27701, SOC 2 Type II, Cloud Security Alliance STAR Registry, EU General Data Protection Regulation, and California Consumer Privacy Act compliance.
provider_name: Centrical
provider_slug: centrical
slug: centrical-trust-center
source_filename: centrical-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: searched\nprobe: true\nsource: https://centrical.com/enterprise-level-security/\nnote: >-\n  Centrical serves no trust.centrical.com or security.centrical.com host (both NXDOMAIN) and no\n  hosted trust-center product. What it does publish is a single public security and compliance page\n  at the non-standard path /enterprise-level-security/ that names its certifications outright, plus\n  dedicated GDPR and CCPA disclosure pages. The automated probe\n  (0-working/probe-security-programs.py) missed it because it checks /trust, /security and\n  /compliance — this was found by reading the 197-URL page sitemap. Certifications are named but the\n  underlying reports are NOT published: the SOC 2 Type II report is available only on request to\n  privacy@centrical.com.\n\nurl: https://centrical.com/enterprise-level-security/\nhosted_trust_center: false\nlegal_entity: Biz-Effective Ltd.\n\ncertifications:\n- id: iso-27001\n  name: ISO/IEC 27001\n  scope:\
  \ Information Security Management\n  evidence: >-\n    \"ISO certification means customers can be confident that Centrical protects Personally\n    Identifiable Information in the cloud to the highest standards.\"\n  report_published: false\n- id: iso-27701\n  name: ISO/IEC 27701\n  scope: Privacy Information Management\n  evidence: Listed as a certification badge on the enterprise security page.\n  report_published: false\n- id: soc2-type-ii\n  name: SOC 2 Type II\n  auditor: Ernst & Young\n  evidence: >-\n    \"Centrical has been audited by Ernest Young and provided a report on its compliance with\n    Service Organization Control (SOC) 2 type II.\"\n  report_published: false\n  report_access: On request to privacy@centrical.com\n- id: csa-star\n  name: Cloud Security Alliance STAR Registry\n  evidence: >-\n    \"Centrical is on the Security Trust Assurance and Risk (STAR) registry of the Cloud Security\n    Alliance (CSA).\"\n  report_published: false\n- id: gdpr\n  name: EU General\
  \ Data Protection Regulation\n  evidence: >-\n    \"With customers in almost every country in the world, Centrical adheres to the General Data\n    Protection Regulation (GDPR).\" Dedicated page at /gdpr-compliant/.\n  url: https://centrical.com/gdpr-compliant/\n- id: ccpa\n  name: California Consumer Privacy Act\n  evidence: Dedicated CCPA disclosure page.\n  url: https://centrical.com/ccpa/\n\nprivacy_program:\n  dpa: true\n  sub_processor_list: true\n  vendor_risk_management: true\n  data_subject_request_process: true\n  annual_privacy_training: true\n  eu_data_residency: >-\n    \"Verified that all user data is stored and processes on EU hosted servers only\" — stated as a\n    GDPR compliance measure. Corroborated by the Europe region component group on\n    centrical.statuspage.io.\n\ncontact:\n  privacy: privacy@centrical.com\n\nnot_published:\n- Vulnerability disclosure or responsible-disclosure policy\n- Bug bounty program (no HackerOne / Bugcrowd / Intigriti presence found)\n\
  - /.well-known/security.txt (RFC 9116) — returns 404 on centrical.com\n- Penetration test summary\n- PCI DSS, HIPAA or FedRAMP authorization\n- Uptime/SLA commitment\n\nx-evidence:\n- {url: 'https://centrical.com/enterprise-level-security/', status: 200, checked: '2026-08-10'}\n- {url: 'https://centrical.com/gdpr-compliant/', status: 200, checked: '2026-08-09'}\n- {url: 'https://centrical.com/ccpa/', status: 200, checked: '2026-08-09'}\n- {url: 'https://centrical.com/.well-known/security.txt', status: 404, checked: '2026-08-10'}\n- {url: 'https://trust.centrical.com/', status: 0, checked: '2026-08-10', note: NXDOMAIN}\n- {url: 'https://security.centrical.com/', status: 0, checked: '2026-08-10', note: NXDOMAIN}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrical/refs/heads/main/security/centrical-trust-center.yml
summary_line: ISO/IEC 27001, ISO/IEC 27701, SOC 2 Type II, Cloud Security Alliance STAR Registry, EU General Data Protection Regulation, California Consumer Privacy Act
tags:
- Company
- Employee Engagement
- Performance Management
- Gamification
- Microlearning
- Contact Center
- Workforce Engagement Management
- Coaching
- Quality Management
- Human Resources
- SaaS
trust_url: https://centrical.com/enterprise-level-security/
---
