---
api_specs:
- filename: funding-circle-introducer-openapi.yml
  format: yaml
  label: Funding Circle Introducer API
  slug: funding-circle-introducer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/funding-circle/refs/heads/main/openapi/funding-circle-introducer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fundingcircle.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.fundingcircle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Funding Circle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Funding Circle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Funding Circle
provider_slug: funding-circle
slug: funding-circle-domain-security
source_filename: funding-circle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fundingcircle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fundingcircle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funding-circle/refs/heads/main/security/funding-circle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Lending
- Small Business
- Fintech
- Loans
- Financial Services
- Payments
---
