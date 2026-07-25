---
api_specs:
- filename: zai-assembly-api.json
  format: json
  label: Zai Assembly API
  slug: zai-assembly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-assembly-api.json
- filename: zai-virtual-accounts-payid.json
  format: json
  label: Zai Virtual Accounts and PayIDs API
  slug: zai-virtual-accounts-payid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-virtual-accounts-payid.json
- filename: zai-payto.json
  format: json
  label: Zai PayTo API
  slug: zai-payto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-payto.json
- filename: zai-async-api.json
  format: json
  label: Zai Asynchronous API
  slug: zai-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-async-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hellozai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: promisepay.com
  spf: true
hosts:
- cert_expires: Sep  4 12:48:14 2026 GMT
  host: www.hellozai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:10:09 2026 GMT
  host: developer.hellozai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: secure.api.promisepay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zai
provider_slug: zai
slug: zai-domain-security
source_filename: zai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hellozai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 12:48:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hellozai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:10:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure.api.promisepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hellozai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: promisepay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/security/zai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Marketplace Payments
- Payments-as-a-Service
- Real-Time Payments
- Account-to-Account
- Open Banking
- PayTo
- PayID
- NPP
- Direct Debit
- Digital Wallets
- Payouts
---
