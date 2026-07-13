---
api_specs:
- filename: pendo-openapi.yml
  format: yaml
  label: Pendo Engage API
  slug: engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendo/refs/heads/main/openapi/pendo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pendo.io
  spf: true
hosts:
- cert_expires: Sep  9 23:58:20 2026 GMT
  host: www.pendo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 21:48:40 2026 GMT
  host: engageapi.pendo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 18:58:34 2026 GMT
  host: app.pendo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pendo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pendo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pendo
provider_slug: pendo
slug: pendo-domain-security
source_filename: pendo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pendo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: engageapi.pendo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:48:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.pendo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:58:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pendo.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pendo/refs/heads/main/security/pendo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Product
- Analytics
- In-App Guidance
- Customer Success
- NPS
---
