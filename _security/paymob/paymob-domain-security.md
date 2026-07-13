---
api_specs:
- filename: paymob-intentions-api-openapi.yml
  format: yaml
  label: Paymob Intentions API
  slug: paymob-intentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-intentions-api-openapi.yml
- filename: paymob-accept-api-openapi.yml
  format: yaml
  label: Paymob Accept API
  slug: paymob-accept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-accept-api-openapi.yml
- filename: paymob-subscriptions-api-openapi.yml
  format: yaml
  label: Paymob Subscriptions API
  slug: paymob-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-subscriptions-api-openapi.yml
- filename: paymob-card-tokens-api-openapi.yml
  format: yaml
  label: Paymob Card Tokens API
  slug: paymob-card-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-card-tokens-api-openapi.yml
- filename: paymob-payouts-api-openapi.yml
  format: yaml
  label: Paymob Payouts (Send) API
  slug: paymob-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/openapi/paymob-payouts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paymob.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paymobsolutions.com
  spf: false
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: paymob.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 12:18:15 2026 GMT
  host: developers.paymob.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 17 23:59:59 2026 GMT
  host: payouts.paymobsolutions.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Paymob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paymob, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Paymob
provider_slug: paymob
slug: paymob-domain-security
source_filename: paymob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paymob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: false\n- host: developers.paymob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:18:15 2026 GMT\n  hsts: null\n- host: payouts.paymobsolutions.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paymob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: paymobsolutions.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymob/refs/heads/main/security/paymob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Fintech
- MENA
- MENAP
- Egypt
- Saudi Arabia
- UAE
- Pakistan
- Oman
- Card Payments
- Mobile Wallets
- BNPL
- Payouts
- Subscriptions
---
