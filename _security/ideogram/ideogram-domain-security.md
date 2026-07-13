---
api_specs:
- filename: ideogram-openapi.yml
  format: yaml
  label: Ideogram API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ideogram/refs/heads/main/openapi/ideogram-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ideogram.ai
  spf: true
hosts:
- cert_expires: Aug 16 18:04:43 2026 GMT
  host: ideogram.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 06:45:40 2026 GMT
  host: docs.ideogram.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 18:04:43 2026 GMT
  host: api.ideogram.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ideogram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ideogram, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ideogram
provider_slug: ideogram
slug: ideogram-domain-security
source_filename: ideogram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ideogram.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:04:43 2026 GMT\n  hsts: false\n- host: docs.ideogram.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 06:45:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ideogram.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:04:43 2026 GMT\n  hsts: null\ndomains:\n- domain: ideogram.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ideogram/refs/heads/main/security/ideogram-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Image Generation
- Text
- Realistic
- Editing
---
