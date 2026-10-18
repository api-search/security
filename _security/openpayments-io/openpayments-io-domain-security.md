---
api_specs:
- filename: openpayments-io-account-information-service-ais-api-openapi.yml
  format: yaml
  label: Open Payments Account Information Service (AIS) API
  slug: openpayments-io-account-information-service-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-account-information-service-ais-api-openapi.yml
- filename: openpayments-io-aspsp-information-service-api-openapi.yml
  format: yaml
  label: Open Payments ASPSP Information Service API
  slug: openpayments-io-aspsp-information-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-aspsp-information-service-api-openapi.yml
- filename: openpayments-io-bankgiro-lookup-api-openapi.yml
  format: yaml
  label: Open Payments Bankgiro Lookup API
  slug: openpayments-io-bankgiro-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-bankgiro-lookup-api-openapi.yml
- filename: openpayments-io-consent-service-api-openapi.yml
  format: yaml
  label: Open Payments Consent Service API
  slug: openpayments-io-consent-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-consent-service-api-openapi.yml
- filename: openpayments-io-fx-connect-api-openapi.yml
  format: yaml
  label: Open Payments FX Connect API
  slug: openpayments-io-fx-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-fx-connect-api-openapi.yml
- filename: openpayments-io-iso-payments-api-openapi.yml
  format: yaml
  label: Open Payments ISO Payments API
  slug: openpayments-io-iso-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-iso-payments-api-openapi.yml
- filename: openpayments-io-kyc-service-api-openapi.yml
  format: yaml
  label: Open Payments KYC Service API
  slug: openpayments-io-kyc-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-kyc-service-api-openapi.yml
- filename: openpayments-io-payment-initiation-service-pis-api-openapi.yml
  format: yaml
  label: Open Payments Payment Initiation Service (PIS) API
  slug: openpayments-io-payment-initiation-service-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-payment-initiation-service-pis-api-openapi.yml
- filename: openpayments-io-payout-service-api-openapi.yml
  format: yaml
  label: Open Payments Payout Service API
  slug: openpayments-io-payout-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-payout-service-api-openapi.yml
- filename: openpayments-io-sepa-direct-debit-api-openapi.yml
  format: yaml
  label: Open Payments SEPA Direct Debit API
  slug: openpayments-io-sepa-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-sepa-direct-debit-api-openapi.yml
- filename: openpayments-io-verification-of-payee-vop-api-openapi.yml
  format: yaml
  label: Open Payments Verification of Payee (VoP) API
  slug: openpayments-io-verification-of-payee-vop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-verification-of-payee-vop-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openpayments.io
  spf: true
hosts:
- cert_expires: Nov 30 17:49:30 2026 GMT
  host: openpayments.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openpayments Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Payments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Payments
provider_slug: openpayments-io
slug: openpayments-io-domain-security
source_filename: openpayments-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openpayments.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 17:49:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openpayments.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/security/openpayments-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Banking
- Fintech
---
