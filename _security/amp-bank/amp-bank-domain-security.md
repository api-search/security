---
api_specs:
- filename: amp-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Balances API
  slug: amp-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-balances-api-openapi.yml
- filename: amp-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Direct Debits API
  slug: amp-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-direct-debits-api-openapi.yml
- filename: amp-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Scheduled Payments API
  slug: amp-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: amp-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Account Transactions API
  slug: amp-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-account-transactions-api-openapi.yml
- filename: amp-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Accounts API
  slug: amp-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-accounts-api-openapi.yml
- filename: amp-bank-banking-payees-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Payees API
  slug: amp-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-payees-api-openapi.yml
- filename: amp-bank-banking-products-api-openapi.yml
  format: yaml
  label: AMP Bank Banking Products API
  slug: amp-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: amp.com.au
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.amp.com.au
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: api.cdr-api.amp.com.au
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: pub.cdr-sme.amp.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amp Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMP Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AMP Bank
provider_slug: amp-bank
slug: amp-bank-domain-security
source_filename: amp-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amp.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.cdr-api.amp.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: null\n- host: pub.cdr-sme.amp.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amp.com.au\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/security/amp-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
---
