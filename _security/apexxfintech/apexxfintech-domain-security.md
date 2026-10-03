---
api_specs:
- filename: apexxfintech-alternative-payment-methods-api-openapi.yml
  format: yaml
  label: Apexxfintech Alternative Payment Methods API
  slug: apexxfintech-alternative-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-alternative-payment-methods-api-openapi.yml
- filename: apexxfintech-buy-now-pay-later-api-openapi.yml
  format: yaml
  label: Apexxfintech Buy Now Pay Later API
  slug: apexxfintech-buy-now-pay-later-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-buy-now-pay-later-api-openapi.yml
- filename: apexxfintech-create-and-manage-card-token-api-openapi.yml
  format: yaml
  label: Apexxfintech Create And Manage Card Token API
  slug: apexxfintech-create-and-manage-card-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-create-and-manage-card-token-api-openapi.yml
- filename: apexxfintech-credit-transaction-api-openapi.yml
  format: yaml
  label: Apexxfintech Credit Transaction API
  slug: apexxfintech-credit-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-credit-transaction-api-openapi.yml
- filename: apexxfintech-get-transactions-api-openapi.yml
  format: yaml
  label: Apexxfintech Get Transactions API
  slug: apexxfintech-get-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-get-transactions-api-openapi.yml
- filename: apexxfintech-hosted-token-api-openapi.yml
  format: yaml
  label: Apexxfintech Hosted Token API
  slug: apexxfintech-hosted-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-hosted-token-api-openapi.yml
- filename: apexxfintech-sdk-api-openapi.yml
  format: yaml
  label: Apexxfintech SDK API
  slug: apexxfintech-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-sdk-api-openapi.yml
- filename: apexxfintech-server-side-encryption-api-openapi.yml
  format: yaml
  label: Apexxfintech SERVER-SIDE ENCRYPTION API
  slug: apexxfintech-server-side-encryption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-server-side-encryption-api-openapi.yml
- filename: apexxfintech-standalone-services-api-openapi.yml
  format: yaml
  label: Apexxfintech STANDALONE SERVICES API
  slug: apexxfintech-standalone-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-standalone-services-api-openapi.yml
- filename: apexxfintech-transaction-hosted-payment-api-openapi.yml
  format: yaml
  label: Apexxfintech Transaction Hosted Payment API
  slug: apexxfintech-transaction-hosted-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-transaction-hosted-payment-api-openapi.yml
- filename: apexxfintech-transaction-payment-api-openapi.yml
  format: yaml
  label: Apexxfintech Transaction Payment API
  slug: apexxfintech-transaction-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-transaction-payment-api-openapi.yml
- filename: apexxfintech-transaction-update-api-openapi.yml
  format: yaml
  label: Apexxfintech Transaction Update API
  slug: apexxfintech-transaction-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/openapi/apexxfintech-transaction-update-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: equityzen.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apexx.global
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: equityzen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 07:33:57 2026 GMT
  host: apexx.global
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Apexxfintech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apexxfintech, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apexxfintech
provider_slug: apexxfintech
slug: apexxfintech-domain-security
source_filename: apexxfintech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: equityzen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\n- host: apexx.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 07:33:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: equityzen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apexx.global\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apexxfintech/refs/heads/main/security/apexxfintech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fintech
- Orchestration
- Global
---
