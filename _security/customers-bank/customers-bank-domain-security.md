---
api_specs:
- filename: customers-bank-accounts-openapi.json
  format: json
  label: Customers Bank Accounts API
  slug: customers-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-accounts-openapi.json
- filename: customers-bank-ach-openapi.json
  format: json
  label: Customers Bank ACH API
  slug: customers-bank-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-ach-openapi.json
- filename: customers-bank-consumerlending-openapi.json
  format: json
  label: Customers Bank Consumer Lending API
  slug: customers-bank-consumer-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-consumerlending-openapi.json
- filename: customers-bank-instantpayments-openapi.json
  format: json
  label: Customers Bank Instant Payments API
  slug: customers-bank-instant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-instantpayments-openapi.json
- filename: customers-bank-itoperations-openapi.json
  format: json
  label: Customers Bank IT Operations API
  slug: customers-bank-it-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-itoperations-openapi.json
- filename: customers-bank-partners-openapi.json
  format: json
  label: Customers Bank Partners API
  slug: customers-bank-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-partners-openapi.json
- filename: customers-bank-security-openapi.json
  format: json
  label: Customers Bank Security API
  slug: customers-bank-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-security-openapi.json
- filename: customers-bank-transfers-openapi.json
  format: json
  label: Customers Bank Transfers API
  slug: customers-bank-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-transfers-openapi.json
- filename: customers-bank-webhooks-openapi.json
  format: json
  label: Customers Bank Webhooks API
  slug: customers-bank-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-webhooks-openapi.json
- filename: customers-bank-wires-openapi.json
  format: json
  label: Customers Bank Wires API
  slug: customers-bank-wires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/openapi/customers-bank-wires-openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: customersbank.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct 19 13:41:29 2026 GMT
  host: www.customersbank.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: cubiapi.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 13:41:29 2026 GMT
  host: cubi-sandbox-api.customersbank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Customers Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Customers Bank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Customers Bank
provider_slug: customers-bank
slug: customers-bank-domain-security
source_filename: customers-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.customersbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 13:41:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: cubiapi.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cubi-sandbox-api.customersbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 13:41:29 2026 GMT\n  hsts: null\ndomains:\n- domain: customersbank.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customers-bank/refs/heads/main/security/customers-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Banking as a Service
- Embedded Finance
- Payments
- Commercial Banking
---
