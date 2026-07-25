---
api_specs:
- filename: macquarie-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Account Balances API
  slug: macquarie-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-account-balances-api-openapi.yml
- filename: macquarie-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Account Direct Debits API
  slug: macquarie-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-account-direct-debits-api-openapi.yml
- filename: macquarie-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Account Scheduled Payments API
  slug: macquarie-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: macquarie-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Account Transactions API
  slug: macquarie-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-account-transactions-api-openapi.yml
- filename: macquarie-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Accounts API
  slug: macquarie-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-accounts-api-openapi.yml
- filename: macquarie-bank-banking-payees-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Payees API
  slug: macquarie-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-payees-api-openapi.yml
- filename: macquarie-bank-banking-products-api-openapi.yml
  format: yaml
  label: Macquarie Bank Banking Products API
  slug: macquarie-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: macquarie.com.au
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: macquariebank.io
  spf: false
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: www.macquarie.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: api.macquariebank.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: developer.macquariebank.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Macquarie Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Macquarie Bank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Macquarie Bank
provider_slug: macquarie-bank
slug: macquarie-bank-domain-security
source_filename: macquarie-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.macquarie.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\n- host: api.macquariebank.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\n- host: developer.macquariebank.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: macquarie.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: macquariebank.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/security/macquarie-bank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
- Payments
---
