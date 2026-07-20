---
api_specs:
- filename: coperniq-openapi.yml
  format: yaml
  label: Coperniq API
  slug: coperniq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coperniq/refs/heads/main/openapi/coperniq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: coperniq.io
  spf: true
hosts:
- cert_expires: Oct  4 23:45:01 2026 GMT
  host: www.coperniq.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: api.coperniq.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coperniq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coperniq, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Coperniq
provider_slug: coperniq
slug: coperniq-domain-security
source_filename: coperniq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coperniq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:45:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coperniq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coperniq.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coperniq/refs/heads/main/security/coperniq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Climate
- Solar
- Construction
- Field Service Management
- Project Management
- Contractors
- CRM
- Energy
---
