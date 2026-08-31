---
api_specs:
- filename: superb-ai-mlops-platform-openapi.json
  format: json
  label: Superb AI MLOps Platform API
  slug: superb-ai-mlops-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superb-ai/refs/heads/main/openapi/superb-ai-mlops-platform-openapi.json
certifications:
- SOC 2 Type II
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Superb Ai Trust Center
name_suffix: Trust Center
overview: Superb AI maintains a public trust center documenting SOC 2 Type II and ISO 27001 compliance.
provider_name: Superb AI
provider_slug: superb-ai
slug: superb-ai-trust-center
source_filename: superb-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://superb-ai.com/en/company/security\nurl: https://superb-ai.com/en/company/security\nname: Superb AI Security & Information Protection\nnote: >-\n  Superb AI publishes a security page rather than a hosted trust portal — there is no\n  trust.superb-ai.com (NXDOMAIN) and no Vanta/Drata/SafeBase-style portal. The page names two\n  third-party certifications and describes the encryption, backup and penetration-testing\n  program. It does NOT publish a vulnerability-disclosure policy, a security contact address or\n  a bug-bounty program, so no VulnerabilityDisclosure artifact and no `Security` pointer were\n  emitted.\ncertifications:\n- name: SOC 2 Type II\n  standard: AICPA SOC 2\n  evidence: >-\n    \"SOC-2 Type II, in particular, is the most comprehensive certification within the SOC\n    framework\" — https://superb-ai.com/en/company/security\n- name: ISO 27001\n  standard: ISO/IEC 27001 (Information Security Management\
  \ System)\n  evidence: >-\n    \"ISO 27001 is an international standard for Information Security Management Systems (ISMS)\n    issued by the International Organization for Standardization\" —\n    https://superb-ai.com/en/company/security\ncontrols:\n- area: encryption-at-rest\n  detail: All data encrypted using AES-256; AWS S3 and AWS Aurora RDS.\n- area: encryption-in-transit\n  detail: HTTPS for all communications.\n- area: key-management\n  detail: Encryption keys managed with AWS KMS.\n- area: backup\n  detail: Daily backups with 7-day retention; quarterly restoration testing; database replication servers.\n- area: penetration-testing\n  detail: >-\n    \"regularly engages top security experts to conduct network and application penetration\n    testing\"\nevidence:\n- url: https://superb-ai.com/en/company/security\n  status: 200\n  note: 260,189-byte page, title \"Trusted AI Data Security and Information Protection | Superb AI\".\n- url: https://trust.superb-ai.com\n  status: 0\n\
  \  note: DNS NXDOMAIN — no hosted trust portal.\nx-corrections:\n- date: '2026-08-29'\n  note: >-\n    probe-security-programs.py originally recorded https://superb-ai.com/en/trust and\n    https://superb-ai.com/en/security/responsible-disclosure as hits. Both are SOFT-404s — a\n    control probe of https://superb-ai.com/en/definitely-not-a-real-page-xyz returned the same\n    200 with an identical ~127.9KB body and the same generic title, and the SOC 2 / ISO 27001\n    strings that triggered the match come from the site-wide footer bundle present on every\n    page. Both were discarded and the trust-center source was corrected to the real security\n    page; the vulnerability-disclosure artifact was deleted outright.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superb-ai/refs/heads/main/security/superb-ai-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001
tags:
- Artificial Intelligence
- Machine-Learning
- Computer-Vision
- Data Labeling
- Annotation
- MLOps
- Training Data
- Model Training
- Inference
- Datasets
trust_url: https://superb-ai.com/en/company/security
---
