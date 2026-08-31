---
certifications:
- SOC 2 Type 2
- DORA
description: ''
kind: trust-center
layout: security
name: Keyrock Trust Center
name_suffix: Trust Center
overview: Keyrock maintains a public trust center documenting SOC 2 Type 2 and DORA compliance.
provider_name: Keyrock
provider_slug: keyrock
slug: keyrock-trust-center
source_filename: keyrock-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nprobe: true\nsource: https://trust.keyrock.com/\nurl: https://trust.keyrock.com/\nplatform: SafeBase\nhost_evidence:\n  dns: trust.keyrock.com CNAME keyrock.portals.safebase.io\n  note: >-\n    The subdomain is a SafeBase-provisioned tenant portal named for Keyrock, which is why this is\n    recorded as a real trust center rather than a speculative subdomain guess. A direct curl to\n    both trust.keyrock.com and keyrock.portals.safebase.io returns an HTTP 403 Cloudflare\n    interstitial; the portal contents below were read through a browser-class fetch that the edge\n    admitted. This is the ONLY Keyrock-controlled surface this pass was able to read end to end —\n    every keyrock.com HTML path, including a nonexistent control path, answers the same 403.\ncertifications:\n- name: SOC 2 Type 2\n  status: listed\n- name: DORA\n  full_name: Digital Operational Resilience Act (EU 2022/2554)\n  status: listed\ndocuments_listed:\n  policies:\n\
  \  - Acceptable Use Policy\n  - Access Control Policy\n  - AI System Development and Evaluation Policy\n  - Anti-Malicious Software Policy\n  - Asset Management Policy\n  - Audit and Accountability Policy\n  - Data Classification Policy\n  - Information Security Policy\n  - Password Policy\n  - Physical Security Policy\n  - Software Development Lifecycle Policy\n  corporate_security:\n  - Asset Management Practices\n  - Email Protection\n  - Employee Handbook\n  access: >-\n    Documents are listed publicly; retrieval is behind an \"Ask for information\" request form, the\n    standard SafeBase gated-document pattern.\nvulnerability_disclosure:\n  listed: false\n  note: >-\n    The trust center names no security contact, no disclosure policy and no bug bounty, and\n    keyrock.com serves no /.well-known/security.txt (404). No `Security` pointer is wired into\n    apis.yml, because there is nothing published to point at.\nevidence:\n- source: https://trust.keyrock.com/\n  http_status: 403\n\
  \  http_status_note: Cloudflare interstitial to curl; body read via browser-class fetch.\n  keywords:\n  - soc 2 type 2\n  - dora\n  - trust center\n- source: dns:CNAME trust.keyrock.com\n  value: keyrock.portals.safebase.io\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyrock/refs/heads/main/security/keyrock-trust-center.yml
summary_line: SOC 2 Type 2, DORA
tags:
- Company
- Market Making
- Liquidity
- Digital Assets
- Cryptocurrency
- Trading
- OTC
- Options
- Market Data
- Financial-Services
trust_url: https://trust.keyrock.com/
---
