---
certifications: []
description: ''
kind: trust-center
layout: security
name: Poka Trust Center
name_suffix: Trust Center
overview: Poka maintains a public trust center covering its security and compliance posture.
provider_name: Poka
provider_slug: poka
slug: poka-trust-center
source_filename: poka-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nprobe: true\nurl: https://trust.poka.io/\nplatform: Vanta\nevidence:\n  - source: dns\n    detail: trust.poka.io CNAME -> 69306f4cf86dbbb938cdaf3a.cname.vantatrust.com (Vanta-hosted Trust Center)\n  - source: https://trust.poka.io/\n    detail: live 200; Vanta Trust Center single-page app (\"Poka Trust Center\")\n  - source: https://www.poka.io/en/security-privacy-compliance\n    detail: Security & Compliance page referencing Security Overview, SLA, Master SaaS Agreement, Acceptable Use Policy; security contact infosec@poka.io\n# Named certifications are served by the Vanta SPA via authenticated/JS-rendered data and\n# were not machine-verifiable at probe time; left empty rather than fabricated.\ncertifications: []\ncontact: [infosec@poka.io]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poka/refs/heads/main/security/poka-trust-center.yml
summary_line: trust center published
tags:
- Company
- Manufacturing
- Connected Worker
- Frontline Operations
- Industrial
- Workforce Training
- Integrations
- SaaS
trust_url: https://trust.poka.io/
---
