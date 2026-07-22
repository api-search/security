---
certifications: []
description: ''
kind: trust-center
layout: security
name: Exaforce Trust Center
name_suffix: Trust Center
overview: Exaforce maintains a public trust center covering its security and compliance posture.
provider_name: Exaforce
provider_slug: exaforce
slug: exaforce-trust-center
source_filename: exaforce-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://trust.exaforce.com/\nurl: https://trust.exaforce.com/\n# Exaforce publishes a hosted trust center at trust.exaforce.com (HTTP 200).\n# The page is a client-side (JS-rendered) trust portal, so specific named\n# certifications could not be extracted verbatim and are intentionally NOT\n# asserted here (no fabrication). A follow-up render is needed to capture any\n# SOC 2 / ISO 27001 / etc. claims before emitting a `Compliance` pointer.\ncertifications: []\nsecurity_contact: security@exaforce.com   # from exaforce.com CAA iodef record\nevidence:\n- source: https://trust.exaforce.com/\n  kind: trust-center\n  detail: hosted trust portal returns 200 with \"Exaforce Trust Center\" heading\n- source: security/exaforce-domain-security.yml\n  kind: caa-iodef\n  detail: 'CAA record: 0 iodef \"mailto:security@exaforce.com\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exaforce/refs/heads/main/security/exaforce-trust-center.yml
summary_line: trust center published
tags:
- Company
- Security
- Cybersecurity
- Security Operations
- SOC
- SIEM
- Threat Detection
- Incident Response
- Artificial Intelligence
- AI Agents
- Managed Detection and Response
- Cloud Security
trust_url: https://trust.exaforce.com/
---
