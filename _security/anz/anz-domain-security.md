---
api_specs:
- filename: anz-banking-account-balances-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Balances API
  slug: anz-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-balances-api-openapi.yml
- filename: anz-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Direct Debits API
  slug: anz-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-direct-debits-api-openapi.yml
- filename: anz-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Scheduled Payments API
  slug: anz-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-scheduled-payments-api-openapi.yml
- filename: anz-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Transactions API
  slug: anz-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-transactions-api-openapi.yml
- filename: anz-banking-accounts-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Accounts API
  slug: anz-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-accounts-api-openapi.yml
- filename: anz-banking-payees-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Payees API
  slug: anz-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-payees-api-openapi.yml
- filename: anz-banking-products-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Products API
  slug: anz-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-products-api-openapi.yml
- filename: anz-banking-products-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) ANZ Plus Banking Products API
  slug: anz-plus-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anz.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anz.com
  spf: true
hosts:
- cert_expires: Apr 22 23:59:59 2027 GMT
  host: www.anz.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: developer.online.anz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 23 23:59:59 2027 GMT
  host: api.anz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Anz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australia and New Zealand Banking Group (ANZ), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australia and New Zealand Banking Group (ANZ)
provider_slug: anz
slug: anz-domain-security
source_filename: anz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anz.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 22 23:59:59 2027 GMT\n  hsts: null\n- host: developer.online.anz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.anz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: anz.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: anz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/security/anz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
