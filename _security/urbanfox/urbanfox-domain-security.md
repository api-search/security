---
api_specs:
- filename: urbanfox-customer-api-openapi.yml
  format: yaml
  label: UrbanFox Customer API
  slug: urbanfox-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanfox/refs/heads/main/openapi/urbanfox-customer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbanfox.io
  spf: true
hosts:
- cert_expires: Oct  4 23:49:03 2026 GMT
  host: urbanfox.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urbanfox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UrbanFox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UrbanFox
provider_slug: urbanfox
slug: urbanfox-domain-security
source_filename: urbanfox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbanfox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:49:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: urbanfox.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanfox/refs/heads/main/security/urbanfox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Detection
- Payment Fraud
- Account Takeover
- Bot Detection
- Risk Management
- Security
- Artificial Intelligence
- eCommerce
---
