---
api_specs:
- filename: phonepe-openapi.yml
  format: yaml
  label: PhonePe Payment Gateway API
  slug: pg
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonepe/refs/heads/main/openapi/phonepe-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: phonepe.com
  spf: true
hosts:
- cert_expires: Dec  3 09:12:59 2026 GMT
  host: www.phonepe.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 09:12:59 2026 GMT
  host: developer.phonepe.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 09:12:59 2026 GMT
  host: api.phonepe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phonepe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PhonePe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PhonePe
provider_slug: phonepe
slug: phonepe-domain-security
source_filename: phonepe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.phonepe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 09:12:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: developer.phonepe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 09:12:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.phonepe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 09:12:59 2026 GMT\n  hsts: null\ndomains:\n- domain: phonepe.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phonepe/refs/heads/main/security/phonepe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- UPI
- QR
- EDC
- App Store
- Fintech
- India
---
