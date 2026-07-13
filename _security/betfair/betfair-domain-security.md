---
api_specs:
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Betting API
  slug: betfair-betting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Accounts API
  slug: betfair-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Heartbeat API
  slug: betfair-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
- filename: betfair-asyncapi.yml
  format: yaml
  label: Betfair Exchange Stream API
  slug: betfair-exchange-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/asyncapi/betfair-asyncapi.yml
- filename: betfair-openapi.yml
  format: yaml
  label: Betfair Historic Data API
  slug: betfair-historic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/openapi/betfair-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: betfair.com
  spf: true
hosts:
- cert_expires: Sep 12 16:17:03 2026 GMT
  host: www.betfair.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 13:27:23 2026 GMT
  host: developer.betfair.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 09:28:59 2026 GMT
  host: api.betfair.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betfair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Betfair, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Betfair
provider_slug: betfair
slug: betfair-domain-security
source_filename: betfair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betfair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:17:03 2026 GMT\n  hsts: null\n- host: developer.betfair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:27:23 2026 GMT\n  hsts: null\n- host: api.betfair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 09:28:59 2026 GMT\n  hsts: null\ndomains:\n- domain: betfair.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betfair/refs/heads/main/security/betfair-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Betting Exchange
- Sports Betting
- Wagering
- Trading
- Market Data
- JSON-RPC
- Streaming
---
