---
api_specs:
- filename: travelers-openapi.yml
  format: yaml
  label: Travelers API
  slug: travelers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelers/refs/heads/main/openapi/travelers-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: travelers.com
  spf: true
hosts:
- cert_expires: Aug 14 03:07:59 2026 GMT
  host: www.travelers.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 19:38:53 2026 GMT
  host: developer.travelers.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 12:34:43 2026 GMT
  host: api.travelers.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Travelers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Travelers, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Travelers
provider_slug: travelers
slug: travelers-domain-security
source_filename: travelers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.travelers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:07:59 2026 GMT\n  hsts: false\n- host: developer.travelers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:38:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.travelers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 12:34:43 2026 GMT\n  hsts: null\ndomains:\n- domain: travelers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelers/refs/heads/main/security/travelers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Property Casualty
- Commercial Insurance
- Claims
- Fintech
- Fortune 500
---
