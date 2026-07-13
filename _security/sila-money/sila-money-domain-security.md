---
api_specs:
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Identity & KYC/KYB API
  slug: sila-money-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Wallets API
  slug: sila-money-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Bank Accounts API
  slug: sila-money-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Payments & Transactions API
  slug: sila-money-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
- filename: sila-money-openapi.yml
  format: yaml
  label: Sila Payment Methods & Cards API
  slug: sila-money-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/openapi/sila-money-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: reject
  dnssec: false
  domain: silamoney.com
  spf: true
  spf_policy: -all
  spf_record: v=spf1 include:spf.mandrillapp.com include:_spf.google.com include:emsd1.com include:spf.autopilothq.com include:sendgrid.net -all
hosts:
- cors_allow_origin: '*'
  host: api.silamoney.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  http_status: 400
  http_version: HTTP/2
  https: true
  origin: sila-prod-lb (AWS ELB, us-west-2)
  server: nginx/1.24.0 (Ubuntu)
  tls_note: Sectigo DV cert, valid May 27 2026 - Dec 11 2026 GMT
  x_content_type_options: nosniff
- host: sandbox.silamoney.com
  https: true
  origin: sila-sandbox-lb (AWS ELB, us-west-2)
  reachable: true
- host: www.silamoney.com
  http_status: 200
  https: true
- host: docs.silamoney.com
  http_status: 200
  https: true
  note: ReadMe-hosted docs (ssl.readmessl.com / Cloudflare), redirects to /docs/get-started.
kind: domain-security
layout: security
method: probed
name: Sila Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sila, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sila
provider_slug: sila-money
slug: sila-money-domain-security
source_filename: sila-money-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nstatus: live\nstatusNote: >-\n  As of 2026-07-12 Sila is operating. DNS resolves for www.silamoney.com,\n  api.silamoney.com (AWS ELB, us-west-2), sandbox.silamoney.com (AWS ELB,\n  us-west-2), and docs.silamoney.com (ReadMe-hosted, Cloudflare). The production\n  API responds - POST https://api.silamoney.com/0.2/check_handle returns HTTP 400\n  with a JSON validation error requiring the signature header - confirming the\n  documented /0.2 surface is live. No acquisition or shutdown was found.\nhosts:\n- host: api.silamoney.com\n  https: true\n  http_version: HTTP/2\n  http_status: 400\n  tls_note: Sectigo DV cert, valid May 27 2026 - Dec 11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  server: nginx/1.24.0 (Ubuntu)\n  x_content_type_options: nosniff\n  cors_allow_origin: '*'\n  origin: sila-prod-lb (AWS ELB, us-west-2)\n- host: sandbox.silamoney.com\n\
  \  https: true\n  reachable: true\n  origin: sila-sandbox-lb (AWS ELB, us-west-2)\n- host: www.silamoney.com\n  https: true\n  http_status: 200\n- host: docs.silamoney.com\n  https: true\n  http_status: 200\n  note: ReadMe-hosted docs (ssl.readmessl.com / Cloudflare), redirects to /docs/get-started.\ndomains:\n- domain: silamoney.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '-all'\n  spf_record: v=spf1 include:spf.mandrillapp.com include:_spf.google.com include:emsd1.com include:spf.autopilothq.com include:sendgrid.net -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_pct: 100\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sila-money/refs/heads/main/security/sila-money-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Embedded Finance
- Banking as a Service
- Payments
- Digital Wallet
- ACH
- KYC
- KYB
- Money Transfer
- Fintech
- Banking API
- Virtual Accounts
---
