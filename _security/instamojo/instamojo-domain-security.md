---
api_specs:
- filename: instamojo-payments-api.yml
  format: yaml
  label: Instamojo Payments API
  slug: instamojo-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instamojo/refs/heads/main/openapi/instamojo-payments-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: instamojo.com
  spf: true
hosts:
- cert_expires: Aug 18 04:28:08 2026 GMT
  host: www.instamojo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:19:13 2026 GMT
  host: docs.instamojo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 00:57:32 2026 GMT
  host: api.instamojo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instamojo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instamojo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Instamojo
provider_slug: instamojo
slug: instamojo-domain-security
source_filename: instamojo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.instamojo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 04:28:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.instamojo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:19:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.instamojo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 00:57:32 2026 GMT\n  hsts: null\ndomains:\n- domain: instamojo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instamojo/refs/heads/main/security/instamojo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- E-Commerce
- India
- Payment Gateway
- Payment Links
- Refunds
- Orders
---
