---
api_specs:
- filename: qfex-openapi-original.yml
  format: yaml
  label: QFEX REST API
  slug: qfex-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qfex/refs/heads/main/openapi/qfex-openapi-original.yml
- filename: qfex-mds-asyncapi.yml
  format: yaml
  label: QFEX Market Data WebSocket (MDS)
  slug: qfex-market-data-websocket-mds
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/qfex/refs/heads/main/asyncapi/qfex-mds-asyncapi.yml
- filename: qfex-trade-asyncapi.yml
  format: yaml
  label: QFEX Trade WebSocket
  slug: qfex-trade-websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/qfex/refs/heads/main/asyncapi/qfex-trade-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: qfex.com
  spf: true
hosts:
- cert_expires: Aug 24 07:33:41 2026 GMT
  host: docs.qfex.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 06:34:48 2026 GMT
  host: api.qfex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 06:34:48 2026 GMT
  host: mds.qfex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qfex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qfex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Qfex
provider_slug: qfex
slug: qfex-domain-security
source_filename: qfex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.qfex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:33:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.qfex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:34:48 2026 GMT\n  hsts: null\n- host: mds.qfex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:34:48 2026 GMT\n  hsts: null\ndomains:\n- domain: qfex.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qfex/refs/heads/main/security/qfex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Trading
- Exchange
- Perpetual Futures
- Market Data
- WebSocket
- FX
- Commodities
- Equities
- Financial Services
- CLI
- Fintech
- Real-time
---
