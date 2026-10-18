---
api_specs:
- filename: moneygram-accounts-api-openapi.yml
  format: yaml
  label: MoneyGram Accounts API
  slug: moneygram-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-accounts-api-openapi.yml
- filename: moneygram-amend-api-openapi.yml
  format: yaml
  label: MoneyGram Amend API
  slug: moneygram-amend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-amend-api-openapi.yml
- filename: moneygram-fx-rate-api-openapi.yml
  format: yaml
  label: MoneyGram Fx Rate API
  slug: moneygram-fx-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-fx-rate-api-openapi.yml
- filename: moneygram-oauth-api-openapi.yml
  format: yaml
  label: MoneyGram OAuth API
  slug: moneygram-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-oauth-api-openapi.yml
- filename: moneygram-partnerconnect-api-openapi.yml
  format: yaml
  label: MoneyGram Partnerconnect API
  slug: moneygram-partnerconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-partnerconnect-api-openapi.yml
- filename: moneygram-reference-data-api-openapi.yml
  format: yaml
  label: MoneyGram Reference Data API
  slug: moneygram-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-reference-data-api-openapi.yml
- filename: moneygram-transactions-api-openapi.yml
  format: yaml
  label: MoneyGram Transactions API
  slug: moneygram-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-transactions-api-openapi.yml
- filename: moneygram-transfer-api-openapi.yml
  format: yaml
  label: MoneyGram Transfer API
  slug: moneygram-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-transfer-api-openapi.yml
- filename: moneygram-transfers-api-openapi.yml
  format: yaml
  label: MoneyGram Transfers API
  slug: moneygram-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/openapi/moneygram-transfers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moneygram.com
  spf: true
hosts:
- cert_expires: Apr  9 01:21:16 2027 GMT
  host: www.moneygram.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moneygram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoneyGram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MoneyGram
provider_slug: moneygram
slug: moneygram-domain-security
source_filename: moneygram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moneygram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  9 01:21:16 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: moneygram.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneygram/refs/heads/main/security/moneygram-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Money
- Payments
- Transfer
- Fintech
- Global
---
