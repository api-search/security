---
api_specs:
- filename: brite-payments-assets-api-openapi.yml
  format: yaml
  label: Brite Payments Assets API
  slug: brite-payments-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brite-payments/refs/heads/main/openapi/brite-payments-assets-api-openapi.yml
- filename: brite-payments-bank-account-api-openapi.yml
  format: yaml
  label: Brite Payments Bank Account API
  slug: brite-payments-bank-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brite-payments/refs/heads/main/openapi/brite-payments-bank-account-api-openapi.yml
- filename: brite-payments-brite-payments-api-api-openapi.yml
  format: yaml
  label: Brite Payments Brite Payments API
  slug: brite-payments-brite-payments-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brite-payments/refs/heads/main/openapi/brite-payments-brite-payments-api-api-openapi.yml
- filename: brite-payments-callback-api-openapi.yml
  format: yaml
  label: Brite Payments Callback API
  slug: brite-payments-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brite-payments/refs/heads/main/openapi/brite-payments-callback-api-openapi.yml
- filename: brite-payments-session-api-openapi.yml
  format: yaml
  label: Brite Payments Session API
  slug: brite-payments-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brite-payments/refs/heads/main/openapi/brite-payments-session-api-openapi.yml
- filename: brite-payments-transaction-api-openapi.yml
  format: yaml
  label: Brite Payments Transaction API
  slug: brite-payments-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brite-payments/refs/heads/main/openapi/brite-payments-transaction-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: britepayments.com
  spf: true
hosts:
- cert_expires: Jan  8 17:55:07 2027 GMT
  host: britepayments.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brite Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brite Payments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brite Payments
provider_slug: brite-payments
slug: brite-payments-domain-security
source_filename: brite-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: britepayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 17:55:07 2027 GMT\n  hsts: false\ndomains:\n- domain: britepayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brite-payments/refs/heads/main/security/brite-payments-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Fintech
- Europe
- OnlinePayments
---
