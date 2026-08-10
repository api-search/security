---
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Vrify Trust Center
name_suffix: Trust Center
overview: VRIFY maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: VRIFY
provider_slug: vrify
slug: vrify-trust-center
source_filename: vrify-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://vrify.com/legal/security\ndocs:\n- https://vrify.com/legal/security\n- https://help.vrify.com/en/articles/11025335-data-security-at-vrify\n- https://vrify.com/articles/data-security-and-transparency-at-vrify\n\ntrust_center:\n  hosted: false\n  note: >-\n    VRIFY publishes no dedicated trust-center host (trust.vrify.com and\n    security.vrify.com do not resolve; vrify.com/trust, /security and /compliance\n    return 404). Its compliance posture is published as a legal page at\n    /legal/security plus a customer-facing help-centre article. The SOC 2 report\n    itself is not self-serve — it is released on request by email.\n  page: https://vrify.com/legal/security\n  page_last_modified: '2024-02-23'\n  report_request: mailto:info@vrify.com\n\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  scope: >-\n    All five Trust Services Criteria — security, availability, processing\n    integrity, confidentiality\
  \ and privacy — as of January 2026.\n  authority: AICPA\n  evidence: https://help.vrify.com/en/articles/11025335-data-security-at-vrify\n  quote: >-\n    \"As of January 2026, this certification covers all five SOC 2 Type II Trust\n    Services Criteria: security, availability, processing integrity,\n    confidentiality, and privacy.\"\n  report_available: on-request\n  report_contact: info@vrify.com\n\npractices:\n- area: security program\n  claim: >-\n    \"Our multi-layered security environment follows the principles of least\n    privilege, separation of duties, defense in depth, and usability.\"\n  source: https://vrify.com/legal/security\n- area: encryption at rest\n  claim: >-\n    Customer data is stored in AWS cloud databases and Amazon S3 buckets and\n    \"encrypted at rest using AES-256 encryption through AWS-native encryption\n    mechanisms\", covering databases, object storage and backups.\n  source: https://help.vrify.com/en/articles/11025335-data-security-at-vrify\n- area:\
  \ encryption in transit\n  claim: >-\n    Not stated on the security page. Observed at the edge: TLS 1.3 with HSTS\n    max-age 31536000 on vrify.com, and HSTS with includeSubDomains + preload on\n    services.vrify.com.\n  source: security/vrify-domain-security.yml\n- area: access control\n  claim: >-\n    \"Within the VRIFY cloud environment, access controls are tightly restricted\n    to authorized personnel only. All VRIFY employees complete regular security\n    training and device compliance checks.\"\n  source: https://help.vrify.com/en/articles/11025335-data-security-at-vrify\n- area: model training data\n  claim: >-\n    Geospatial data used to train VRIFY Predict models is anonymized in four\n    stages — data aggregation (company names and project specifications\n    stripped), unique numeric asset identifiers replacing names, coordinate\n    masking into a normalized index range, and conversion to a numerical image\n    matrix that retains no coordinates or project information.\n\
  \  source: https://help.vrify.com/en/articles/11025335-data-security-at-vrify\n- area: authoritative document\n  claim: >-\n    The help-centre security article explicitly disclaims contractual force; the\n    Client Terms of Service is named as the authoritative data-storage agreement.\n  source: https://vrify.com/legal/client-terms-of-service\n\ngaps:\n- No /.well-known/security.txt on vrify.com (404) — see well-known/vrify-well-known.yml.\n- No published vulnerability-disclosure policy, security contact, or bug-bounty program.\n- No subprocessor list published.\n- No self-serve trust portal; the SOC 2 report requires an email request.\n\nx-evidence:\n- url: https://vrify.com/legal/security\n  http_status: 200\n  fetched: '2026-08-05'\n- url: https://help.vrify.com/en/articles/11025335-data-security-at-vrify.md\n  http_status: 200\n  fetched: '2026-08-05'\n- url: https://vrify.com/security\n  http_status: 404\n  fetched: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vrify/refs/heads/main/security/vrify-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Company
- Mining
- Mineral Exploration
- Geoscience
- Artificial Intelligence
- Machine Learning
- 3D Visualization
- Data Visualization
- Investor Relations
- SaaS
- Canada
trust_url: ''
---
