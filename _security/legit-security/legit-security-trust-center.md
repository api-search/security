---
certifications: []
description: ''
kind: trust-center
layout: security
name: Legit Security Trust Center
name_suffix: Trust Center
overview: Legit Security maintains a public trust center covering its security and compliance posture.
provider_name: Legit Security
provider_slug: legit-security
slug: legit-security-trust-center
source_filename: legit-security-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nurl: https://trust.legitsecurity.com/\nplatform: Scytale (trustcenter.scytale.ai)\nmirror: https://trustcenter.scytale.ai/legitsecurity\ncertifications: []\nevidence:\n- source: https://trust.legitsecurity.com/\n  status: 200\n  kind: trust-center\n  detail: >-\n    Page title \"Trust Center\"; served from a Scytale-hosted single-page app\n    (api.scytale.ai / trustcenter.scytale.ai). Verified reachable 2026-07-19.\n- source: https://trustcenter.scytale.ai/legitsecurity\n  status: 200\n  kind: trust-center-mirror\nnotes: >-\n  The trust center is client-rendered and gates its document/certification list\n  behind the SPA, so no named certifications could be verified from the public\n  HTML or bundle. certifications[] is deliberately empty rather than guessed —\n  no Compliance pointer is emitted until a certification is verified.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legit-security/refs/heads/main/security/legit-security-trust-center.yml
summary_line: trust center published
tags:
- Company
- Cybersecurity
- Application Security
- ASPM
- DevSecOps
- Software Supply Chain Security
- Secrets Detection
- SAST
- SCA
- Compliance
- AI Security
- MCP
trust_url: https://trust.legitsecurity.com/
---
