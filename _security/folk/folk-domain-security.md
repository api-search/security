---
api_specs:
- filename: openapi.json
  format: json
  label: Folk API
  slug: folk-api
  spec_type: OpenAPI
  url: https://developer.folk.app/api-reference/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: folk.app
  spf: true
hosts:
- cert_expires: Aug 16 14:59:43 2026 GMT
  host: www.folk.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 06:35:33 2026 GMT
  host: developer.folk.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api.folk.app
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Folk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Folk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Folk
provider_slug: folk
slug: folk-domain-security
source_filename: folk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.folk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 14:59:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.folk.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:35:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.folk.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: folk.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/security/folk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Contacts
- Pipelines
- Sales
- Relationships
- Notes
- Deals
- Webhooks
---
