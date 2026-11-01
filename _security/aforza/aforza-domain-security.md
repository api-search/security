---
api_specs:
- filename: aforza-user-management-openapi.json
  format: json
  label: User Management API
  slug: user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aforza/openapi/aforza-user-management-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aforza.com
  spf: true
hosts:
- cert_expires: Nov 25 17:30:19 2026 GMT
  host: aforza.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 05:09:12 2027 GMT
  host: developer.aforza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 07:07:58 2026 GMT
  host: api.aforza.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aforza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aforza, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aforza
provider_slug: aforza
slug: aforza-domain-security
source_filename: aforza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aforza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 17:30:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.aforza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 05:09:12 2027 GMT\n  hsts: false\n- host: api.aforza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 07:07:58 2026 GMT\n  hsts: null\ndomains:\n- domain: aforza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aforza/security/aforza-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- API
- Cloud
---
