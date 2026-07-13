---
api_specs:
- filename: robin-ai-openapi.yml
  format: yaml
  label: Robin Legal Intelligence Platform API
  slug: robin-legal-intelligence-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robin-ai/refs/heads/main/openapi/robin-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: robinai.com
  spf: true
hosts:
- cert_expires: Sep  2 04:35:58 2026 GMT
  host: robinai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.robinai.com
  https: false
kind: domain-security
layout: security
method: probed
name: Robin Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Robin AI, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Robin AI
provider_slug: robin-ai
slug: robin-ai-domain-security
source_filename: robin-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: robinai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 04:35:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.robinai.com\n  https: false\ndomains:\n- domain: robinai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robin-ai/refs/heads/main/security/robin-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Legal
- LegalTech
- Contract Review
- Contract Analysis
- Contract Lifecycle Management
- CLM
- Document Extraction
- Structured Data
- Legal AI
- Artificial Intelligence
- Word Add-In
- Playbook
- Redlining
- Obligation Tracking
- Anthropic
- Claude
---
