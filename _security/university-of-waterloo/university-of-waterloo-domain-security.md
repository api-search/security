---
api_specs:
- filename: university-of-waterloo-open-data-api.yaml
  format: yaml
  label: University of Waterloo Open Data API (v3)
  slug: open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-open-data-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uwaterloo.ca
  spf: true
hosts:
- cert_expires: Aug  3 00:36:52 2026 GMT
  host: uwaterloo.ca
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: openapi.data.uwaterloo.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Waterloo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Waterloo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Waterloo
provider_slug: university-of-waterloo
slug: university-of-waterloo-domain-security
source_filename: university-of-waterloo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uwaterloo.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  3 00:36:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: openapi.data.uwaterloo.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: uwaterloo.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/security/university-of-waterloo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Canada
- Research
---
