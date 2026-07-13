---
api_specs:
- filename: imentiv-ai-openapi.yml
  format: yaml
  label: Imentiv AI API
  slug: imentiv-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imentiv-ai/main/openapi/imentiv-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: imentiv.ai
  spf: true
hosts:
- cert_expires: Sep 24 03:12:04 2026 GMT
  host: imentiv.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 21:23:35 2026 GMT
  host: api.imentiv.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imentiv Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imentiv AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Imentiv AI
provider_slug: imentiv-ai
slug: imentiv-ai-domain-security
source_filename: imentiv-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imentiv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.imentiv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:23:35 2026 GMT\n  hsts: null\ndomains:\n- domain: imentiv.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imentiv-ai/refs/heads/main/security/imentiv-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Emotion Detection
- Machine Learning
- Video Analysis
---
