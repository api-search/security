---
api_specs:
- filename: resemble-ai-openapi.yml
  format: yaml
  label: Resemble AI Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resemble-ai/refs/heads/main/openapi/resemble-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: resemble.ai
  spf: true
hosts:
- cert_expires: Sep 19 20:29:12 2026 GMT
  host: www.resemble.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 04:57:41 2026 GMT
  host: docs.resemble.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.resemble.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Resemble Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resemble AI, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Resemble AI
provider_slug: resemble-ai
slug: resemble-ai-domain-security
source_filename: resemble-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.resemble.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:29:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.resemble.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 04:57:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.resemble.ai\n  https: false\ndomains:\n- domain: resemble.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resemble-ai/refs/heads/main/security/resemble-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Voice
- TTS
- Voice Cloning
- Voice Conversion
- Audio
- Detection
---
