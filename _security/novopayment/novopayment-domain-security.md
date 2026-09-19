---
api_specs:
- filename: novopayment-accounts-openapi.yml
  format: yaml
  label: NovoPayment Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-accounts-openapi.yml
- filename: novopayment-alias-directory-openapi.yml
  format: yaml
  label: NovoPayment Alias Directory API
  slug: alias-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-alias-directory-openapi.yml
- filename: novopayment-cards-openapi.yml
  format: yaml
  label: NovoPayment Cards API
  slug: cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-cards-openapi.yml
- filename: novopayment-compliance-openapi.yml
  format: yaml
  label: NovoPayment Compliance API
  slug: compliance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-compliance-openapi.yml
- filename: novopayment-customers-openapi.yml
  format: yaml
  label: NovoPayment Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-customers-openapi.yml
- filename: novopayment-issuer-tokenization-openapi.yml
  format: yaml
  label: NovoPayment Issuer Tokenization API
  slug: issuer-tokenization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-issuer-tokenization-openapi.yml
- filename: novopayment-mastercard-issuer-tokenization-openapi.yml
  format: yaml
  label: NovoPayment MasterCard Tokenization API
  slug: mastercard-issuer-tokenization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-mastercard-issuer-tokenization-openapi.yml
- filename: novopayment-merchant-presented-qr-openapi.yml
  format: yaml
  label: NovoPayment Merchant Presented QR
  slug: merchant-presented-qr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-merchant-presented-qr-openapi.yml
- filename: novopayment-oauth2-data-encryption-openapi.yml
  format: yaml
  label: NovoPayment Security OAuth2 API
  slug: oauth2-data-encryption
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-oauth2-data-encryption-openapi.yml
- filename: novopayment-onboarding-openapi.yml
  format: yaml
  label: NovoPayment Onboarding API
  slug: onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-onboarding-openapi.yml
- filename: novopayment-operations-openapi.yml
  format: yaml
  label: NovoPayment Operations API
  slug: operations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-operations-openapi.yml
- filename: novopayment-payment-authorizer-openapi.yml
  format: yaml
  label: NovoPayment Payment Authorizer API
  slug: payment-authorizer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-payment-authorizer-openapi.yml
- filename: novopayment-profile-openapi.yml
  format: yaml
  label: NovoPayment Profile API
  slug: profile
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-profile-openapi.yml
- filename: novopayment-push-provisioning-openapi.yml
  format: yaml
  label: NovoPayment Push Provisioning API
  slug: push-provisioning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-push-provisioning-openapi.yml
- filename: novopayment-real-time-payments-openapi.yml
  format: yaml
  label: NovoPayment Real-Time Payments API
  slug: real-time-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/openapi/novopayment-real-time-payments-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: novopayment.com
  spf: true
hosts:
- cert_expires: Dec  5 03:39:20 2026 GMT
  host: developer.novopayment.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: sandbox-api.novopayment.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: cert-api.novopayment.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Novopayment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NovoPayment, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NovoPayment
provider_slug: novopayment
slug: novopayment-domain-security
source_filename: novopayment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.novopayment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 03:39:20 2026 GMT\n  hsts: false\n- host: sandbox-api.novopayment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\n- host: cert-api.novopayment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: novopayment.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novopayment/refs/heads/main/security/novopayment-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Banking as a Service
- Embedded Finance
- Card Issuing
- Digital Wallet
- Tokenization
- Real-Time Payments
- Onboarding
- KYC
- Latin America
- Fintech
- Digital Banking
---
