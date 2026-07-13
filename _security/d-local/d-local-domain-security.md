---
api_specs:
- filename: d-local-payments-api-openapi.yml
  format: yaml
  label: dLocal Payments API
  slug: d-local-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-payments-api-openapi.yml
- filename: d-local-refunds-api-openapi.yml
  format: yaml
  label: dLocal Refunds API
  slug: d-local-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-refunds-api-openapi.yml
- filename: d-local-cards-api-openapi.yml
  format: yaml
  label: dLocal Cards API
  slug: d-local-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-cards-api-openapi.yml
- filename: d-local-payouts-v3-api-openapi.yml
  format: yaml
  label: dLocal Payouts V3 API
  slug: d-local-payouts-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-payouts-v3-api-openapi.yml
- filename: d-local-platforms-api-openapi.yml
  format: yaml
  label: dLocal For Platforms API
  slug: d-local-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-platforms-api-openapi.yml
- filename: d-local-kyc-verifications-api-openapi.yml
  format: yaml
  label: dLocal KYC Verifications API
  slug: d-local-kyc-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-kyc-verifications-api-openapi.yml
- filename: d-local-chargebacks-api-openapi.yml
  format: yaml
  label: dLocal Chargebacks API
  slug: d-local-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-chargebacks-api-openapi.yml
- filename: d-local-enrollments-api-openapi.yml
  format: yaml
  label: dLocal Enrollments API
  slug: d-local-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-enrollments-api-openapi.yml
- filename: d-local-exchange-rates-api-openapi.yml
  format: yaml
  label: dLocal Exchange Rates API
  slug: d-local-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/openapi/d-local-exchange-rates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dlocal.com
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: dlocal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 09:17:29 2026 GMT
  host: docs.dlocal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: api.dlocal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: D Local Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dLocal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: dLocal
provider_slug: d-local
slug: d-local-domain-security
source_filename: d-local-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\n- host: docs.dlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:17:29 2026 GMT\n  hsts: null\n- host: api.dlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dlocal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-local/refs/heads/main/security/d-local-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Payouts
- EmergingMarkets
- LatAm
- Africa
- Asia
- FX
- Fintech
---
