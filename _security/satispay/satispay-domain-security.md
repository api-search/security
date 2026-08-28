---
api_specs:
- filename: satispay-gbusiness-api.json
  format: json
  label: Satispay GBusiness API
  slug: satispay-gbusiness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/satispay/refs/heads/main/openapi/satispay-gbusiness-api.json
- filename: satispay-production.json
  format: json
  label: Satispay GBusiness API (production surface)
  slug: satispay-gbusiness-production
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/satispay/refs/heads/main/openapi/satispay-production.json
- filename: satispay-sandbox.json
  format: json
  label: Satispay GBusiness API (sandbox)
  slug: satispay-gbusiness-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/satispay/refs/heads/main/openapi/satispay-sandbox.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: satispay.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.satispay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:25:48 2026 GMT
  host: developers.satispay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: authservices.satispay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Satispay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Satispay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Satispay
provider_slug: satispay
slug: satispay-domain-security
source_filename: satispay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.satispay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.satispay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:25:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: authservices.satispay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: satispay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/satispay/refs/heads/main/security/satispay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Mobile Payments
- Fintech
- E-Money
- E-Commerce
- Italy
- Europe
- Merchant Services
- Recurring Payments
- Refunds
- Meal Vouchers
- Company
---
