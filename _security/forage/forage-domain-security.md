---
api_specs:
- filename: forage-payments-api-openapi.yml
  format: yaml
  label: Forage EBT SNAP Payments API
  slug: forage-ebt-snap-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-payments-api-openapi.yml
- filename: forage-bearer-tokens-api-openapi.yml
  format: yaml
  label: Forage Bearer Tokens API
  slug: forage-bearer-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-bearer-tokens-api-openapi.yml
- filename: forage-card-details-api-openapi.yml
  format: yaml
  label: Forage Card Details API
  slug: forage-card-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-card-details-api-openapi.yml
- filename: forage-custom-sessions-api-openapi.yml
  format: yaml
  label: Forage Custom Sessions API
  slug: forage-custom-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-custom-sessions-api-openapi.yml
- filename: forage-deferred-capture-api-openapi.yml
  format: yaml
  label: Forage Deferred Capture API
  slug: forage-deferred-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-deferred-capture-api-openapi.yml
- filename: forage-fully-hosted-sessions-api-openapi.yml
  format: yaml
  label: Forage Fully Hosted Sessions API
  slug: forage-fully-hosted-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-fully-hosted-sessions-api-openapi.yml
- filename: forage-order-payments-api-openapi.yml
  format: yaml
  label: Forage Order Payments API
  slug: forage-order-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-order-payments-api-openapi.yml
- filename: forage-order-refunds-api-openapi.yml
  format: yaml
  label: Forage Order Refunds API
  slug: forage-order-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-order-refunds-api-openapi.yml
- filename: forage-orders-api-openapi.yml
  format: yaml
  label: Forage Orders API
  slug: forage-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-orders-api-openapi.yml
- filename: forage-payment-methods-api-openapi.yml
  format: yaml
  label: Forage Payment Methods API
  slug: forage-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-payment-methods-api-openapi.yml
- filename: forage-payment-refunds-api-openapi.yml
  format: yaml
  label: Forage Payment Refunds API
  slug: forage-payment-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-payment-refunds-api-openapi.yml
- filename: forage-reports-api-openapi.yml
  format: yaml
  label: Forage Reports API
  slug: forage-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-reports-api-openapi.yml
- filename: forage-sandbox-testing-api-openapi.yml
  format: yaml
  label: Forage Sandbox Testing API
  slug: forage-sandbox-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/openapi/forage-sandbox-testing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinforage.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinforage.app
  spf: false
hosts:
- cert_expires: Sep 22 14:32:05 2026 GMT
  host: www.joinforage.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 16:38:18 2026 GMT
  host: docs.joinforage.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.joinforage.app
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Forage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Forage
provider_slug: forage
slug: forage-domain-security
source_filename: forage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinforage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:32:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.joinforage.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 16:38:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.joinforage.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: joinforage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: joinforage.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forage/refs/heads/main/security/forage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- EBT
- SNAP
- EBT Cash
- HSA/FSA
- Fintech
- Government Benefits
- Grocery
- Checkout
- Financial Services
---
