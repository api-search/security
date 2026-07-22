---
api_specs:
- filename: vitally-rest-openapi.yml
  format: yaml
  label: Vitally REST API
  slug: vitally-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitally/refs/heads/main/openapi/vitally-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vitally.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vitally-eu.io
  spf: false
hosts:
- cert_expires: Sep 21 18:40:25 2026 GMT
  host: vitally.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: rest.vitally-eu.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vitally Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vitally, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vitally
provider_slug: vitally
slug: vitally-domain-security
source_filename: vitally-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vitally.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 18:40:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.vitally-eu.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vitally.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vitally-eu.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitally/refs/heads/main/security/vitally-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Success
- SaaS
- CRM
- NPS
- Surveys
- Analytics
- Artificial Intelligence
---
