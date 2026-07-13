---
api_specs:
- filename: kraken-spot-rest-openapi.yml
  format: yaml
  label: Kraken Spot REST API
  slug: kraken-spot-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/openapi/kraken-spot-rest-openapi.yml
- filename: kraken-asyncapi.yml
  format: yaml
  label: Kraken Spot WebSocket API v2
  slug: kraken-spot-websocket-api-v2
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/asyncapi/kraken-asyncapi.yml
- filename: kraken-futures-rest-openapi.yml
  format: yaml
  label: Kraken Futures REST API
  slug: kraken-futures-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/openapi/kraken-futures-rest-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:certificate-abuse@kraken.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kraken.com
  spf: true
hosts:
- cert_expires: Sep 28 00:33:58 2026 GMT
  host: www.kraken.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 08:05:46 2026 GMT
  host: docs.kraken.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 10:41:00 2026 GMT
  host: api.kraken.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kraken Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kraken, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kraken
provider_slug: kraken
slug: kraken-domain-security
source_filename: kraken-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kraken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:33:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kraken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 08:05:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kraken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:41:00 2026 GMT\n  hsts: null\ndomains:\n- domain: kraken.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:certificate-abuse@kraken.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kraken/refs/heads/main/security/kraken-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Spot Trading
- Futures
- Derivatives
- Staking
- Earn
- NFT
- WebSocket
- FIX
- Custody
- OTC
- Prime Brokerage
- Embed
- OAuth
- Public APIs
---
