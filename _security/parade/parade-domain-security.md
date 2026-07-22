---
api_specs:
- filename: parade-digital-transactions-openapi.yaml
  format: yaml
  label: Parade Transactions API
  slug: parade-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-digital-transactions-openapi.yaml
- filename: parade-load-sync-openapi.yaml
  format: yaml
  label: Parade Load Feed
  slug: parade-load-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-load-sync-openapi.yaml
- filename: parade-partner-webhooks-openapi.yaml
  format: yaml
  label: Parade Syndication Webhooks
  slug: parade-syndication-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/openapi/parade-partner-webhooks-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parade.ai
  spf: true
hosts:
- cert_expires: Sep 25 23:53:34 2026 GMT
  host: parade.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 11:21:37 2026 GMT
  host: api.capacity.stage.parade.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 15:09:01 2026 GMT
  host: api.syndication.stage.parade.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Parade
provider_slug: parade
slug: parade-domain-security
source_filename: parade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parade.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:53:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.capacity.stage.parade.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 11:21:37 2026 GMT\n  hsts: false\n- host: api.syndication.stage.parade.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 15:09:01 2026 GMT\n  hsts: null\ndomains:\n- domain: parade.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parade/refs/heads/main/security/parade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Freight
- Logistics
- Trucking
- Supply Chain
- Capacity Management
- Freight Brokerage
- Transportation
- Load Board
- Artificial Intelligence
---
