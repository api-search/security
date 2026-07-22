---
api_specs:
- filename: vectranetworks-rux-v3.3-openapi.yml
  format: yaml
  label: Vectra AI Platform API (RUX)
  slug: vectra-ai-platform-api-rux
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-rux-v3.3-openapi.yml
- filename: vectranetworks-detect-v2.3-openapi.yml
  format: yaml
  label: Vectra Detect API
  slug: vectra-detect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-detect-v2.3-openapi.yml
certifications: []
description: Vectra AI operates a trust center at trust.vectra.ai. The hostname CNAMEs to trust.cname.drata.com (Drata Trust Center) and the endpoint answers HTTP 403 to non-browser clients (bot-gated), so the certification list could not be read programmatically. No named certifications are asserted here — only the verified existence and platform of the trust center. The security-programs probe found no security.txt, and no public bug-bounty program page on HackerOne/Bugcrowd/Intigriti was verified.
kind: trust-center
layout: security
name: Vectranetworks Trust Center
name_suffix: Trust Center
overview: Vectra AI maintains a public trust center covering its security and compliance posture.
provider_name: Vectra AI
provider_slug: vectranetworks
slug: vectranetworks-trust-center
source_filename: vectranetworks-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: DNS CNAME lookup of trust.vectra.ai + HTTP probe\ndescription: >-\n  Vectra AI operates a trust center at trust.vectra.ai. The hostname CNAMEs to\n  trust.cname.drata.com (Drata Trust Center) and the endpoint answers HTTP 403\n  to non-browser clients (bot-gated), so the certification list could not be\n  read programmatically. No named certifications are asserted here — only the\n  verified existence and platform of the trust center. The security-programs\n  probe found no security.txt, and no public bug-bounty program page on\n  HackerOne/Bugcrowd/Intigriti was verified.\ntrust_center:\n  url: https://trust.vectra.ai/\n  platform: Drata Trust Center\n  evidence:\n  - 'DNS: trust.vectra.ai CNAME trust.cname.drata.com'\n  - 'HTTP: 403 (bot-gated) at fetch time'\ncertifications: []\nnotes: Certifications listed inside the gated trust center were not verifiable in this pass; do not treat the empty list as an absence claim.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/security/vectranetworks-trust-center.yml
summary_line: trust center published
tags:
- Company
- Cybersecurity
- Network Detection and Response
- Threat Detection
- Security Operations
- Artificial Intelligence
- SIEM
trust_url: ''
---
