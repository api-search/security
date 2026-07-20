---
certifications: []
description: ''
kind: trust-center
layout: security
name: Attackiq Trust Center
name_suffix: Trust Center
overview: AttackIQ maintains a public trust center covering its security and compliance posture.
provider_name: AttackIQ
provider_slug: attackiq
slug: attackiq-trust-center
source_filename: attackiq-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nprobe: true\nurl: https://trust.attackiq.com/\ncertifications: []\nevidence:\n  - source: https://trust.attackiq.com/\n    status: 200\n    kind: trust-portal\n    note: >-\n      A dedicated trust portal is live at trust.attackiq.com (client-rendered\n      SPA, likely SafeBase/Vanta-class). The certification list is loaded via\n      JavaScript and could not be read server-side on this pass, so specific\n      named certifications (SOC 2 / ISO 27001 / etc.) are left UNVERIFIED rather\n      than asserted. Re-run with a headless fetch to enumerate certifications.\nnotes: >-\n  The portal's existence is verified; its contents are not. No `Compliance`\n  pointer is emitted because no named certification could be confirmed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attackiq/refs/heads/main/security/attackiq-trust-center.yml
summary_line: trust center published
tags:
- Company
- Security
- Cybersecurity
- Breach and Attack Simulation
- Continuous Threat Exposure Management
- Security Validation
- MITRE ATT&CK
- Threat Exposure Management
trust_url: https://trust.attackiq.com/
---
