---
api_specs:
- filename: nightfall-ai-openapi.yml
  format: yaml
  label: Nightfall AI
  slug: nightfall-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nightfall-ai/refs/heads/main/openapi/nightfall-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nightfall.ai
  spf: true
hosts:
- cert_expires: Sep 29 04:39:52 2026 GMT
  host: www.nightfall.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.nightfall.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nightfall Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nightfall AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nightfall AI
provider_slug: nightfall-ai
slug: nightfall-ai-domain-security
source_filename: nightfall-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nightfall.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:39:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nightfall.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nightfall.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nightfall-ai/refs/heads/main/security/nightfall-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Privacy
- Sensitive Data
---
