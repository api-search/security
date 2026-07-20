---
api_specs:
- filename: larridin-scout-openapi.yml
  format: yaml
  label: Larridin Scout API v1
  slug: scout-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/larridin/refs/heads/main/openapi/larridin-scout-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: larridin.com
  spf: true
hosts:
- cert_expires: Oct  4 21:03:03 2026 GMT
  host: larridin.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 13:46:16 2026 GMT
  host: docs.larridin.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 16:58:45 2026 GMT
  host: scout-api.larridin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Larridin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Larridin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Larridin
provider_slug: larridin
slug: larridin-domain-security
source_filename: larridin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: larridin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:03:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.larridin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:46:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: scout-api.larridin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:58:45 2026 GMT\n  hsts: null\ndomains:\n- domain: larridin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/larridin/refs/heads/main/security/larridin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Adoption
- AI Governance
- Analytics
- Developer Productivity
- Developer Intelligence
- Workflow Intelligence
- Enterprise Software
- Observability
---
