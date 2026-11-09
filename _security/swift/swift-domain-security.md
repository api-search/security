---
api_specs:
- filename: swift-payment-pre-validation-api-openapi.yml
  format: yaml
  label: Payment Pre-validation API
  slug: payment-pre-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-payment-pre-validation-api-openapi.yml
- filename: swift-account-numbers-api-openapi.yml
  format: yaml
  label: SWIFT Account Numbers API
  slug: swift-account-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-account-numbers-api-openapi.yml
- filename: swift-bbans-api-openapi.yml
  format: yaml
  label: SWIFT BBANs API
  slug: swift-bbans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-bbans-api-openapi.yml
- filename: swift-bics-api-openapi.yml
  format: yaml
  label: SWIFT BICs API
  slug: swift-bics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-bics-api-openapi.yml
- filename: swift-country-codes-api-openapi.yml
  format: yaml
  label: SWIFT Country Codes API
  slug: swift-country-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-country-codes-api-openapi.yml
- filename: swift-currency-codes-api-openapi.yml
  format: yaml
  label: SWIFT Currency Codes API
  slug: swift-currency-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-currency-codes-api-openapi.yml
- filename: swift-leis-api-openapi.yml
  format: yaml
  label: SWIFT LEIs API
  slug: swift-leis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-leis-api-openapi.yml
- filename: swift-national-ids-api-openapi.yml
  format: yaml
  label: SWIFT National IDs API
  slug: swift-national-ids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-national-ids-api-openapi.yml
- filename: swift-ibans-api-openapi.yml
  format: yaml
  label: SWIFT IBANs API
  slug: swift-ibans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-ibans-api-openapi.yml
- filename: swift-account-information-api-openapi.yml
  format: yaml
  label: SWIFT Account Information API
  slug: swift-account-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-account-information-api-openapi.yml
- filename: swift-distributions-api-openapi.yml
  format: yaml
  label: SWIFT Distributions API
  slug: swift-distributions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-distributions-api-openapi.yml
- filename: swift-fileact-api-openapi.yml
  format: yaml
  label: SWIFT Fileact API
  slug: swift-fileact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-fileact-api-openapi.yml
- filename: swift-fin-api-openapi.yml
  format: yaml
  label: SWIFT Fin API
  slug: swift-fin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-fin-api-openapi.yml
- filename: swift-get-changed-payment-transactions-api-openapi.yml
  format: yaml
  label: SWIFT Get Changed Payment Transactions API
  slug: swift-get-changed-payment-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-get-changed-payment-transactions-api-openapi.yml
- filename: swift-get-payment-transaction-details-api-openapi.yml
  format: yaml
  label: SWIFT Get Payment Transaction Details API
  slug: swift-get-payment-transaction-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-get-payment-transaction-details-api-openapi.yml
- filename: swift-iban-national-ids-api-openapi.yml
  format: yaml
  label: SWIFT Iban National IDs API
  slug: swift-iban-national-ids-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-iban-national-ids-api-openapi.yml
- filename: swift-interact-api-openapi.yml
  format: yaml
  label: SWIFT Interact API
  slug: swift-interact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-interact-api-openapi.yml
- filename: swift-pmis-api-openapi.yml
  format: yaml
  label: SWIFT Pmis API
  slug: swift-pmis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-pmis-api-openapi.yml
- filename: swift-reporting-api-openapi.yml
  format: yaml
  label: SWIFT Reporting API
  slug: swift-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-reporting-api-openapi.yml
- filename: swift-status-confirmations-api-openapi.yml
  format: yaml
  label: SWIFT Status Confirmations API
  slug: swift-status-confirmations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swift/openapi/swift-status-confirmations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swift.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.swift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developer.swift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.swift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Swift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SWIFT, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SWIFT
provider_slug: swift
slug: swift-domain-security
source_filename: swift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: developer.swift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: api.swift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: swift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/swift/security/swift-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Banking
- Cross-Border Payments
- Financial Messaging
- Financial Services
- GPI
- ISO 20022
- Payments
- SWIFT
---
