---
api_specs:
- filename: prosper-ai-voice-openapi.json
  format: json
  label: Prosper Voice API
  slug: prosper-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/openapi/prosper-ai-voice-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getprosperapp.com
  spf: true
hosts:
- cert_expires: Sep 24 21:27:11 2026 GMT
  host: docs.getprosperapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:27:11 2026 GMT
  host: voice.getprosperapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prosper Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prosper AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Prosper AI
provider_slug: prosper-ai
slug: prosper-ai-domain-security
source_filename: prosper-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.getprosperapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:27:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: voice.getprosperapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:27:11 2026 GMT\n  hsts: null\ndomains:\n- domain: getprosperapp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/security/prosper-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Voice AI
- Revenue Cycle Management
- Patient Access
- EHR Integration
- AI Agents
- MCP
---
