---
api_specs:
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Account Holders API
  slug: lithic-com-account-holders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Accounts API
  slug: lithic-com-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Cards API
  slug: lithic-com-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Transactions & Authorizations API
  slug: lithic-com-transactions-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Authorization Rules API
  slug: lithic-com-authorization-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Real-Time Decisioning API
  slug: lithic-com-realtime-decisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Disputes API
  slug: lithic-com-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Events & Webhooks API
  slug: lithic-com-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Financial Accounts & Statements API
  slug: lithic-com-financial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Balances & Holds API
  slug: lithic-com-balances-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Payments (ACH) API
  slug: lithic-com-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Ledger, Transfers & Settlement API
  slug: lithic-com-ledger-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic External Payments & Bank Accounts API
  slug: lithic-com-external-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Tokenization & Digital Wallets API
  slug: lithic-com-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
- filename: lithic-com-openapi.yml
  format: yaml
  label: Lithic Fraud & Transaction Monitoring API
  slug: lithic-com-fraud-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/openapi/lithic-com-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lithic.com
  spf: true
hosts:
- cert_expires: Sep 28 08:19:38 2026 GMT
  host: www.lithic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 14:22:06 2026 GMT
  host: docs.lithic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.lithic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lithic Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lithic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lithic
provider_slug: lithic-com
slug: lithic-com-domain-security
source_filename: lithic-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lithic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:19:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lithic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:22:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lithic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lithic.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lithic-com/refs/heads/main/security/lithic-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Card Issuing
- Payments
- Issuer Processor
- KYC
- Banking as a Service
---
