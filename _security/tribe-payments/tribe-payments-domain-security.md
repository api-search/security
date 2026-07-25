---
api_specs:
- filename: tribe-payments-trb-cc-api-merchant-api-credit-card-v3.json
  format: json
  label: Payment Gateway - Credit Card API
  slug: gateway-credit-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-cc-api-merchant-api-credit-card-v3.json
- filename: tribe-payments-trb-hpp-api-merchant-api-hpp-v3.json
  format: json
  label: Payment Gateway - Hosted Payments API (HPP)
  slug: gateway-hosted-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-hpp-api-merchant-api-hpp-v3.json
- filename: tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-v3.json
  format: json
  label: Payment Gateway - Credit Card Token API
  slug: gateway-credit-card-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-cc-token-api-merchant-api-credit-card-token-v3.json
- filename: tribe-payments-trb-report-api-merchant-api-report-v3.json
  format: json
  label: Payment Gateway - Reports API
  slug: gateway-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-report-api-merchant-api-report-v3.json
- filename: tribe-payments-trb-isac-pos-tdd-device-api-openapi-device-directory-api-v3.json
  format: json
  label: Point of Sale - Device Directory API
  slug: pos-device-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-isac-pos-tdd-device-api-openapi-device-directory-api-v3.json
- filename: tribe-payments-trb-risk-monitor-client-api-openapi.json
  format: json
  label: Risk Monitor - Client API
  slug: risk-monitor-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-trb-risk-monitor-client-api-openapi.json
- filename: tribe-payments-obb-bank-api-openapi.json
  format: json
  label: Open Banking - Bank API
  slug: open-banking-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-obb-bank-api-openapi.json
- filename: tribe-payments-obb-tpp-api-openapi.json
  format: json
  label: Open Banking - Third-Party Providers API (TPP)
  slug: open-banking-tpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/openapi/tribe-payments-obb-tpp-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tribepayments.com
  spf: true
hosts:
- cert_expires: Sep 19 08:44:50 2026 GMT
  host: www.tribepayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 04:05:46 2026 GMT
  host: doc.tribepayments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Tribe Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tribe Payments, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tribe Payments
provider_slug: tribe-payments
slug: tribe-payments-domain-security
source_filename: tribe-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tribepayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:44:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.tribepayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:05:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: tribepayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tribe-payments/refs/heads/main/security/tribe-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- Issuer Processor
- Card Issuing
- Acquiring
- Payment Gateway
- Payment Processing
- Open Banking
- Account-to-Account
- Banking-as-a-Service
- Fraud
- Point of Sale
---
