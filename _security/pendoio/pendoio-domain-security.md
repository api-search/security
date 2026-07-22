---
api_specs:
- filename: pendoio-engage-openapi.yml
  format: yaml
  label: Pendo Engage API
  slug: pendo-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-engage-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pendo.io
  spf: true
hosts:
- cert_expires: Oct 17 04:14:07 2026 GMT
  host: app.pendo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 03:58:57 2026 GMT
  host: us1.app.pendo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 07:17:23 2026 GMT
  host: app.eu.pendo.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pendoio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pendo.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pendo.io
provider_slug: pendoio
slug: pendoio-domain-security
source_filename: pendoio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.pendo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 04:14:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: us1.app.pendo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 03:58:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.eu.pendo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 07:17:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pendo.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/security/pendoio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Product Analytics
- Product Experience
- Digital Adoption
- User Analytics
- In-App Guidance
- Customer Feedback
- SaaS
---
