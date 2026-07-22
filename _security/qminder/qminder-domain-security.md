---
api_specs:
- filename: qminder-openapi-original.json
  format: json
  label: Qminder REST API
  slug: qminder-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/openapi/qminder-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qminder.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: qminder.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.qminder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qminder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qminder, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qminder
provider_slug: qminder
slug: qminder-domain-security
source_filename: qminder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qminder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.qminder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: qminder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qminder/refs/heads/main/security/qminder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Queue Management
- Appointment Scheduling
- Visitor Management
- Customer Experience
- REST
- GraphQL
- Webhooks
- SaaS
---
