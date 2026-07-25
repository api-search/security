---
api_specs:
- filename: paystone-datacandy-openapi.yml
  format: yaml
  label: Paystone DataCandy API
  slug: paystone-datacandy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/openapi/paystone-datacandy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paystone.com
  spf: true
hosts:
- cert_expires: Sep 26 17:32:29 2026 GMT
  host: www.paystone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 23:59:59 2026 GMT
  host: api.paystone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paystone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paystone, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paystone
provider_slug: paystone
slug: paystone-domain-security
source_filename: paystone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paystone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:32:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.paystone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paystone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paystone/refs/heads/main/security/paystone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Canada
- Payment Processing
- Acquiring
- Gift Cards
- Loyalty
- Subscriptions
- Billing
- Merchant Services
---
