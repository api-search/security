---
api_specs:
- filename: beeper-desktop-api-openapi-original.yml
  format: yaml
  label: Beeper Desktop API
  slug: beeper-desktop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/openapi/beeper-desktop-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beeper.com
  spf: true
hosts:
- cert_expires: Oct  3 19:34:50 2026 GMT
  host: beeper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beeper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beeper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Beeper
provider_slug: beeper
slug: beeper-domain-security
source_filename: beeper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beeper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 19:34:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beeper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeper/refs/heads/main/security/beeper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Messaging
- Chat
- Communication
- Matrix
- MCP
- Desktop
- Aggregator
---
