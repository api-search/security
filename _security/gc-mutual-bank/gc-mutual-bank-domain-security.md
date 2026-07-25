---
api_specs:
- filename: gc-mutual-bank-banking-account-balances-api-openapi.yml
  format: yaml
  label: G&C Mutual Bank Banking Account Balances API
  slug: gc-mutual-bank-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-banking-account-balances-api-openapi.yml
- filename: gc-mutual-bank-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: G&C Mutual Bank Banking Account Direct Debits API
  slug: gc-mutual-bank-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-banking-account-direct-debits-api-openapi.yml
- filename: gc-mutual-bank-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: G&C Mutual Bank Banking Account Scheduled Payments API
  slug: gc-mutual-bank-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-banking-account-scheduled-payments-api-openapi.yml
- filename: gc-mutual-bank-banking-account-transactions-api-openapi.yml
  format: yaml
  label: G&C Mutual Bank Banking Account Transactions API
  slug: gc-mutual-bank-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-banking-account-transactions-api-openapi.yml
- filename: gc-mutual-bank-banking-accounts-api-openapi.yml
  format: yaml
  label: G&C Mutual Bank Banking Accounts API
  slug: gc-mutual-bank-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-banking-accounts-api-openapi.yml
- filename: gc-mutual-bank-banking-payees-api-openapi.yml
  format: yaml
  label: G&C Mutual Bank Banking Payees API
  slug: gc-mutual-bank-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-banking-payees-api-openapi.yml
- filename: gc-mutual-bank-banking-products-api-openapi.yml
  format: yaml
  label: G&C Mutual Bank Banking Products API
  slug: gc-mutual-bank-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/openapi/gc-mutual-bank-banking-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unity.bank
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gcmutualbank.com.au
  spf: true
hosts:
- host: unity.bank
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: ibank.gcmutualbank.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gc Mutual Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for G&C Mutual Bank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: G&C Mutual Bank
provider_slug: gc-mutual-bank
slug: gc-mutual-bank-domain-security
source_filename: gc-mutual-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unity.bank\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: ibank.gcmutualbank.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: unity.bank\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gcmutualbank.com.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gc-mutual-bank/refs/heads/main/security/gc-mutual-bank-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Mutual Bank
- Australia
---
