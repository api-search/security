---
api_specs:
- filename: loopay-affiliate-api-openapi.yml
  format: yaml
  label: Loopay Affiliate API
  slug: loopay-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-affiliate-api-openapi.yml
- filename: loopay-bank-api-openapi.yml
  format: yaml
  label: Loopay Bank API
  slug: loopay-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-bank-api-openapi.yml
- filename: loopay-company-api-openapi.yml
  format: yaml
  label: Loopay Company API
  slug: loopay-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-company-api-openapi.yml
- filename: loopay-companyproduct-api-openapi.yml
  format: yaml
  label: Loopay CompanyProduct API
  slug: loopay-companyproduct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-companyproduct-api-openapi.yml
- filename: loopay-country-api-openapi.yml
  format: yaml
  label: Loopay Country API
  slug: loopay-country-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-country-api-openapi.yml
- filename: loopay-currency-api-openapi.yml
  format: yaml
  label: Loopay Currency API
  slug: loopay-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-currency-api-openapi.yml
- filename: loopay-documenttype-api-openapi.yml
  format: yaml
  label: Loopay DocumentType API
  slug: loopay-documenttype-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-documenttype-api-openapi.yml
- filename: loopay-movements-api-openapi.yml
  format: yaml
  label: Loopay Movements API
  slug: loopay-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-movements-api-openapi.yml
- filename: loopay-paidmethods-api-openapi.yml
  format: yaml
  label: Loopay PaidMethods API
  slug: loopay-paidmethods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-paidmethods-api-openapi.yml
- filename: loopay-payin-api-openapi.yml
  format: yaml
  label: Loopay PayIn API
  slug: loopay-payin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-payin-api-openapi.yml
- filename: loopay-payout-api-openapi.yml
  format: yaml
  label: Loopay Payout API
  slug: loopay-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-payout-api-openapi.yml
- filename: loopay-physicalpoint-api-openapi.yml
  format: yaml
  label: Loopay PhysicalPoint API
  slug: loopay-physicalpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-physicalpoint-api-openapi.yml
- filename: loopay-sourcesofpayment-api-openapi.yml
  format: yaml
  label: Loopay SourcesOfPayment API
  slug: loopay-sourcesofpayment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-sourcesofpayment-api-openapi.yml
- filename: loopay-sourcesofpaymentadmin-api-openapi.yml
  format: yaml
  label: Loopay SourcesOfPaymentAdmin API
  slug: loopay-sourcesofpaymentadmin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-sourcesofpaymentadmin-api-openapi.yml
- filename: loopay-user-api-openapi.yml
  format: yaml
  label: Loopay User API
  slug: loopay-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/openapi/loopay-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: loopay.com
  spf: true
hosts:
- cert_expires: Sep 10 01:43:40 2026 GMT
  host: loopay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.loopay.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Loopay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loopay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Loopay
provider_slug: loopay
slug: loopay-domain-security
source_filename: loopay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loopay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:43:40 2026 GMT\n  hsts: false\n- host: api.loopay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: loopay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loopay/refs/heads/main/security/loopay-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Fintech
- Banking as a Service
- Cross-Border Payments
- Payouts
- Treasury
- Latin America
---
