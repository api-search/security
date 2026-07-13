---
api_specs:
- filename: oas.json
  format: json
  label: Transcend API
  slug: transcend-api
  spec_type: OpenAPI
  url: https://docs.transcend.io/api/oas.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transcend.io
  spf: true
hosts:
- cert_expires: Sep 15 02:36:24 2026 GMT
  host: transcend.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 01:25:34 2026 GMT
  host: docs.transcend.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: api.transcend.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transcend Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transcend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transcend
provider_slug: transcend-io
slug: transcend-io-domain-security
source_filename: transcend-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transcend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:36:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.transcend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 01:25:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.transcend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: transcend.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcend-io/refs/heads/main/security/transcend-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transcend
- Privacy
- Data Governance
- Consent
- Preference Management
- DSR
- Data Inventory
- AI Governance
- GDPR
- CCPA
- Compliance
- Webhooks
- GraphQL
- MCP
- SDK
- Terraform
- Helm
---
