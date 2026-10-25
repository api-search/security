---
api_specs:
- filename: commonwealth-bank-accounts-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Accounts API
  slug: commonwealth-bank-accounts-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-accounts-api-api-openapi.yml
- filename: commonwealth-bank-balances-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Balances API
  slug: commonwealth-bank-balances-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-balances-api-api-openapi.yml
- filename: commonwealth-bank-customer-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Customer API
  slug: commonwealth-bank-customer-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-customer-api-api-openapi.yml
- filename: commonwealth-bank-payees-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Payees API
  slug: commonwealth-bank-payees-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-payees-api-api-openapi.yml
- filename: commonwealth-bank-products-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Products API
  slug: commonwealth-bank-products-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-products-api-api-openapi.yml
- filename: commonwealth-bank-regular-payments-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Regular Payments API
  slug: commonwealth-bank-regular-payments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-regular-payments-api-api-openapi.yml
- filename: commonwealth-bank-transaction-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Transaction API
  slug: commonwealth-bank-transaction-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-transaction-api-api-openapi.yml
- filename: commonwealth-bank-accounts-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Accounts API
  slug: commonwealth-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-accounts-api-openapi.yml
- filename: commonwealth-bank-agreements-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Agreements API
  slug: commonwealth-bank-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-agreements-api-openapi.yml
- filename: commonwealth-bank-credit-transfer-initiations-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Credit Transfer Initiations API
  slug: commonwealth-bank-credit-transfer-initiations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-credit-transfer-initiations-api-openapi.yml
- filename: commonwealth-bank-discovery-api-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Discovery API
  slug: commonwealth-bank-discovery-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-discovery-api-api-openapi.yml
- filename: commonwealth-bank-partner-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Partner API
  slug: commonwealth-bank-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-partner-api-openapi.yml
- filename: commonwealth-bank-payments-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Payments API
  slug: commonwealth-bank-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-payments-api-openapi.yml
- filename: commonwealth-bank-utilities-api-openapi.yml
  format: yaml
  label: Commonwealth Bank Utilities API
  slug: commonwealth-bank-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/openapi/commonwealth-bank-utilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: commbank.com.au
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: developer.api.commbank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.commbank.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: paymentgateway.commbank.com.au
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Commonwealth Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commonwealth Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Commonwealth Bank
provider_slug: commonwealth-bank
slug: commonwealth-bank-domain-security
source_filename: commonwealth-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.api.commbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.commbank.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: paymentgateway.commbank.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: commbank.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commonwealth-bank/refs/heads/main/security/commonwealth-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Banks
- Consumer Banking
- Business Banking
- Open Banking
- CDR
- Product Reference Data
- ADI
- Australia
---
