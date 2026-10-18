---
api_specs:
- filename: ndax-accounts-api-openapi.yml
  format: yaml
  label: NDAX Accounts API
  slug: ndax-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ndax/refs/heads/main/openapi/ndax-accounts-api-openapi.yml
- filename: ndax-instruments-api-openapi.yml
  format: yaml
  label: NDAX Instruments API
  slug: ndax-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ndax/refs/heads/main/openapi/ndax-instruments-api-openapi.yml
- filename: ndax-miscellaneous-api-openapi.yml
  format: yaml
  label: NDAX Miscellaneous API
  slug: ndax-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ndax/refs/heads/main/openapi/ndax-miscellaneous-api-openapi.yml
- filename: ndax-oms-orders-api-openapi.yml
  format: yaml
  label: NDAX OMS Orders API
  slug: ndax-oms-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ndax/refs/heads/main/openapi/ndax-oms-orders-api-openapi.yml
- filename: ndax-products-api-openapi.yml
  format: yaml
  label: NDAX Products API
  slug: ndax-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ndax/refs/heads/main/openapi/ndax-products-api-openapi.yml
- filename: ndax-tickets-api-openapi.yml
  format: yaml
  label: NDAX Tickets API
  slug: ndax-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ndax/refs/heads/main/openapi/ndax-tickets-api-openapi.yml
- filename: ndax-trades-api-openapi.yml
  format: yaml
  label: NDAX Trades API
  slug: ndax-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ndax/refs/heads/main/openapi/ndax-trades-api-openapi.yml
- filename: ndax-users-api-openapi.yml
  format: yaml
  label: NDAX Users API
  slug: ndax-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ndax/refs/heads/main/openapi/ndax-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ndax.io
  spf: true
hosts:
- cert_expires: Jan  3 00:48:24 2027 GMT
  host: ndax.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ndax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NDAX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NDAX
provider_slug: ndax
slug: ndax-domain-security
source_filename: ndax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ndax.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 00:48:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ndax.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ndax/refs/heads/main/security/ndax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- WebSocket
- Canada
---
