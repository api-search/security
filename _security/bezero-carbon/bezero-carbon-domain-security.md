---
api_specs:
- filename: bezero-carbon-projects-api-openapi.yml
  format: yaml
  label: BeZero Carbon Projects API
  slug: bezero-carbon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bezero-carbon/refs/heads/main/openapi/bezero-carbon-projects-api-openapi.yml
- filename: bezero-carbon-ratings-api-openapi.yml
  format: yaml
  label: BeZero Carbon Ratings API
  slug: bezero-carbon-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bezero-carbon/refs/heads/main/openapi/bezero-carbon-ratings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bezerocarbon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bezerocarbonmarkets.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: bezerocarbon.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api-docs.bezerocarbonmarkets.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.bezerocarbonmarkets.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bezero Carbon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BeZero Carbon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BeZero Carbon
provider_slug: bezero-carbon
slug: bezero-carbon-domain-security
source_filename: bezero-carbon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bezerocarbon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-docs.bezerocarbonmarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\n- host: api.bezerocarbonmarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bezerocarbon.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bezerocarbonmarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bezero-carbon/refs/heads/main/security/bezero-carbon-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Carbon Ratings
- Carbon Markets
- Climate
- Sustainability
- ESG
- Ratings
- Reference Data
- Market Intelligence
- Risk Analysis
---
