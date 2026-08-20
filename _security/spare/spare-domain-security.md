---
api_specs:
- filename: spare-account-api-openapi.yml
  format: yaml
  label: Spare Account API
  slug: spare-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-account-api-openapi.yml
- filename: spare-accountinformationreport-api-openapi.yml
  format: yaml
  label: Spare AccountInformationReport API
  slug: spare-accountinformationreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-accountinformationreport-api-openapi.yml
- filename: spare-balance-api-openapi.yml
  format: yaml
  label: Spare Balance API
  slug: spare-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-balance-api-openapi.yml
- filename: spare-beneficiary-api-openapi.yml
  format: yaml
  label: Spare Beneficiary API
  slug: spare-beneficiary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-beneficiary-api-openapi.yml
- filename: spare-cert-api-openapi.yml
  format: yaml
  label: Spare Cert API
  slug: spare-cert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-cert-api-openapi.yml
- filename: spare-connection-api-openapi.yml
  format: yaml
  label: Spare Connection API
  slug: spare-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-connection-api-openapi.yml
- filename: spare-consent-api-openapi.yml
  format: yaml
  label: Spare Consent API
  slug: spare-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-consent-api-openapi.yml
- filename: spare-customer-api-openapi.yml
  format: yaml
  label: Spare Customer API
  slug: spare-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-customer-api-openapi.yml
- filename: spare-directdebit-api-openapi.yml
  format: yaml
  label: Spare DirectDebit API
  slug: spare-directdebit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-directdebit-api-openapi.yml
- filename: spare-parties-api-openapi.yml
  format: yaml
  label: Spare Parties API
  slug: spare-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-parties-api-openapi.yml
- filename: spare-payment-api-openapi.yml
  format: yaml
  label: Spare Payment API
  slug: spare-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-payment-api-openapi.yml
- filename: spare-provider-api-openapi.yml
  format: yaml
  label: Spare Provider API
  slug: spare-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-provider-api-openapi.yml
- filename: spare-request-api-openapi.yml
  format: yaml
  label: Spare Request API
  slug: spare-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-request-api-openapi.yml
- filename: spare-riskreport-api-openapi.yml
  format: yaml
  label: Spare RiskReport API
  slug: spare-riskreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-riskreport-api-openapi.yml
- filename: spare-statement-api-openapi.yml
  format: yaml
  label: Spare Statement API
  slug: spare-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-statement-api-openapi.yml
- filename: spare-token-api-openapi.yml
  format: yaml
  label: Spare Token API
  slug: spare-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-token-api-openapi.yml
- filename: spare-transaction-api-openapi.yml
  format: yaml
  label: Spare Transaction API
  slug: spare-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-transaction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tryspare.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: tryspare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:09:40 2026 GMT
  host: docs.tryspare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: ob.tryspare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Spare
provider_slug: spare
slug: spare-domain-security
source_filename: spare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryspare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tryspare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:09:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ob.tryspare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tryspare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/security/spare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Open Banking
- Open Finance
- Account Information
- Payment Initiation
- AISP
- PISP
- Consent
- Bank Data
- Transaction
- Balances
- Payments
- Fintech
- MENA
- Saudi Arabia
- Bahrain
- UAE
---
