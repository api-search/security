---
api_specs:
- filename: allica-bank-account-access-api-openapi.yml
  format: yaml
  label: Allica Bank Account Access API
  slug: allica-bank-account-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-account-access-api-openapi.yml
- filename: allica-bank-accounts-api-openapi.yml
  format: yaml
  label: Allica Bank Accounts API
  slug: allica-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-accounts-api-openapi.yml
- filename: allica-bank-balances-api-openapi.yml
  format: yaml
  label: Allica Bank Balances API
  slug: allica-bank-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-balances-api-openapi.yml
- filename: allica-bank-beneficiaries-api-openapi.yml
  format: yaml
  label: Allica Bank Beneficiaries API
  slug: allica-bank-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-beneficiaries-api-openapi.yml
- filename: allica-bank-direct-debits-api-openapi.yml
  format: yaml
  label: Allica Bank Direct Debits API
  slug: allica-bank-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-direct-debits-api-openapi.yml
- filename: allica-bank-domestic-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Payments API
  slug: allica-bank-domestic-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-payments-api-openapi.yml
- filename: allica-bank-domestic-scheduled-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Scheduled Payments API
  slug: allica-bank-domestic-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-scheduled-payments-api-openapi.yml
- filename: allica-bank-domestic-standing-orders-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Standing Orders API
  slug: allica-bank-domestic-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-standing-orders-api-openapi.yml
- filename: allica-bank-file-payments-api-openapi.yml
  format: yaml
  label: Allica Bank File Payments API
  slug: allica-bank-file-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-file-payments-api-openapi.yml
- filename: allica-bank-offers-api-openapi.yml
  format: yaml
  label: Allica Bank Offers API
  slug: allica-bank-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-offers-api-openapi.yml
- filename: allica-bank-parties-api-openapi.yml
  format: yaml
  label: Allica Bank Parties API
  slug: allica-bank-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-parties-api-openapi.yml
- filename: allica-bank-payment-details-api-openapi.yml
  format: yaml
  label: Allica Bank Payment Details API
  slug: allica-bank-payment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-payment-details-api-openapi.yml
- filename: allica-bank-products-api-openapi.yml
  format: yaml
  label: Allica Bank Products API
  slug: allica-bank-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-products-api-openapi.yml
- filename: allica-bank-scheduled-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Scheduled Payments API
  slug: allica-bank-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-scheduled-payments-api-openapi.yml
- filename: allica-bank-standing-orders-api-openapi.yml
  format: yaml
  label: Allica Bank Standing Orders API
  slug: allica-bank-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-standing-orders-api-openapi.yml
- filename: allica-bank-transactions-api-openapi.yml
  format: yaml
  label: Allica Bank Transactions API
  slug: allica-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: allica.bank
  spf: true
hosts:
- cert_expires: Sep 23 13:24:04 2026 GMT
  host: www.allica.bank
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: developer.api.ob.allica.bank
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: rs1.api.ob.allica.bank
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Allica Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allica Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Allica Bank
provider_slug: allica-bank
slug: allica-bank-domain-security
source_filename: allica-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allica.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:24:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.api.ob.allica.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rs1.api.ob.allica.bank\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: allica.bank\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/security/allica-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- SME
- Business Banking
- Fintech
---
