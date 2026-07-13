---
api_specs:
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Charges API
  slug: tap-payments-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Authorize API
  slug: tap-payments-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Refunds API
  slug: tap-payments-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Customers API
  slug: tap-payments-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Tokens API
  slug: tap-payments-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Cards API
  slug: tap-payments-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Invoices API
  slug: tap-payments-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Payouts API
  slug: tap-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
- filename: tap-payments-openapi.yml
  format: yaml
  label: Tap Payments Business API
  slug: tap-payments-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/openapi/tap-payments-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_rua: mailto:email_dmarc_reports@tap.company
  dnssec: false
  domain: tap.company
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mailgun.org include:spf.mandrillapp.com include:mg.tap.com.kw ~all
hosts:
- cert_expires: Nov 29 13:20:39 2026 GMT
  cert_issuer: GoDaddy Secure Certificate Authority - G2
  host: www.tap.company
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 02:00:34 2026 GMT
  cert_issuer: Let's Encrypt
  host: developers.tap.company
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 11:12:48 2026 GMT
  cert_issuer: GoDaddy Secure Certificate Authority - G2
  host: api.tap.company
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  note: Bare host returns HTTP 404; the API base path is /v2. Fronted by an AWS ELB in eu-west-1.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tap Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tap Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tap Payments
provider_slug: tap-payments
slug: tap-payments-domain-security
source_filename: tap-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tap.company\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GoDaddy Secure Certificate Authority - G2\n  cert_expires: Nov 29 13:20:39 2026 GMT\n  hsts: false\n- host: developers.tap.company\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep  2 02:00:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tap.company\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: GoDaddy Secure Certificate Authority - G2\n  cert_expires: Dec  5 11:12:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  note: Bare host returns HTTP 404; the API base path is /v2. Fronted by an AWS ELB in eu-west-1.\ndomains:\n- domain: tap.company\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:mailgun.org include:spf.mandrillapp.com include:mg.tap.com.kw\
  \ ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: mailto:email_dmarc_reports@tap.company\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tap-payments/refs/heads/main/security/tap-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- Payment Gateway
- MENA
- Middle East
- Online Payments
- Charges
- Cards
- KNET
- mada
- Financial Infrastructure
---
