---
api_specs:
- filename: rhumbix-public-api-openapi-original.json
  format: json
  label: Rhumbix Public API
  slug: rhumbix-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhumbix/refs/heads/main/openapi/rhumbix-public-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rhumbix.com
  spf: true
hosts:
- cert_expires: Sep  4 04:22:19 2026 GMT
  host: www.rhumbix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: async-api.rhumbix.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rhumbix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rhumbix, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rhumbix
provider_slug: rhumbix
slug: rhumbix-domain-security
source_filename: rhumbix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rhumbix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 04:22:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: async-api.rhumbix.com\n  https: false\ndomains:\n- domain: rhumbix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhumbix/refs/heads/main/security/rhumbix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applications
- Construction
- Construction Technology
- Workforce Management
- Timekeeping
- Payroll
- Field Data Collection
- Project Management
- Job Costing
- Integrations
- REST API
---
