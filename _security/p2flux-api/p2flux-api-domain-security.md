---
api_specs:
- filename: p2flux-api-cancellation-api-openapi.yml
  format: yaml
  label: P2Flux API Cancellation API
  slug: p2flux-api-cancellation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-cancellation-api-openapi.yml
- filename: p2flux-api-one-time-payments-api-openapi.yml
  format: yaml
  label: P2Flux API One-time payments API
  slug: p2flux-api-one-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-one-time-payments-api-openapi.yml
- filename: p2flux-api-recurring-payments-api-openapi.yml
  format: yaml
  label: P2Flux API Recurring payments API
  slug: p2flux-api-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-recurring-payments-api-openapi.yml
- filename: p2flux-api-refunds-api-openapi.yml
  format: yaml
  label: P2Flux API Refunds API
  slug: p2flux-api-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-refunds-api-openapi.yml
- filename: p2flux-api-service-api-openapi.yml
  format: yaml
  label: P2Flux API Service API
  slug: p2flux-api-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-service-api-openapi.yml
- filename: p2flux-api-subscriptions-api-openapi.yml
  format: yaml
  label: P2Flux API Subscriptions API
  slug: p2flux-api-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/openapi/p2flux-api-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: p2flux.com
  spf: true
hosts:
- cert_expires: Nov 16 19:08:56 2026 GMT
  host: p2flux.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 13:47:23 2026 GMT
  host: api.p2flux.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 18:53:52 2026 GMT
  host: api-test.p2flux.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: P2Flux Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for P2Flux API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: P2Flux API
provider_slug: p2flux-api
slug: p2flux-api-domain-security
source_filename: p2flux-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: p2flux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 19:08:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.p2flux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 13:47:23 2026 GMT\n  hsts: null\n- host: api-test.p2flux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 18:53:52 2026 GMT\n  hsts: null\ndomains:\n- domain: p2flux.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/p2flux-api/refs/heads/main/security/p2flux-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment API
- Cryptocurrency
- Stablecoins
- USDC
- Base
- Recurring Payments
- Subscription
- Refunds
- Non-Custodial
---
