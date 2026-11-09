---
api_specs:
- filename: footfally-com-api-openapi.json
  format: json
  label: Footfally API API
  slug: footfally-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/footfally-com/openapi/_original/footfally-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: footfally.com
  spf: true
hosts:
- cert_expires: Feb  1 01:32:25 2027 GMT
  host: footfally.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Footfally Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Footfally, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Footfally
provider_slug: footfally-com
slug: footfally-com-domain-security
source_filename: footfally-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: footfally.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 01:32:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: footfally.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/footfally-com/security/footfally-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Retail
- Scheduling
- Pricing
- Expenses
- SaaS
- Company
---
