---
api_specs:
- filename: dlocal-payouts-api-openapi.yml
  format: yaml
  label: dLocal Payouts API
  slug: dlocal-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-payouts-api-openapi.yml
- filename: dlocal-accounts-api-openapi.yml
  format: yaml
  label: dLocal Accounts API
  slug: dlocal-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-accounts-api-openapi.yml
- filename: dlocal-balance-api-openapi.yml
  format: yaml
  label: dLocal Balance API
  slug: dlocal-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-balance-api-openapi.yml
- filename: dlocal-bank-accounts-api-openapi.yml
  format: yaml
  label: dLocal Bank Accounts API
  slug: dlocal-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-bank-accounts-api-openapi.yml
- filename: dlocal-chargebacks-api-openapi.yml
  format: yaml
  label: dLocal Chargebacks API
  slug: dlocal-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-chargebacks-api-openapi.yml
- filename: dlocal-currency-api-openapi.yml
  format: yaml
  label: dLocal Currency API
  slug: dlocal-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-currency-api-openapi.yml
- filename: dlocal-documents-api-openapi.yml
  format: yaml
  label: dLocal Documents API
  slug: dlocal-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-documents-api-openapi.yml
- filename: dlocal-kyc-api-openapi.yml
  format: yaml
  label: dLocal KYC API
  slug: dlocal-kyc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-kyc-api-openapi.yml
- filename: dlocal-payment-methods-api-openapi.yml
  format: yaml
  label: dLocal Payment Methods API
  slug: dlocal-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-payment-methods-api-openapi.yml
- filename: dlocal-payments-api-openapi.yml
  format: yaml
  label: dLocal Payments API
  slug: dlocal-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-payments-api-openapi.yml
- filename: dlocal-payouts-api-openapi.yml
  format: yaml
  label: dLocal Payouts API
  slug: dlocal-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-payouts-api-openapi.yml
- filename: dlocal-refunds-api-openapi.yml
  format: yaml
  label: dLocal Refunds API
  slug: dlocal-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-refunds-api-openapi.yml
- filename: dlocal-tokens-api-openapi.yml
  format: yaml
  label: dLocal Tokens API
  slug: dlocal-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-tokens-api-openapi.yml
- filename: dlocal-transfers-api-openapi.yml
  format: yaml
  label: dLocal Transfers API
  slug: dlocal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-transfers-api-openapi.yml
- filename: dlocal-verifications-api-openapi.yml
  format: yaml
  label: dLocal Verifications API
  slug: dlocal-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/openapi/dlocal-verifications-api-openapi.yml
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
  host: www.dlocal.com
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
name: Dlocal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dLocal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: dLocal
provider_slug: dlocal
slug: dlocal-domain-security
source_filename: dlocal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\n- host: docs.dlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:17:29 2026 GMT\n  hsts: null\n- host: api.dlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dlocal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dlocal/refs/heads/main/security/dlocal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Emerging Markets
- Payins
- Payouts
- Fintech
- Latin America
- Africa
- Asia
- Local Payment Methods
- Payment Processing
---
