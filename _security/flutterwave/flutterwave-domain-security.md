---
api_specs:
- filename: flutterwave-payments-api-openapi.yml
  format: yaml
  label: Flutterwave Payments API
  slug: flutterwave-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-payments-api-openapi.yml
- filename: flutterwave-transfers-api-openapi.yml
  format: yaml
  label: Flutterwave Transfers API
  slug: flutterwave-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-transfers-api-openapi.yml
- filename: flutterwave-settlements-api-openapi.yml
  format: yaml
  label: Flutterwave Settlements API
  slug: flutterwave-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-settlements-api-openapi.yml
- filename: flutterwave-wallets-api-openapi.yml
  format: yaml
  label: Flutterwave Wallets API
  slug: flutterwave-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-wallets-api-openapi.yml
- filename: flutterwave-banks-api-openapi.yml
  format: yaml
  label: Flutterwave Banks API
  slug: flutterwave-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-banks-api-openapi.yml
- filename: flutterwave-webhooks-api-openapi.yml
  format: yaml
  label: Flutterwave Webhooks API
  slug: flutterwave-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/openapi/flutterwave-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flutterwave.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: flutterwave.cloud
  spf: false
hosts:
- cert_expires: Oct  2 00:34:28 2026 GMT
  host: flutterwave.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 20:48:25 2026 GMT
  host: developer.flutterwave.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.flutterwave.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flutterwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flutterwave, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flutterwave
provider_slug: flutterwave
slug: flutterwave-domain-security
source_filename: flutterwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flutterwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:34:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.flutterwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:48:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.flutterwave.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: flutterwave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: flutterwave.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/security/flutterwave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payouts
- Mobile Money
- Cards
- Africa
- Fintech
- Remittance
- Virtual Accounts
- Chargebacks
- Multi-Currency
---
