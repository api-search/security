---
api_specs:
- filename: rentcheck-openapi-original.yml
  format: yaml
  label: RentCheck REST API
  slug: rentcheck-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentcheck/refs/heads/main/openapi/rentcheck-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getrentcheck.com
  spf: true
hosts:
- cert_expires: Oct 16 01:51:09 2026 GMT
  host: getrentcheck.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: prod-public-api.getrentcheck.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentcheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RentCheck, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: RentCheck
provider_slug: rentcheck
slug: rentcheck-domain-security
source_filename: rentcheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getrentcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 01:51:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod-public-api.getrentcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getrentcheck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentcheck/refs/heads/main/security/rentcheck-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Property Management
- Property Inspection
- Real Estate
- PropTech
- Inspections
- Maintenance
- Rental
---
