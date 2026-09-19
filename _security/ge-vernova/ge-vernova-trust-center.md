---
certification_count: 8
certifications:
- ISO 27001
- ISO 27017
- ISO 27018
- ISO 27701
- ISO 9001
- IEC 62443-4-1
- SOC 3
- SOC 3 Type 2
description: ''
kind: trust-center
layout: security
name: Ge Vernova Trust Center
name_suffix: Trust Center
overview: GE Vernova maintains a public trust center documenting ISO 27001, ISO 27017, ISO 27018, ISO 27701, ISO 9001, IEC 62443-4-1, SOC 3, and SOC 3 Type 2 compliance.
provider_name: GE Vernova
provider_slug: ge-vernova
slug: ge-vernova-trust-center
source_filename: ge-vernova-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nprobe: true\nurl: https://trust.gevernova.com/\nnote: >-\n  trust.gevernova.com resolves and returns HTTP 200. It is a Whistic-hosted trust portal delivered\n  as an Angular single-page application — the served HTML is a shell with an empty <title> and no\n  body text, and the SPA's own config endpoints are answered by the same catch-all shell, so the\n  certification inventory it renders could not be read by a non-browser client. The certifications\n  recorded below therefore come from the page GE Vernova serves as readable HTML, the\n  Electrification Software cybersecurity page, not from the trust portal.\nvendor: Whistic\ncertifications:\n  - ISO 27001\n  - ISO 27017\n  - ISO 27018\n  - ISO 27701\n  - ISO 9001\n  - IEC 62443-4-1\n  - SOC 3\n  - SOC 3 Type 2\nframeworks:\n  - NIST Cybersecurity Framework\ncompliance_page: https://www.gevernova.com/software/cybersecurity\ndetail: conformance/ge-vernova-conformance.yml\nevidence:\n\
  \  - source: https://trust.gevernova.com/\n    status: 200\n    keywords: [whistic]\n    note: SPA shell, no readable body content\n  - source: https://www.gevernova.com/software/cybersecurity\n    status: 200\n    keywords: [iso 27001, iec 62443, nist, soc 3, compliance, penetration testing]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ge-vernova/refs/heads/main/security/ge-vernova-trust-center.yml
summary_line: ISO 27001, ISO 27017, ISO 27018, ISO 27701, ISO 9001, IEC 62443-4-1, SOC 3, SOC 3 Type 2
tags:
- Decarbonization
- Electrification
- Energy
- Fortune 500
- Power
- Renewable Energy
- Sustainability
- Industrial
- Asset Performance Management
- Manufacturing Execution Systems
- Historian
- Grid
trust_url: https://trust.gevernova.com/
---
