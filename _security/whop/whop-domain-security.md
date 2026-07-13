---
api_specs:
- filename: whop-openapi.yml
  format: yaml
  label: Whop Memberships API
  slug: whop-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Products API
  slug: whop-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Plans API
  slug: whop-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Payments API
  slug: whop-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Users API
  slug: whop-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Companies API
  slug: whop-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Checkout Configurations API
  slug: whop-checkout-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Transfers API
  slug: whop-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Webhooks API
  slug: whop-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-openapi.yml
  format: yaml
  label: Whop Promo Codes API
  slug: whop-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/openapi/whop-openapi.yml
- filename: whop-asyncapi.yml
  format: yaml
  label: Whop Realtime WebSocket API
  slug: whop-realtime-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/asyncapi/whop-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: whop.com
  spf: true
hosts:
- cert_expires: Oct  5 21:25:28 2026 GMT
  host: whop.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 04:17:11 2026 GMT
  host: docs.whop.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 20:00:39 2026 GMT
  host: api.whop.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whop, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Whop
provider_slug: whop
slug: whop-domain-security
source_filename: whop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:25:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.whop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 04:17:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.whop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:00:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: whop.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whop/refs/heads/main/security/whop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Memberships
- Payments
- Creator Economy
- Marketplace
- Digital Products
- Access Control
- Commerce
---
