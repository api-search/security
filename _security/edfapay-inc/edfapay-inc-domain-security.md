---
api_specs:
- filename: edfapay-inc-revamp.json
  format: json
  label: EdfaPay Management API
  slug: edfapay-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edfapay-inc/refs/heads/main/openapi/edfapay-inc-revamp.json
- filename: edfapay-inc-payment-initiate.json
  format: json
  label: EdfaPay Payment Gateway API
  slug: edfapay-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edfapay-inc/refs/heads/main/openapi/edfapay-inc-payment-initiate.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: edfapay.com
  spf: true
hosts:
- cert_expires: Sep  4 22:02:28 2026 GMT
  host: edfapay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 10:49:05 2026 GMT
  host: apidev.edfapay.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 21 10:49:05 2026 GMT
  host: revamp-api.edfapay.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Edfapay Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EdfaPay, Inc., probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EdfaPay, Inc.
provider_slug: edfapay-inc
slug: edfapay-inc-domain-security
source_filename: edfapay-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edfapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:02:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidev.edfapay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 10:49:05 2026 GMT\n  hsts: null\n- host: revamp-api.edfapay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 10:49:05 2026 GMT\n  hsts: null\ndomains:\n- domain: edfapay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edfapay-inc/refs/heads/main/security/edfapay-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payment Gateway
- Fintech
- SoftPOS
- Apple Pay
- Saudi Arabia
- Merchant Onboarding
---
