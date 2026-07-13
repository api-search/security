---
api_specs:
- filename: ludo-ai-rest-api-openapi.yml
  format: yaml
  label: Ludo.ai REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/openapi/ludo-ai-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ludo.ai
  spf: true
hosts:
- cert_expires: Sep 16 11:59:49 2026 GMT
  host: ludo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:00:10 2026 GMT
  host: api.ludo.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 09:08:06 2026 GMT
  host: mcp.ludo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ludo Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ludo.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ludo.ai
provider_slug: ludo-ai
slug: ludo-ai-domain-security
source_filename: ludo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ludo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:59:49 2026 GMT\n  hsts: false\n- host: api.ludo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: mcp.ludo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:08:06 2026 GMT\n  hsts: null\ndomains:\n- domain: ludo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ludo-ai/refs/heads/main/security/ludo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Asset Generation
- Game Design
- Game Development
---
