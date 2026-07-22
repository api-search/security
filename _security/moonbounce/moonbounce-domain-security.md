---
api_specs:
- filename: moonbounce-openapi-original.json
  format: json
  label: Clavata Public API v1
  slug: clavata-public-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonbounce/refs/heads/main/openapi/moonbounce-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moonbounce.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clavata.ai
  spf: true
hosts:
- cert_expires: Oct 12 17:42:25 2026 GMT
  host: moonbounce.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: gateway.app.clavata.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moonbounce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moonbounce, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Moonbounce
provider_slug: moonbounce
slug: moonbounce-domain-security
source_filename: moonbounce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moonbounce.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 17:42:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.app.clavata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moonbounce.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: clavata.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonbounce/refs/heads/main/security/moonbounce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Content Moderation
- Trust And Safety
- AI Governance
- Policy Enforcement
- Content Evaluation
---
