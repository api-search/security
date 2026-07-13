---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Limitless Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://api.limitless.ai/v1/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: limitless.ai
  spf: true
hosts:
- cert_expires: Oct  8 20:17:30 2026 GMT
  host: www.limitless.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:13:01 2026 GMT
  host: api.limitless.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Limitless Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Limitless, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Limitless
provider_slug: limitless-ai
slug: limitless-ai-domain-security
source_filename: limitless-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.limitless.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 20:17:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.limitless.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:13:01 2026 GMT\n  hsts: null\ndomains:\n- domain: limitless.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limitless-ai/refs/heads/main/security/limitless-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Wearable
- Pendant
- Meeting Notes
- Lifelogs
- Personal AI
- API
- MCP
- OpenAPI
---
