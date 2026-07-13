---
api_specs:
- filename: spin-ai-openapi.yml
  format: yaml
  label: Spin.AI SpinOne API
  slug: spin-ai-spinone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spin-ai/refs/heads/main/openapi/spin-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spin.ai
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.spin.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: spin.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: apg-1.spin.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spin Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spin.AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spin.AI
provider_slug: spin-ai
slug: spin-ai-domain-security
source_filename: spin-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: spin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apg-1.spin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spin.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spin-ai/refs/heads/main/security/spin-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Backup
- Compliance
- Data Protection
- Ransomware
- SaaS Security
---
