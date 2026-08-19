---
api_specs:
- filename: clevergy-connect-api-openapi.yml
  format: yaml
  label: Clevergy Connect API
  slug: clevergy-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevergy/refs/heads/main/openapi/clevergy-connect-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clever.gy
  spf: true
hosts:
- cert_expires: Sep 19 15:35:24 2026 GMT
  host: clever.gy
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 02:20:34 2026 GMT
  host: connect.clever.gy
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clevergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clevergy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clevergy
provider_slug: clevergy
slug: clevergy-domain-security
source_filename: clevergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clever.gy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:35:24 2026 GMT\n  hsts: false\n- host: connect.clever.gy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:20:34 2026 GMT\n  hsts: null\ndomains:\n- domain: clever.gy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevergy/refs/heads/main/security/clevergy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate Tech
- Energy
- Energy Management
- Utilities
- Smart Meter
- Solar
- Home Energy
- Battery Storage
- Electric Vehicle Charging
- Smart Home
- Sustainability
- Spain
- White Label
- Embedded Components
- Webhooks
---
